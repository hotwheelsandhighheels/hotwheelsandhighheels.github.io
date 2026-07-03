---
layout: default
title: Scratch Paper
permalink: /Trunk/scratch-paper/
title: Scratch Paper - Hot Wheels & High Heels
---

# Scratch Paper

<p style="text-align: center; opacity: 0.6; font-style: italic; margin-bottom: 32px;"> </p>

---

<div class="bulletin-board" id="bulletin-board">

  <!-- POST-IT TEMPLATE — copy and fill:
       
       PINK CARD (purple text):
       <div class="post-it pink" style="left: Xpx; top: Ypx; transform: rotate(Zdeg);" draggable="true">
         <p>Your note here.</p>
       </div>
       
       PURPLE CARD (pink text):
       <div class="post-it purple" style="left: Xpx; top: Ypx; transform: rotate(Zdeg);" draggable="true">
         <p>Your note here.</p>
       </div>
       
       Add data-stack="group-name" to cards that belong together.
       Cards with the same stack value will overlap slightly.
  -->

<div class="post-it pink" style="left: 60px; top: 40px; transform: rotate(Zdeg);" draggable="true">
  <p>Whenever there is a memory being remembered we are performing the double perspective. An archive (any archive) performs the double perspective <i>because</i> it is an archive. It is a memory aid; it does memory work.</p>
</div>

<div class="post-it purple" style="left: 360px; top: 60px; transform: rotate(1deg);" draggable="true" data-stack="accidentalarchivist">
  <p>You will never find me. You will always find me.</p>
</div>

<div class="post-it pink" style="left: 375px; top: 75px; transform: rotate(-1deg);" draggable="true" data-stack="accidentalarchivist">
  <p>You are the documentary.</p>
</div>


</div>

<p id="bibliography" style="margin-top: 48px;"><a href="https://www.zotero.org/groups/6565887/millennial_epoch/library" target="_blank">Bibliography</a></p>

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/back-roads/">← Check the road map</a>
  <a href="/submit/">Fill my gas tank →</a>
</div>

<style>
.bulletin-board {
  position: relative;
  width: 100%;
  min-height: 700px;
  background: 
    repeating-conic-gradient(
      var(--bg) 0% 25%,
      transparent 0% 50%
    ) 0 0 / 40px 40px;
  background-color: var(--bg);
  border: 0.5px solid rgba(163, 0, 255, 0.2);
  border-radius: 4px;
  padding: 20px;
  margin: 24px 0;
  overflow: visible;
}

.post-it {
  position: absolute;
  width: 180px;
  min-height: 80px;
  padding: 16px;
  border-radius: 2px;
  cursor: grab;
  user-select: none;
  z-index: 1;
  transition: z-index 0s, box-shadow 0.2s ease;
  font-family: 'Lora', serif;
  font-size: 11pt;
  line-height: 1.5;
}

.post-it:active {
  cursor: grabbing;
}

.post-it:hover {
  z-index: 10;
}

.post-it p {
  margin: 0;
  font-size: 11pt;
  line-height: 1.5;
  font-weight: 600;
}

/* PINK CARD */
.post-it.pink {
  background: rgba(255, 0, 163, 0.2);
  border: 0.5px solid rgba(255, 0, 163, 0.4);
  box-shadow: 2px 2px 8px rgba(255, 0, 163, 0.15);
}

.post-it.pink:hover {
  box-shadow: 2px 2px 16px rgba(255, 0, 163, 0.35);
}

.post-it.pink p {
  color: var(--pink);
}

/* PURPLE CARD */
.post-it.purple {
  background: rgba(163, 0, 255, 0.2);
  border: 0.5px solid rgba(163, 0, 255, 0.4);
  box-shadow: 2px 2px 8px rgba(163, 0, 255, 0.15);
}

.post-it.purple:hover {
  box-shadow: 2px 2px 16px rgba(163, 0, 255, 0.35);
}

.post-it.purple p {
  color: var(--purple);
}

/* STACKED CARDS */
.post-it[data-stack]:hover {
  transform: rotate(0deg) !important;
}

@media (max-width: 600px) {
  .bulletin-board {
    min-height: 500px;
    padding: 12px;
  }
  
  .post-it {
    width: 140px;
    min-height: 60px;
    padding: 12px;
  }
  
  .post-it p {
    font-size: 10pt;
  }
}
</style>

<script>
(function() {
  const board = document.getElementById('bulletin-board');
  if (!board) return;

  let dragCard = null;
  let offsetX = 0;
  let offsetY = 0;
  let hasMoved = false;
  let startX = 0;
  let startY = 0;

  board.addEventListener('mousedown', function(e) {
    const card = e.target.closest('.post-it');
    if (!card) return;
    dragCard = card;
    hasMoved = false;
    const rect = card.getBoundingClientRect();
    offsetX = e.clientX - rect.left;
    offsetY = e.clientY - rect.top;
    startX = e.clientX;
    startY = e.clientY;
    card.style.zIndex = 20;
    card.style.cursor = 'grabbing';
  });

  document.addEventListener('mousemove', function(e) {
    if (!dragCard) return;
    const dx = Math.abs(e.clientX - startX);
    const dy = Math.abs(e.clientY - startY);
    if (dx > 2 || dy > 2) hasMoved = true;
    
    const boardRect = board.getBoundingClientRect();
    const x = e.clientX - boardRect.left - offsetX;
    const y = e.clientY - boardRect.top - offsetY;
    dragCard.style.left = x + 'px';
    dragCard.style.top = y + 'px';
  });

  document.addEventListener('mouseup', function() {
    if (dragCard) {
      dragCard.style.zIndex = 1;
      dragCard.style.cursor = 'grab';
      dragCard = null;
    }
  });

  // Prevent click events from firing after drag
  board.addEventListener('click', function(e) {
    if (hasMoved) {
      e.stopPropagation();
      e.preventDefault();
    }
  }, true);
})();
</script>