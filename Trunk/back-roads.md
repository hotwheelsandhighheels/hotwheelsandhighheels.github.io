---
layout: default
title: Back Roads
permalink: /Trunk/back-roads/
title: Back Roads - Hot Wheels & High Heels
---

# Back Roads
This is a visualization of all the ideas being mapped in the archive. It's a lot messier than I intended it to be but like all pages in the Trunk, it is a work in progress and will be changing as I do more research and add to the archive. You can drag the boxes around, click on them to get a little summary, and if included, a link lets you visit a related page on the site.

*Click to explore. Drag to rearrange. Reset to start over.*

---

<div class="connections-map-wrapper">
<div class="connections-container" id="connections-map">

<!-- NODE PREVIEW POPUP -->
<div class="node-preview" id="node-preview" style="display: none;">
  <div class="node-preview-content">
    <span class="node-preview-close" onclick="closePreview()">close</span>
    <h3 id="preview-title"></h3>
    <p id="preview-type"></p>
    <p id="preview-description"></p>
    <a id="preview-link" href="#">→</a>
  </div>
</div>

<svg class="connections-svg" id="connections-svg"></svg>

<div style="position: absolute; top: 10px; right: 10px; z-index: 30; display: flex; gap: 8px;">
  <button id="reveal-all-btn" style="background: transparent; border: 0.5px solid var(--pink); color: var(--pink); font-family: 'Lora', serif; font-size: 9pt; padding: 4px 10px; cursor: url('/assets/svg/cursor.svg') 8 2, auto; opacity: 0.7;">unfold</button>
  <button id="reset-map-btn" style="background: transparent; border: 0.5px solid var(--purple); color: var(--purple); font-family: 'Lora', serif; font-size: 9pt; padding: 4px 10px; cursor: url('/assets/svg/cursor.svg') 8 2, auto; opacity: 0.7;">fold</button>
</div>

<!-- ============================================
     CENTER NODE
     ============================================ -->
<div class="connection-node center-node" 
     id="CN-0001"
     data-x="600" data-y="400"
     data-depth="0"
     data-children=""
     data-visible="true">
  <h3>Humans</h3>
</div>

<!-- ============================================
     NODE TEMPLATE — copy and fill for each node:
     
     BRANCH NODE (depth 1):
     <div class="connection-node THEME-COLOR-CLASS" 
          id="CN-XXXX" 
          data-x="X" data-y="Y" 
          data-depth="1" 
          data-parent="CN-0001" 
          data-children="CN-XXXX,CN-XXXX">
       <h3>Node Label</h3>
     </div>
     
     CHILD NODE (depth 2+):
     <div class="connection-node THEME-COLOR-CLASS" 
          id="CN-XXXX" 
          data-x="X" data-y="Y" 
          data-depth="2" 
          data-parent="CN-XXXX" 
          data-children="">
       <h3>Node Label</h3>
     </div>
     
     THEME COLOR CLASSES (12 available):
     theme-place, theme-loss, theme-intimacy, theme-web,
     theme-identity, theme-expression, theme-future, theme-care,
     theme-witness, theme-surveillance, theme-emergence, theme-threshold
     
     CENTER NODE uses: center-node
     ============================================ -->

<script>
(function() {
  const container = document.getElementById('connections-map');
  const svg = document.getElementById('connections-svg');
  const allNodes = container.querySelectorAll('.connection-node');
  const nodeClicks = {};

  /*
     EDGE TEMPLATE — add connections between nodes:
     { id: 'CE-XXXX', from: 'CN-XXXX', to: 'CN-XXXX' },
  */
  const connections = [
    // Center → Branch connections go here
    // { id: 'CE-0001', from: 'CN-0001', to: 'CN-0002' },
    
    // Branch → Child connections go here
    // { id: 'CE-XXXX', from: 'CN-XXXX', to: 'CN-XXXX' },
    
    // Cross-connections go here
    // { id: 'CE-XXXX', from: 'CN-XXXX', to: 'CN-XXXX' },
  ];

  allNodes.forEach(node => {
    if (node.id !== 'CN-0001') {
      node.style.display = 'none';
    }
  });

  function showNode(id) {
    const node = document.getElementById(id);
    if (node) {
      node.style.display = 'block';
      drawLines();
    }
  }

  function showChildren(parentId) {
    const parent = document.getElementById(parentId);
    if (!parent) return;
    const childrenIds = parent.getAttribute('data-children');
    if (!childrenIds) return;
    childrenIds.split(',').forEach(id => {
      showNode(id.trim());
    });
  }

  function hideChildren(parentId) {
    const parent = document.getElementById(parentId);
    if (!parent) return;
    const childrenIds = parent.getAttribute('data-children');
    if (!childrenIds) return;
    childrenIds.split(',').forEach(id => {
      const child = document.getElementById(id.trim());
      if (child) {
        child.style.display = 'none';
        const grandKids = child.getAttribute('data-children');
        if (grandKids) {
          grandKids.split(',').forEach(gid => {
            const gchild = document.getElementById(gid.trim());
            if (gchild) gchild.style.display = 'none';
          });
        }
        nodeClicks[id.trim()] = 0;
      }
    });
    drawLines();
  }

  function revealAll() {
    allNodes.forEach(node => {
      node.style.display = 'block';
      nodeClicks[node.id] = 0;
    });
    closePreview();
    drawLines();
  }

  function resetMap() {
    allNodes.forEach(node => {
      if (node.id !== 'CN-0001') {
        node.style.display = 'none';
      }
      nodeClicks[node.id] = 0;
    });
    closePreview();
    drawLines();
  }
  document.getElementById('reveal-all-btn').addEventListener('click', revealAll);
  document.getElementById('reset-map-btn').addEventListener('click', resetMap);
  
  function positionNodes() {
    allNodes.forEach(node => {
      const x = node.getAttribute('data-x');
      const y = node.getAttribute('data-y');
      if (x && y) {
        node.style.left = x + 'px';
        node.style.top = y + 'px';
      }
    });
    drawLines();
  }

  function drawLines() {
    svg.innerHTML = '';
    connections.forEach(conn => {
      const fromNode = document.getElementById(conn.from);
      const toNode = document.getElementById(conn.to);
      if (!fromNode || !toNode) return;
      if (fromNode.style.display === 'none' || toNode.style.display === 'none') return;

      const fromRect = fromNode.getBoundingClientRect();
      const toRect = toNode.getBoundingClientRect();
      const containerRect = container.getBoundingClientRect();

      const x1 = fromRect.left - containerRect.left + fromRect.width / 2;
      const y1 = fromRect.top - containerRect.top + fromRect.height / 2;
      const x2 = toRect.left - containerRect.left + toRect.width / 2;
      const y2 = toRect.top - containerRect.top + toRect.height / 2;

      const line = document.createElementNS('http://www.w3.org/2000/svg', 'line');
      line.setAttribute('x1', x1);
      line.setAttribute('y1', y1);
      line.setAttribute('x2', x2);
      line.setAttribute('y2', y2);
      svg.appendChild(line);
    });
  }

  let dragNode = null;
  let offsetX = 0;
  let offsetY = 0;
  let hasMoved = false;

  container.addEventListener('mousedown', function(e) {
    const node = e.target.closest('.connection-node');
    if (!node) return;
    dragNode = node;
    hasMoved = false;
    const rect = node.getBoundingClientRect();
    offsetX = e.clientX - rect.left;
    offsetY = e.clientY - rect.top;
    node.style.zIndex = 10;
  });

  document.addEventListener('mousemove', function(e) {
    if (!dragNode) return;
    hasMoved = true;
    const containerRect = container.getBoundingClientRect();
    const x = e.clientX - containerRect.left - offsetX;
    const y = e.clientY - containerRect.top - offsetY;
    dragNode.style.left = Math.max(0, Math.min(x, containerRect.width - dragNode.offsetWidth)) + 'px';
    dragNode.style.top = Math.max(0, Math.min(y, containerRect.height - dragNode.offsetHeight)) + 'px';
    drawLines();
  });

  document.addEventListener('mouseup', function() {
    if (dragNode) {
      dragNode.style.zIndex = 1;
      dragNode = null;
    }
  });

  function showPreview(node) {
    const id = node.id;
    const data = previewData[id];
    if (!data) return;

    const preview = document.getElementById('node-preview');
    document.getElementById('preview-title').textContent = data.title;
    document.getElementById('preview-type').textContent = data.type;
    document.getElementById('preview-description').textContent = data.description;

    const link = document.getElementById('preview-link');
    if (data.link) {
      link.href = data.link;
      link.style.display = 'inline';
    } else {
      link.style.display = 'none';
    }

    const nodeRect = node.getBoundingClientRect();
    const containerRect = container.getBoundingClientRect();
    const previewWidth = 320;
    const previewHeight = 220;

    let left = nodeRect.left - containerRect.left + nodeRect.width + 16;
    let top = nodeRect.top - containerRect.top;

    if (left + previewWidth > containerRect.width) {
      left = nodeRect.left - containerRect.left - previewWidth - 16;
    }
    if (top + previewHeight > containerRect.height) {
      top = containerRect.height - previewHeight - 16;
    }
    if (top < 0) top = 16;

    preview.style.left = left + 'px';
    preview.style.top = top + 'px';
    preview.style.transform = 'none';
    preview.style.display = 'block';
  }

  function closePreview() {
    document.getElementById('node-preview').style.display = 'none';
  }

  container.addEventListener('click', function(e) {
    if (hasMoved) return;
    const node = e.target.closest('.connection-node');
    if (!node) {
      closePreview();
      return;
    }
    
    const id = node.id;
    if (!nodeClicks[id]) nodeClicks[id] = 0;
    
    nodeClicks[id]++;
    
    const step = nodeClicks[id];
    const hasChildren = node.getAttribute('data-children');
    
    if (step === 1 && hasChildren) {
      showChildren(id);
    }
    
    if (step === 2) {
      showPreview(node);
    }
    
    if (step === 3) {
      closePreview();
    }
    
    if (step === 4 && hasChildren) {
      hideChildren(id);
      nodeClicks[id] = 0;
    }
    
    if (!hasChildren) {
      if (step === 1) {
        showPreview(node);
      } else if (step === 2) {
        closePreview();
        nodeClicks[id] = 0;
      }
    }
  });

  /*
     PREVIEW DATA TEMPLATE — add one entry per node:
     'CN-XXXX': { title: 'Label', type: '', description: '', link: null },
  */
  const previewData = {
    'CN-0001': { title: 'Humans', type: '', description: '', link: null },
  };

  positionNodes();
  window.addEventListener('resize', drawLines);
})();
</script>
</div>
</div>

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/auto-chopped/">Chopped & Screwed →</a>
  <a href="/Trunk/scratch-paper/">Dig thru the glove box →</a>
</div>

<style>
.connections-map-wrapper {
  width: 100vw;
  margin-left: calc(-50vw + 50%);
  margin-right: calc(-50vw + 50%);
  margin-top: 24px;
  margin-bottom: 24px;
}

.connections-container {
  position: relative;
  width: 100%;
  min-height: 900px;
  overflow: visible;
  margin: 0;
}

.connections-svg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
}

.connections-svg line {
  stroke: var(--pink);
  stroke-width: 0.5px;
  opacity: 0.3;
}

.connection-node {
  position: absolute;
  padding: 8px 14px;
  border: 0.5px solid;
  border-radius: 6px;
  cursor: pointer;
  user-select: none;
  z-index: 1;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
  min-width: 60px;
  text-align: center;
  background: var(--bg);
}

.connection-node:hover {
  box-shadow: 0 0 16px rgba(255, 0, 163, 0.12);
  z-index: 2;
}

.connection-node h3 {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 600;
  font-size: 13pt;
  margin: 0;
  text-transform: none;
  letter-spacing: 0;
  color: inherit;
}

.connection-node.center-node {
  border-color: var(--pink);
  background: rgba(255, 0, 163, 0.06);
}

.connection-node.center-node h3 {
  color: var(--pink);
  font-size: 16pt;
}

.theme-place { border-color: var(--theme-place); color: var(--theme-place); }
.theme-loss { border-color: var(--theme-loss); color: var(--theme-loss); }
.theme-intimacy { border-color: var(--theme-intimacy); color: var(--theme-intimacy); }
.theme-web { border-color: var(--theme-web); color: var(--theme-web); }
.theme-identity { border-color: var(--theme-identity); color: var(--theme-identity); }
.theme-expression { border-color: var(--theme-expression); color: var(--theme-expression); }
.theme-future { border-color: var(--theme-future); color: var(--theme-future); }
.theme-care { border-color: var(--theme-care); color: var(--theme-care); }
.theme-witness { border-color: var(--theme-witness); color: var(--theme-witness); }
.theme-surveillance { border-color: var(--theme-surveillance); color: var(--theme-surveillance); }
.theme-emergence { border-color: var(--theme-emergence); color: var(--theme-emergence); }
.theme-threshold { border-color: var(--theme-threshold); color: var(--theme-threshold); }

.node-preview {
  position: absolute;
  z-index: 20;
  min-width: 280px;
  max-width: 360px;
}

.node-preview-content {
  background: var(--bg);
  border: 0.5px solid var(--pink);
  padding: 20px;
  border-radius: 6px;
  box-shadow: 0 0 24px rgba(255, 0, 163, 0.15);
}

.node-preview-content h3 {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 600;
  font-size: 18pt;
  color: var(--pink);
  margin: 0 0 4px 0;
  text-transform: none;
  letter-spacing: 0;
}

.node-preview-content p {
  font-family: 'Lora', serif;
  font-size: 11pt;
  line-height: 1.6;
  color: var(--text);
  opacity: 0.8;
  margin: 0 0 12px 0;
}

.node-preview-content a {
  font-family: 'Lora', serif;
  font-size: 11pt;
  color: var(--pink);
  text-decoration: none;
}

.node-preview-content a:hover {
  text-decoration: underline;
}

.node-preview-close {
  position: absolute;
  top: 8px;
  right: 12px;
  font-family: 'Lora', serif;
  font-size: 10pt;
  color: var(--pink);
  cursor: pointer;
  opacity: 0.7;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

.node-preview-close:hover {
  opacity: 1;
}

@media (max-width: 600px) {
  .connections-container {
    min-height: 600px;
  }
  
  .connection-node {
    padding: 6px 10px;
    max-width: 120px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  
  .connection-node h3 {
    font-size: 10pt;
  }
  
  .connection-node.center-node h3 {
    font-size: 13pt;
  }
}
</style>