---
layout: default
title: Connections
permalink: /Trunk/connections/
title: Connections - Hot Wheels & High Heels
---

# Connections
This is a visualization of all the ideas being mapped in the archive. It’s a lot messier than I intended it to be but like all pages in the Trunk, it is a work in progress and will be changing as I do more research and add to the archive. You can drag the boxes around, click on them to get a little summary, and if included, a link lets you visit a related page on the site.

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
    <a id="preview-link" href="#">Visit page →</a>
  </div>
</div>

<svg class="connections-svg" id="connections-svg"></svg>

<div style="position: absolute; top: 10px; right: 10px; z-index: 30; display: flex; gap: 8px;">
  <button onclick="revealAll()" style="background: transparent; border: 0.5px solid var(--pink); color: var(--pink); font-family: 'Lora', serif; font-size: 9pt; padding: 4px 10px; cursor: url('/assets/svg/cursor.svg') 8 2, auto; opacity: 0.7;">Reveal All</button>
  <button onclick="resetMap()" style="background: transparent; border: 0.5px solid var(--purple); color: var(--purple); font-family: 'Lora', serif; font-size: 9pt; padding: 4px 10px; cursor: url('/assets/svg/cursor.svg') 8 2, auto; opacity: 0.7;">Reset</button>
</div>

<!-- ============================================
     CENTER
     ============================================ -->
<div class="connection-node center-node" 
     id="node-millennial-epoch"
     data-x="600" data-y="400"
     data-depth="0"
     data-children="node-double-perspective,node-memory,node-the-archive,node-the-drivers,node-memory-technologies,node-berners-lee-web,node-digital-archival-theory,node-surveillance,node-born-digital-objects,node-memory-workers,node-cultural-systems,node-major-tensions,node-central-thesis"
     data-visible="true">
  <h3>Millennial Epoch</h3>
</div>

<!-- ============================================
     BRANCH 1: DOUBLE PERSPECTIVE
     ============================================ -->
<div class="connection-node theme-intimacy" id="node-double-perspective" data-x="600" data-y="200" data-depth="1" data-parent="millennial-epoch" data-children="node-experience-self,node-narrator-self,node-tension,node-archive-codetermination">
  <h3>Double Perspective</h3>
</div>
<div class="connection-node theme-intimacy" id="node-experience-self" data-x="480" data-y="140" data-depth="2" data-parent="double-perspective"><h3>Experience Self</h3></div>
<div class="connection-node theme-intimacy" id="node-narrator-self" data-x="720" data-y="140" data-depth="2" data-parent="double-perspective"><h3>Narrator Self</h3></div>
<div class="connection-node theme-intimacy" id="node-tension" data-x="560" data-y="160" data-depth="2" data-parent="double-perspective"><h3>Tension</h3></div>
<div class="connection-node theme-intimacy" id="node-archive-codetermination" data-x="640" data-y="160" data-depth="2" data-parent="double-perspective"><h3>Archive Codetermination</h3></div>

<!-- ============================================
     BRANCH 2: MEMORY
     ============================================ -->
<div class="connection-node theme-place" id="node-memory" data-x="300" data-y="200" data-depth="1" data-parent="millennial-epoch" data-children="node-personal-memory,node-collective-memory,node-distorted-memory,node-familial-memory,node-witness-memory">
  <h3>Memory</h3>
</div>
<div class="connection-node theme-place" id="node-personal-memory" data-x="180" data-y="140" data-depth="2" data-parent="memory"><h3>Personal Memory</h3></div>
<div class="connection-node theme-place" id="node-collective-memory" data-x="280" data-y="120" data-depth="2" data-parent="memory"><h3>Collective Memory</h3></div>
<div class="connection-node theme-place" id="node-distorted-memory" data-x="380" data-y="130" data-depth="2" data-parent="memory"><h3>Distorted Memory</h3></div>
<div class="connection-node theme-place" id="node-familial-memory" data-x="240" data-y="170" data-depth="2" data-parent="memory"><h3>Familial Memory</h3></div>
<div class="connection-node theme-place" id="node-witness-memory" data-x="340" data-y="170" data-depth="2" data-parent="memory"><h3>Witness</h3></div>

<!-- ============================================
     BRANCH 3: THE ARCHIVE
     ============================================ -->
<div class="connection-node theme-loss" id="node-the-archive" data-x="900" data-y="200" data-depth="1" data-parent="millennial-epoch" data-children="node-traditional-archive,node-digital-archive,node-social-archive-concept,node-archive-fever">
  <h3>The Archive</h3>
</div>
<div class="connection-node theme-loss" id="node-traditional-archive" data-x="780" data-y="130" data-depth="2" data-parent="the-archive"><h3>Traditional Archive</h3></div>
<div class="connection-node theme-loss" id="node-digital-archive" data-x="900" data-y="110" data-depth="2" data-parent="the-archive"><h3>Digital Archive</h3></div>
<div class="connection-node theme-loss" id="node-social-archive-concept" data-x="1020" data-y="130" data-depth="2" data-parent="the-archive"><h3>Social Archive</h3></div>
<div class="connection-node theme-loss" id="node-archive-fever" data-x="940" data-y="170" data-depth="2" data-parent="the-archive"><h3>Archive Fever</h3></div>

<!-- ============================================
     BRANCH 4: THE DRIVERS
     ============================================ -->
<div class="connection-node theme-identity" id="node-the-drivers" data-x="150" data-y="400" data-depth="1" data-parent="millennial-epoch" data-children="node-driver-place,node-driver-loss,node-driver-intimacy,node-driver-web,node-driver-identity,node-driver-expression,node-driver-future,node-driver-care,node-driver-witness,node-driver-surveillance,node-driver-emergence,node-driver-threshold">
  <h3>The Drivers</h3>
</div>
<div class="connection-node theme-place" id="node-driver-place" data-x="30" data-y="340" data-depth="2" data-parent="the-drivers"><h3>Place</h3></div>
<div class="connection-node theme-loss" id="node-driver-loss" data-x="100" data-y="320" data-depth="2" data-parent="the-drivers"><h3>Loss</h3></div>
<div class="connection-node theme-intimacy" id="node-driver-intimacy" data-x="170" data-y="330" data-depth="2" data-parent="the-drivers"><h3>Intimacy</h3></div>
<div class="connection-node theme-web" id="node-driver-web" data-x="220" data-y="350" data-depth="2" data-parent="the-drivers"><h3>Web</h3></div>
<div class="connection-node theme-identity" id="node-driver-identity" data-x="60" data-y="370" data-depth="2" data-parent="the-drivers"><h3>Identity</h3></div>
<div class="connection-node theme-expression" id="node-driver-expression" data-x="130" data-y="380" data-depth="2" data-parent="the-drivers"><h3>Expression</h3></div>
<div class="connection-node theme-future" id="node-driver-future" data-x="200" data-y="390" data-depth="2" data-parent="the-drivers"><h3>Future</h3></div>
<div class="connection-node theme-care" id="node-driver-care" data-x="80" data-y="410" data-depth="2" data-parent="the-drivers"><h3>Care</h3></div>
<div class="connection-node theme-witness" id="node-driver-witness" data-x="150" data-y="420" data-depth="2" data-parent="the-drivers"><h3>Witness</h3></div>
<div class="connection-node theme-surveillance" id="node-driver-surveillance" data-x="220" data-y="430" data-depth="2" data-parent="the-drivers"><h3>Surveillance</h3></div>
<div class="connection-node theme-emergence" id="node-driver-emergence" data-x="50" data-y="450" data-depth="2" data-parent="the-drivers"><h3>Emergence</h3></div>
<div class="connection-node theme-threshold" id="node-driver-threshold" data-x="180" data-y="460" data-depth="2" data-parent="the-drivers"><h3>Threshold</h3></div>

<!-- ============================================
     BRANCH 5: MEMORY TECHNOLOGIES
     ============================================ -->
<div class="connection-node theme-web" id="node-memory-technologies" data-x="1050" data-y="400" data-depth="1" data-parent="millennial-epoch" data-children="node-email,node-forums,node-myspace,node-facebook,node-twitter,node-instagram,node-tiktok,node-smartphones,node-search-engines,node-ai">
  <h3>Memory Technologies</h3>
</div>
<div class="connection-node theme-web" id="node-email" data-x="960" data-y="340" data-depth="2" data-parent="memory-technologies"><h3>Email</h3></div>
<div class="connection-node theme-web" id="node-forums" data-x="1030" data-y="320" data-depth="2" data-parent="memory-technologies"><h3>Forums</h3></div>
<div class="connection-node theme-web" id="node-myspace" data-x="1100" data-y="330" data-depth="2" data-parent="memory-technologies"><h3>MySpace</h3></div>
<div class="connection-node theme-web" id="node-facebook" data-x="1140" data-y="350" data-depth="2" data-parent="memory-technologies"><h3>Facebook</h3></div>
<div class="connection-node theme-web" id="node-twitter" data-x="1080" data-y="370" data-depth="2" data-parent="memory-technologies"><h3>Twitter / X</h3></div>
<div class="connection-node theme-web" id="node-instagram" data-x="1000" data-y="380" data-depth="2" data-parent="memory-technologies"><h3>Instagram</h3></div>
<div class="connection-node theme-web" id="node-tiktok" data-x="1120" data-y="390" data-depth="2" data-parent="memory-technologies"><h3>TikTok</h3></div>
<div class="connection-node theme-web" id="node-smartphones" data-x="1050" data-y="420" data-depth="2" data-parent="memory-technologies"><h3>Smartphones</h3></div>
<div class="connection-node theme-web" id="node-search-engines" data-x="980" data-y="430" data-depth="2" data-parent="memory-technologies"><h3>Search Engines</h3></div>
<div class="connection-node theme-web" id="node-ai" data-x="1100" data-y="440" data-depth="2" data-parent="memory-technologies"><h3>AI</h3></div>

<!-- ============================================
     BRANCH 6: BERNERS-LEE'S WEB
     ============================================ -->
<div class="connection-node theme-expression" id="node-berners-lee-web" data-x="1050" data-y="200" data-depth="1" data-parent="millennial-epoch" data-children="node-hypertext,node-hypermedia,node-universal-access,node-future-proofing,node-global-authorship">
  <h3>Berners-Lee's Web</h3>
</div>
<div class="connection-node theme-expression" id="node-hypertext" data-x="960" data-y="140" data-depth="2" data-parent="berners-lee-web"><h3>Hypertext</h3></div>
<div class="connection-node theme-expression" id="node-hypermedia" data-x="1050" data-y="120" data-depth="2" data-parent="berners-lee-web"><h3>Hypermedia</h3></div>
<div class="connection-node theme-expression" id="node-universal-access" data-x="1140" data-y="140" data-depth="2" data-parent="berners-lee-web"><h3>Universal Access</h3></div>
<div class="connection-node theme-expression" id="node-future-proofing" data-x="1020" data-y="170" data-depth="2" data-parent="berners-lee-web"><h3>Future-Proofing</h3></div>
<div class="connection-node theme-expression" id="node-global-authorship" data-x="1100" data-y="170" data-depth="2" data-parent="berners-lee-web"><h3>Global Authorship</h3></div>

<!-- ============================================
     BRANCH 7: DIGITAL ARCHIVAL THEORY
     ============================================ -->
<div class="connection-node theme-witness" id="node-digital-archival-theory" data-x="900" data-y="500" data-depth="1" data-parent="millennial-epoch" data-children="node-derrida,node-manoff,node-ismail,node-contemporary-archive-studies">
  <h3>Digital Archival Theory</h3>
</div>
<div class="connection-node theme-witness" id="node-derrida" data-x="780" data-y="450" data-depth="2" data-parent="digital-archival-theory"><h3>Derrida</h3></div>
<div class="connection-node theme-witness" id="node-manoff" data-x="880" data-y="440" data-depth="2" data-parent="digital-archival-theory"><h3>Manoff</h3></div>
<div class="connection-node theme-witness" id="node-ismail" data-x="980" data-y="450" data-depth="2" data-parent="digital-archival-theory"><h3>Ismail</h3></div>
<div class="connection-node theme-witness" id="node-contemporary-archive-studies" data-x="920" data-y="480" data-depth="2" data-parent="digital-archival-theory"><h3>Contemporary Studies</h3></div>

<!-- ============================================
     BRANCH 8: SURVEILLANCE
     ============================================ -->
<div class="connection-node theme-surveillance" id="node-surveillance" data-x="300" data-y="550" data-depth="1" data-parent="millennial-epoch" data-children="node-snowden,node-data-extraction,node-algorithmic-profiling,node-platform-governance,node-tracking,node-digital-sobriety">
  <h3>Surveillance</h3>
</div>
<div class="connection-node theme-surveillance" id="node-snowden" data-x="200" data-y="500" data-depth="2" data-parent="surveillance"><h3>Snowden</h3></div>
<div class="connection-node theme-surveillance" id="node-data-extraction" data-x="300" data-y="490" data-depth="2" data-parent="surveillance"><h3>Data Extraction</h3></div>
<div class="connection-node theme-surveillance" id="node-algorithmic-profiling" data-x="400" data-y="500" data-depth="2" data-parent="surveillance"><h3>Algorithmic Profiling</h3></div>
<div class="connection-node theme-surveillance" id="node-platform-governance" data-x="280" data-y="530" data-depth="2" data-parent="surveillance"><h3>Platform Governance</h3></div>
<div class="connection-node theme-surveillance" id="node-tracking" data-x="380" data-y="530" data-depth="2" data-parent="surveillance"><h3>Tracking</h3></div>
<div class="connection-node theme-surveillance" id="node-digital-sobriety" data-x="320" data-y="560" data-depth="2" data-parent="surveillance"><h3>Digital Sobriety</h3></div>

<!-- ============================================
     BRANCH 9: BORN-DIGITAL OBJECTS
     ============================================ -->
<div class="connection-node theme-emergence" id="node-born-digital-objects" data-x="600" data-y="600" data-depth="1" data-parent="millennial-epoch" data-children="node-memes,node-screenshots,node-status-updates,node-stories,node-videos,node-photo-dumps,node-comments">
  <h3>Born-Digital Objects</h3>
</div>
<div class="connection-node theme-emergence" id="node-memes" data-x="480" data-y="550" data-depth="2" data-parent="born-digital-objects"><h3>Memes</h3></div>
<div class="connection-node theme-emergence" id="node-screenshots" data-x="560" data-y="540" data-depth="2" data-parent="born-digital-objects"><h3>Screenshots</h3></div>
<div class="connection-node theme-emergence" id="node-status-updates" data-x="640" data-y="550" data-depth="2" data-parent="born-digital-objects"><h3>Status Updates</h3></div>
<div class="connection-node theme-emergence" id="node-stories" data-x="720" data-y="560" data-depth="2" data-parent="born-digital-objects"><h3>Stories</h3></div>
<div class="connection-node theme-emergence" id="node-videos" data-x="520" data-y="580" data-depth="2" data-parent="born-digital-objects"><h3>Videos</h3></div>
<div class="connection-node theme-emergence" id="node-photo-dumps" data-x="620" data-y="590" data-depth="2" data-parent="born-digital-objects"><h3>Photo Dumps</h3></div>
<div class="connection-node theme-emergence" id="node-comments" data-x="700" data-y="580" data-depth="2" data-parent="born-digital-objects"><h3>Comments</h3></div>

<!-- ============================================
     BRANCH 10: MEMORY WORKERS
     ============================================ -->
<div class="connection-node theme-care" id="node-memory-workers" data-x="150" data-y="600" data-depth="1" data-parent="millennial-epoch" data-children="node-archivists,node-researchers,node-writers,node-poets,node-families,node-everyday-users">
  <h3>Memory Workers</h3>
</div>
<div class="connection-node theme-care" id="node-archivists" data-x="50" data-y="550" data-depth="2" data-parent="memory-workers"><h3>Archivists</h3></div>
<div class="connection-node theme-care" id="node-researchers" data-x="130" data-y="540" data-depth="2" data-parent="memory-workers"><h3>Researchers</h3></div>
<div class="connection-node theme-care" id="node-writers" data-x="200" data-y="550" data-depth="2" data-parent="memory-workers"><h3>Writers</h3></div>
<div class="connection-node theme-care" id="node-poets" data-x="90" data-y="580" data-depth="2" data-parent="memory-workers"><h3>Poets</h3></div>
<div class="connection-node theme-care" id="node-families" data-x="170" data-y="590" data-depth="2" data-parent="memory-workers"><h3>Families</h3></div>
<div class="connection-node theme-care" id="node-everyday-users" data-x="250" data-y="580" data-depth="2" data-parent="memory-workers"><h3>Everyday Users</h3></div>

<!-- ============================================
     BRANCH 11: CULTURAL SYSTEMS
     ============================================ -->
<div class="connection-node theme-expression" id="node-cultural-systems" data-x="1050" data-y="600" data-depth="1" data-parent="millennial-epoch" data-children="node-going-viral,node-parasocial,node-upgrade-you,node-between-you-and-i">
  <h3>Cultural Systems</h3>
</div>
<div class="connection-node theme-expression" id="node-going-viral" data-x="960" data-y="550" data-depth="2" data-parent="cultural-systems"><h3>Going Viral</h3></div>
<div class="connection-node theme-expression" id="node-parasocial" data-x="1060" data-y="540" data-depth="2" data-parent="cultural-systems"><h3>Parasocial</h3></div>
<div class="connection-node theme-expression" id="node-upgrade-you" data-x="1140" data-y="560" data-depth="2" data-parent="cultural-systems"><h3>Upgrade You</h3></div>
<div class="connection-node theme-expression" id="node-between-you-and-i" data-x="1040" data-y="580" data-depth="2" data-parent="cultural-systems"><h3>Between You & I</h3></div>

<!-- ============================================
     BRANCH 12: MAJOR TENSIONS
     ============================================ -->
<div class="connection-node theme-future" id="node-major-tensions" data-x="600" data-y="700" data-depth="1" data-parent="millennial-epoch">
  <h3>Major Tensions</h3>
</div>

<!-- ============================================
     BRANCH 13: CENTRAL THESIS
     ============================================ -->
<div class="connection-node theme-future" id="node-central-thesis" data-x="600" data-y="750" data-depth="1" data-parent="millennial-epoch">
  <h3>Central Thesis</h3>
</div>

<script>
(function() {
  const container = document.getElementById('connections-map');
  const svg = document.getElementById('connections-svg');
  const allNodes = container.querySelectorAll('.connection-node');

  const connections = [
    // Center to all branches
    { from: 'node-millennial-epoch', to: 'node-double-perspective' },
    { from: 'node-millennial-epoch', to: 'node-memory' },
    { from: 'node-millennial-epoch', to: 'node-the-archive' },
    { from: 'node-millennial-epoch', to: 'node-the-drivers' },
    { from: 'node-millennial-epoch', to: 'node-memory-technologies' },
    { from: 'node-millennial-epoch', to: 'node-berners-lee-web' },
    { from: 'node-millennial-epoch', to: 'node-digital-archival-theory' },
    { from: 'node-millennial-epoch', to: 'node-surveillance' },
    { from: 'node-millennial-epoch', to: 'node-born-digital-objects' },
    { from: 'node-millennial-epoch', to: 'node-memory-workers' },
    { from: 'node-millennial-epoch', to: 'node-cultural-systems' },
    { from: 'node-millennial-epoch', to: 'node-major-tensions' },
    { from: 'node-millennial-epoch', to: 'node-central-thesis' },
    
    // Double Perspective internal
    { from: 'node-double-perspective', to: 'node-experience-self' },
    { from: 'node-double-perspective', to: 'node-narrator-self' },
    { from: 'node-double-perspective', to: 'node-tension' },
    { from: 'node-double-perspective', to: 'node-archive-codetermination' },
    
    // Memory internal
    { from: 'node-memory', to: 'node-personal-memory' },
    { from: 'node-memory', to: 'node-collective-memory' },
    { from: 'node-memory', to: 'node-distorted-memory' },
    { from: 'node-memory', to: 'node-familial-memory' },
    { from: 'node-memory', to: 'node-witness-memory' },
    
    // The Archive internal
    { from: 'node-the-archive', to: 'node-traditional-archive' },
    { from: 'node-the-archive', to: 'node-digital-archive' },
    { from: 'node-the-archive', to: 'node-social-archive-concept' },
    { from: 'node-the-archive', to: 'node-archive-fever' },
    
    // The Drivers internal
    { from: 'node-the-drivers', to: 'node-driver-place' },
    { from: 'node-the-drivers', to: 'node-driver-loss' },
    { from: 'node-the-drivers', to: 'node-driver-intimacy' },
    { from: 'node-the-drivers', to: 'node-driver-web' },
    { from: 'node-the-drivers', to: 'node-driver-identity' },
    { from: 'node-the-drivers', to: 'node-driver-expression' },
    { from: 'node-the-drivers', to: 'node-driver-future' },
    { from: 'node-the-drivers', to: 'node-driver-care' },
    { from: 'node-the-drivers', to: 'node-driver-witness' },
    { from: 'node-the-drivers', to: 'node-driver-surveillance' },
    { from: 'node-the-drivers', to: 'node-driver-emergence' },
    { from: 'node-the-drivers', to: 'node-driver-threshold' },
    
    // Memory Technologies internal
    { from: 'node-memory-technologies', to: 'node-email' },
    { from: 'node-memory-technologies', to: 'node-forums' },
    { from: 'node-memory-technologies', to: 'node-myspace' },
    { from: 'node-memory-technologies', to: 'node-facebook' },
    { from: 'node-memory-technologies', to: 'node-twitter' },
    { from: 'node-memory-technologies', to: 'node-instagram' },
    { from: 'node-memory-technologies', to: 'node-tiktok' },
    { from: 'node-memory-technologies', to: 'node-smartphones' },
    { from: 'node-memory-technologies', to: 'node-search-engines' },
    { from: 'node-memory-technologies', to: 'node-ai' },
    
    // Berners-Lee's Web internal
    { from: 'node-berners-lee-web', to: 'node-hypertext' },
    { from: 'node-berners-lee-web', to: 'node-hypermedia' },
    { from: 'node-berners-lee-web', to: 'node-universal-access' },
    { from: 'node-berners-lee-web', to: 'node-future-proofing' },
    { from: 'node-berners-lee-web', to: 'node-global-authorship' },
    
    // Digital Archival Theory internal
    { from: 'node-digital-archival-theory', to: 'node-derrida' },
    { from: 'node-digital-archival-theory', to: 'node-manoff' },
    { from: 'node-digital-archival-theory', to: 'node-ismail' },
    { from: 'node-digital-archival-theory', to: 'node-contemporary-archive-studies' },
    
    // Surveillance internal
    { from: 'node-surveillance', to: 'node-snowden' },
    { from: 'node-surveillance', to: 'node-data-extraction' },
    { from: 'node-surveillance', to: 'node-algorithmic-profiling' },
    { from: 'node-surveillance', to: 'node-platform-governance' },
    { from: 'node-surveillance', to: 'node-tracking' },
    { from: 'node-surveillance', to: 'node-digital-sobriety' },
    
    // Born-Digital Objects internal
    { from: 'node-born-digital-objects', to: 'node-memes' },
    { from: 'node-born-digital-objects', to: 'node-screenshots' },
    { from: 'node-born-digital-objects', to: 'node-status-updates' },
    { from: 'node-born-digital-objects', to: 'node-stories' },
    { from: 'node-born-digital-objects', to: 'node-videos' },
    { from: 'node-born-digital-objects', to: 'node-photo-dumps' },
    { from: 'node-born-digital-objects', to: 'node-comments' },
    
    // Memory Workers internal
    { from: 'node-memory-workers', to: 'node-archivists' },
    { from: 'node-memory-workers', to: 'node-researchers' },
    { from: 'node-memory-workers', to: 'node-writers' },
    { from: 'node-memory-workers', to: 'node-poets' },
    { from: 'node-memory-workers', to: 'node-families' },
    { from: 'node-memory-workers', to: 'node-everyday-users' },
    
    // Cultural Systems internal
    { from: 'node-cultural-systems', to: 'node-going-viral' },
    { from: 'node-cultural-systems', to: 'node-parasocial' },
    { from: 'node-cultural-systems', to: 'node-upgrade-you' },
    { from: 'node-cultural-systems', to: 'node-between-you-and-i' },
    
    // CROSS-CONNECTIONS
    { from: 'node-double-perspective', to: 'node-memory' },
    { from: 'node-double-perspective', to: 'node-the-archive' },
    { from: 'node-double-perspective', to: 'node-the-drivers' },
    { from: 'node-archive-codetermination', to: 'node-distorted-memory' },
    { from: 'node-archive-codetermination', to: 'node-search-engines' },
    { from: 'node-experience-self', to: 'node-personal-memory' },
    { from: 'node-narrator-self', to: 'node-collective-memory' },
    { from: 'node-myspace', to: 'node-personal-memory' },
    { from: 'node-facebook', to: 'node-personal-memory' },
    { from: 'node-derrida', to: 'node-archive-fever' },
    { from: 'node-derrida', to: 'node-traditional-archive' },
    { from: 'node-berners-lee-web', to: 'node-digital-archive' },
    { from: 'node-snowden', to: 'node-surveillance' },
    { from: 'node-memes', to: 'node-collective-memory' },
    { from: 'node-screenshots', to: 'node-personal-memory' },
    { from: 'node-poets', to: 'node-driver-expression' },
    { from: 'node-writers', to: 'node-memory-workers' },
    { from: 'node-ai', to: 'node-surveillance' },
    { from: 'node-smartphones', to: 'node-memory-technologies' },
    { from: 'node-digital-sobriety', to: 'node-memory-technologies' },
    { from: 'node-everyday-users', to: 'node-social-archive-concept' },
    { from: 'node-families', to: 'node-familial-memory' },
    { from: 'node-platform-governance', to: 'node-platforms' },
    { from: 'node-going-viral', to: 'node-memes' },
    { from: 'node-between-you-and-i', to: 'node-personal-memory' },
    { from: 'node-witness-memory', to: 'node-driver-witness' },
    { from: 'node-surveillance', to: 'node-driver-surveillance' },
    { from: 'node-central-thesis', to: 'node-double-perspective' },
    { from: 'node-central-thesis', to: 'node-social-archive-concept' },
    { from: 'node-major-tensions', to: 'node-double-perspective' },
    { from: 'node-major-tensions', to: 'node-surveillance' },
  ];

  // Hide all nodes except center on load
  allNodes.forEach(node => {
    if (node.id !== 'node-millennial-epoch') {
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

  function revealAll() {
    allNodes.forEach(node => {
      node.style.display = 'block';
    });
    drawLines();
  }

  function resetMap() {
    allNodes.forEach(node => {
      if (node.id !== 'node-millennial-epoch') {
        node.style.display = 'none';
      }
    });
    closePreview();
    drawLines();
  }

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

  const previewData = {
    'node-millennial-epoch': {
      title: 'The Millennial Epoch',
      type: 'Center',
      description: 'Not just an age cohort. An epoch is a turn in history — a series of overlapping transformations in technology, politics, economics, and culture that changed the conditions of life for millennials and everyone after.',
      link: '/Trunk/epoch/'
    },
    'node-double-perspective': {
      title: 'Double Perspective',
      type: 'Framework',
      description: 'The interpretive mechanism for the whole project. Experience Self + Narrator Self = Double Perspective. Built from Gornick and Lopate. Applied beyond creative nonfiction into memory work itself.',
      link: '/Trunk/dp/'
    },
    'node-experience-self': { title: 'Experience Self', type: 'Concept', description: 'Lives in the past. Reacts in present time. Has blind spots. Performs objectivity — as close to the facts as you experienced them.', link: null },
    'node-narrator-self': { title: 'Narrator Self', type: 'Concept', description: 'Lives in the present. Organizes chaos. Is self-aware. Performs subjectivity — interprets through a lens. Owes authenticity, not factual evidence.', link: null },
    'node-tension': { title: 'Tension', type: 'Concept', description: 'What happened vs what was recorded. What I remember vs what the archive preserves. Personal meaning vs collective meaning.', link: null },
    'node-archive-codetermination': { title: 'Archive Codetermination', type: 'Concept', description: 'The archive influences memory. Retrieval changes recollection. Search engines privilege certain traces. Platforms determine visibility. Documentation becomes memory.', link: null },
    'node-memory': { title: 'Memory', type: 'Branch', description: 'The raw material of the archive. Personal, collective, distorted, familial. Memory is never singular, never stable, never finished.', link: null },
    'node-personal-memory': { title: 'Personal Memory', type: 'Concept', description: 'What you remember without looking anything up. Camera rolls, screenshots, text messages, voice notes — the unaided recollection of your own life.', link: null },
    'node-collective-memory': { title: 'Collective Memory', type: 'Concept', description: 'The shared memory of a generation. Memes, viral culture, shared internet experiences. What we remember together — or think we do.', link: null },
    'node-distorted-memory': { title: 'Distorted Memory', type: 'Concept', description: 'What happens when the archive codetermines what you remember. False recollection. Search engines shaping recall. The internet telling you what happened.', link: null },
    'node-familial-memory': { title: 'Familial Memory', type: 'Concept', description: 'Email threads, Google Groups, family photos, intergenerational preservation. Who keeps the family archive? Who gets to tell the family story?', link: null },
    'node-witness-memory': { title: 'Witness', type: 'Concept', description: 'Being seen. Recording. Archiving. Testimony. Memory as evidence that something happened.', link: null },
    'node-the-archive': { title: 'The Archive', type: 'Branch', description: 'The institution, the theory, the practice. From the arkheion to the cloud — who stores memory, who interprets it, who decides what survives.', link: '/Trunk/archive/' },
    'node-traditional-archive': { title: 'Traditional Archive', type: 'Concept', description: 'Fixed in time and space. Unique, authentic, secured. The arkheion — residence of the archons, house of authority.', link: null },
    'node-digital-archive': { title: 'Digital Archive', type: 'Concept', description: 'Dynamic, networked, participatory, global. What happens when the archive leaves the building and lives on servers.', link: null },
    'node-social-archive-concept': { title: 'Social Archive', type: 'Concept', description: 'User-generated memory. Metadata as artifact. Platform traces as historical record. Everyday people creating the archive without knowing it.', link: '/Trunk/archive/' },
    'node-archive-fever': { title: 'Archive Fever', type: 'Concept', description: 'Derrida\'s concept. The compulsive need to record, preserve, return to the origin. The death drive versus the pleasure principle.', link: null },
    'node-the-drivers': { title: 'The Drivers', type: 'Collection', description: 'My interviews reveal experiences that cover themes such as place, loss, intimacy, web, identity, expression, future, care, witness, surveillance, emergence, threshold.', link: '/Trunk/drivers/' },
    'node-driver-place': { title: 'Place', type: 'Theme', description: 'Neighborhoods, local identity, belonging, gentrification. "You can\'t google my hood."', link: '/Trunk/drivers/#place' },
    'node-driver-loss': { title: 'Loss', type: 'Theme', description: 'Demolished places, lost records, disappearing communities, vanished internet traces. "How do you phantom limb a street?"', link: '/Trunk/drivers/#loss' },
    'node-driver-intimacy': { title: 'Intimacy', type: 'Theme', description: 'Family, friendship, vulnerability, private memory. The spaces where identity forms.', link: '/Trunk/drivers/#intimacy' },
    'node-driver-web': { title: 'Web', type: 'Theme', description: 'Platforms, searchability, digital mediation, algorithmic memory. Experiences mediated by digital life.', link: '/Trunk/drivers/#web' },
    'node-driver-identity': { title: 'Identity', type: 'Theme', description: 'Culture, race, gender, class, self-construction. The ongoing work of becoming oneself.', link: '/Trunk/drivers/#identity' },
    'node-driver-expression': { title: 'Expression', type: 'Theme', description: 'Poetry, art, memes, creative meaning-making. "I thought poetry was what you went to when you wanted to talk about what you thought god was."', link: '/Trunk/drivers/#expression' },
    'node-driver-future': { title: 'Future', type: 'Theme', description: 'Hope, preservation, community futures, technological futures. What comes next.', link: '/Trunk/drivers/#future' },
    'node-driver-care': { title: 'Care', type: 'Theme', description: 'Mutual support, community, love, responsibility. How we held each other up.', link: '/Trunk/drivers/#care' },
    'node-driver-witness': { title: 'Witness', type: 'Theme', description: 'Observation, documentation, memorialization, testimony. Who saw it and remembered.', link: '/Trunk/drivers/#witness' },
    'node-driver-surveillance': { title: 'Surveillance', type: 'Theme', description: 'Platforms, data collection, visibility, tech power. Who was watching and what visibility cost.', link: '/Trunk/drivers/#surveillance' },
    'node-driver-emergence': { title: 'Emergence', type: 'Theme', description: 'New cultural forms, new technologies, new communities, new identities taking shape.', link: '/Trunk/drivers/#emergence' },
    'node-driver-threshold': { title: 'Threshold', type: 'Theme', description: 'Migration, generational transition, analog to digital, past to future. The worlds we stand between.', link: '/Trunk/drivers/#threshold' },
    'node-memory-technologies': { title: 'Memory Technologies', type: 'Branch', description: 'The tools that shape how we remember. Each technology changes not just what we record but how we recall.', link: null },
    'node-email': { title: 'Email', type: 'Technology', description: 'The archive we don\'t think of as an archive. Family threads, birth announcements — durable personal recordkeeping.', link: null },
    'node-forums': { title: 'Forums', type: 'Technology', description: 'Bulletin boards, Reddit, Discord. Community memory built through conversation.', link: null },
    'node-myspace': { title: 'MySpace', type: 'Platform', description: 'The first social network for millennials. Customizable, chaotic, intimate. Like inviting a friend into your bedroom.', link: null },
    'node-facebook': { title: 'Facebook', type: 'Platform', description: 'A global archive of everyday life — and one of the largest corporations on earth.', link: null },
    'node-twitter': { title: 'Twitter / X', type: 'Platform', description: 'Short-form public discourse. A case study in what happens when one person buys the archive.', link: null },
    'node-instagram': { title: 'Instagram', type: 'Platform', description: 'Photo sharing as curated performance. Everyday life as searchable visual archive.', link: null },
    'node-tiktok': { title: 'TikTok', type: 'Platform', description: 'Algorithmic discovery. The first platform the U.S. government tried to ban outright.', link: null },
    'node-smartphones': { title: 'Smartphones', type: 'Technology', description: 'A computer, camera, microphone, GPS tracker in your hand. Turned everyday life into continuously documented experience.', link: null },
    'node-search-engines': { title: 'Search Engines', type: 'Technology', description: 'The gatekeepers of digital memory. Google\'s algorithm shapes what we find, trust, and forget.', link: null },
    'node-ai': { title: 'AI', type: 'Technology', description: 'Artificial intelligence reshaping authorship, labor, and what it means to create.', link: null },
    'node-berners-lee-web': { title: 'Berners-Lee\'s Web', type: 'Branch', description: 'The vision: a universally linked information system. Hypertext, universal access, free to everyone. The web was never meant to be owned.', link: null },
    'node-hypertext': { title: 'Hypertext', type: 'Concept', description: 'Human-readable information linked in an unconstrained way. The foundation of the web.', link: null },
    'node-hypermedia': { title: 'Hypermedia', type: 'Concept', description: 'The expansion of hypertext to graphics, sound, video. The web as multimedia archive.', link: null },
    'node-universal-access': { title: 'Universal Access', type: 'Concept', description: 'Everyone should be able to read the web. Universal readership as a design principle.', link: null },
    'node-future-proofing': { title: 'Future-Proofing', type: 'Concept', description: 'Information should outlast the systems that created it. Portable, extendible, independent of any one platform.', link: null },
    'node-global-authorship': { title: 'Global Authorship', type: 'Concept', description: 'Everyone should be able to write to the web. A vision of total participation.', link: null },
    'node-digital-archival-theory': { title: 'Digital Archival Theory', type: 'Branch', description: 'The scholars studying what happens when archives go online.', link: '/Trunk/notes/' },
    'node-derrida': { title: 'Derrida', type: 'Researcher', description: 'Wrote Archive Fever. The archive begins as a house of authority. The death drive haunts every act of preservation.', link: null },
    'node-manoff': { title: 'Manoff', type: 'Researcher', description: 'Archives are not neutral. No political power without control of the archive.', link: null },
    'node-ismail': { title: 'Ismail', type: 'Researcher', description: 'Born-digital memes as archival discourse. Virality, mutability, intertextuality.', link: null },
    'node-contemporary-archive-studies': { title: 'Contemporary Studies', type: 'Concept', description: 'Metadata standards, FAIR principles, preservation ethics, ownership disputes, sustainability.', link: null },
    'node-surveillance': { title: 'Surveillance', type: 'Branch', description: 'The other side of the archive. Who\'s watching, what they\'re collecting, what visibility costs.', link: null },
    'node-snowden': { title: 'Snowden', type: 'Event', description: 'Revealed extensive government surveillance. Changed the conversation about privacy and the state.', link: null },
    'node-data-extraction': { title: 'Data Extraction', type: 'Concept', description: 'The business model of the internet. Every click, scroll, pause — harvested, packaged, sold.', link: null },
    'node-algorithmic-profiling': { title: 'Algorithmic Profiling', type: 'Concept', description: 'The version of you built from data. Your algorithmic self.', link: null },
    'node-platform-governance': { title: 'Platform Governance', type: 'Concept', description: 'Who makes the rules? Content moderation, bans, API access. Platforms govern with corporate accountability.', link: null },
    'node-tracking': { title: 'Tracking', type: 'Concept', description: 'Cookies, pixels, fingerprints. The invisible infrastructure that follows you across the web.', link: null },
    'node-digital-sobriety': { title: 'Digital Sobriety', type: 'Concept', description: 'Using technology with more intention, less extraction. The archived web only survived about 30 years.', link: null },
    'node-born-digital-objects': { title: 'Born-Digital Objects', type: 'Branch', description: 'Content created in digital form that was never physical. The raw material of the social archive.', link: null },
    'node-memes': { title: 'Memes', type: 'Object', description: 'Cultural units of transmission. Virality, mutability, intertextuality. Collective memory in image form.', link: null },
    'node-screenshots': { title: 'Screenshots', type: 'Object', description: 'Capturing a moment before it disappears. The primary tool of the lay archivist.', link: null },
    'node-status-updates': { title: 'Status Updates', type: 'Object', description: 'The original social media artifact. Away messages, Facebook statuses, tweets. Broadcasting the self.', link: null },
    'node-stories': { title: 'Stories', type: 'Object', description: 'Ephemeral content that disappears in 24 hours. Memory with an expiration date.', link: null },
    'node-videos': { title: 'Videos', type: 'Object', description: 'YouTube, TikTok, Reels. Video as documentation, entertainment, evidence.', link: null },
    'node-photo-dumps': { title: 'Photo Dumps', type: 'Object', description: 'The anti-curated post. The mess of real life presented as aesthetic.', link: null },
    'node-comments': { title: 'Comments', type: 'Object', description: 'The layer beneath the content. Conversation, argument, community. The archive\'s footnotes.', link: null },
    'node-memory-workers': { title: 'Memory Workers', type: 'Branch', description: 'Anyone who records, preserves, interprets, or transmits memory. The people doing the work of the archive.', link: '/Trunk/drivers/' },
    'node-archivists': { title: 'Archivists', type: 'Role', description: 'The professionals. Trained in preservation, organization, access.', link: null },
    'node-researchers': { title: 'Researchers', type: 'Role', description: 'Academics studying memory, archives, digital culture. Building the theory.', link: null },
    'node-writers': { title: 'Writers', type: 'Role', description: 'Memory workers who use language as their medium. Turning experience into art.', link: '/Drivers/' },
    'node-poets': { title: 'Poets', type: 'Role', description: 'Language at its most compressed and precise. "I thought poetry was what you went to when you wanted to talk about what you thought god was."', link: '/Drivers/' },
    'node-families': { title: 'Families', type: 'Role', description: 'The original memory workers. Who keeps the photos? Who tells the stories?', link: null },
    'node-everyday-users': { title: 'Everyday Users', type: 'Role', description: 'Anyone who posts, shares, screenshots, saves. Creating the archive without knowing it.', link: null },
    'node-cultural-systems': { title: 'Cultural Systems', type: 'Branch', description: 'The patterns that organize how culture moves through the epoch. Virality, parasocial relationships, technological adoption, intimate exchange.', link: null },
    'node-going-viral': { title: 'Going Viral', type: 'System', description: 'Memes, remix culture, intertextuality, emotional shorthand. How culture spreads through networks.', link: '/Trunk/archive/' },
    'node-parasocial': { title: 'Parasocial', type: 'System', description: 'Celebrity intimacy, influencers, personal brands, audience relationships. When strangers feel like friends.', link: '/Trunk/archive/' },
    'node-upgrade-you': { title: 'Upgrade You', type: 'System', description: 'Mobile technology, apps, platform adoption, digital infrastructure. The updates pushed on us whether we asked or not.', link: '/Trunk/archive/' },
    'node-between-you-and-i': { title: 'Between You & I', type: 'System', description: 'Local memory, personal history, family stories, ownership of memory. The intimate moments meant for specific people.', link: '/Trunk/archive/' },
    'node-major-tensions': { title: 'Major Tensions', type: 'Branch', description: 'The oppositions that structure the epoch. Memory vs documentation. Human vs platform. Local vs global. Public vs private. Preservation vs disappearance. Community vs extraction. Authenticity vs performance. Witness vs surveillance. Nostalgia vs futurity.', link: null },
    'node-central-thesis': { title: 'Central Thesis', type: 'Branch', description: 'Millennials experienced a unique transition from analog memory systems to digital ones. Everyday artifacts reveal epoch-scale cultural transformation. Platforms became memory infrastructure. Personal archives are historical archives.', link: null }
  };

  container.addEventListener('click', function(e) {
    if (hasMoved) return;
    const node = e.target.closest('.connection-node');
    if (!node) {
      closePreview();
      return;
    }
    const id = node.id;
    showChildren(id);
    
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
  });

  function closePreview() {
    document.getElementById('node-preview').style.display = 'none';
  }

  positionNodes();
  window.addEventListener('resize', drawLines);
})();
</script>
</div>
</div>

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/ai-reception/">← New developments</a>
  <a href="/Trunk/notes/">Dig thru the glove box →</a>
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