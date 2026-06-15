---
layout: default
title: Connections
permalink: /Trunk/connections/
title: Connections - Hot Wheels & High Heels
---

# Connections

This is a visualization of all the ideas being mapped in the archive. It's a lot messier than I intended it to be but like all pages in the Trunk, it is a work in progress and will be changing as I do more research and add to the archive. You can drag the boxes around, click on them to get a little summary, and if included, a link lets you visit a related page on the site. 

*Move boxes around to explore and click to learn more.*

---

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

  <!-- ============================================
       CENTER NODE
       ============================================ -->
  <div class="connection-node center-node" 
       id="node-memory"
       data-x="420" data-y="280">
    <h3>Memory</h3>
    <span class="node-type">Center</span>
  </div>

  <!-- ============================================
       ARCHIVE SECTIONS — pink, site structure
       ============================================ -->
  <div class="connection-node theme-future" id="node-social-archive" data-x="420" data-y="130">
    <h3>Social Archive</h3>
    <span class="node-type">Collection</span>
  </div>
  <div class="connection-node theme-future" id="node-upgrade-you" data-x="280" data-y="80">
    <h3>Upgrade You</h3>
    <span class="node-type">Archive Section</span>
  </div>
  <div class="connection-node theme-future" id="node-going-viral" data-x="420" data-y="50">
    <h3>Going Viral</h3>
    <span class="node-type">Archive Section</span>
  </div>
  <div class="connection-node theme-future" id="node-the-parasocial" data-x="560" data-y="80">
    <h3>The Parasocial</h3>
    <span class="node-type">Archive Section</span>
  </div>
  <div class="connection-node theme-future" id="node-broken-record" data-x="280" data-y="180">
    <h3>Broken Record</h3>
    <span class="node-type">Archive Section</span>
  </div>
  <div class="connection-node theme-future" id="node-between-you-and-i" data-x="560" data-y="180">
    <h3>Between You &amp; I</h3>
    <span class="node-type">Archive Section</span>
  </div>
  <div class="connection-node theme-future" id="node-ai-reception" data-x="420" data-y="200">
    <h3>AI Reception</h3>
    <span class="node-type">Archive Section</span>
  </div>

  <!-- ============================================
       TIMELINE CATEGORIES — cyan/coral/mint/silver/chartreuse
       ============================================ -->
  <div class="connection-node theme-web" id="node-tech-category" data-x="200" data-y="50">
    <h3>Technology</h3>
    <span class="node-type">Timeline Category</span>
  </div>
  <div class="connection-node theme-loss" id="node-politics-category" data-x="640" data-y="50">
    <h3>Politics</h3>
    <span class="node-type">Timeline Category</span>
  </div>
  <div class="connection-node theme-creativity" id="node-culture-category" data-x="200" data-y="140">
    <h3>Culture</h3>
    <span class="node-type">Timeline Category</span>
  </div>
  <div class="connection-node theme-future" id="node-economics-category" data-x="640" data-y="140">
    <h3>Economics</h3>
    <span class="node-type">Timeline Category</span>
  </div>
  <div class="connection-node theme-place" id="node-local-category" data-x="280" data-y="110">
    <h3>Local Memory</h3>
    <span class="node-type">Timeline Category</span>
  </div>
  <div class="connection-node theme-place" id="node-environment-category" data-x="560" data-y="110">
    <h3>Environment</h3>
    <span class="node-type">Timeline Category</span>
  </div>

  <!-- ============================================
       QUOTE THEMES — chartreuse/coral/gold/cyan/orchid/mint/silver
       ============================================ -->
  <div class="connection-node theme-place" id="node-place-theme" data-x="100" data-y="240">
    <h3>Place</h3>
    <span class="node-type">Quote Theme</span>
  </div>
  <div class="connection-node theme-loss" id="node-loss-theme" data-x="740" data-y="240">
    <h3>Loss</h3>
    <span class="node-type">Quote Theme</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-intimacy-theme" data-x="100" data-y="320">
    <h3>Intimacy</h3>
    <span class="node-type">Quote Theme</span>
  </div>
  <div class="connection-node theme-web" id="node-web-theme" data-x="740" data-y="320">
    <h3>Web</h3>
    <span class="node-type">Quote Theme</span>
  </div>
  <div class="connection-node theme-identity" id="node-identity-theme" data-x="100" data-y="400">
    <h3>Identity</h3>
    <span class="node-type">Quote Theme</span>
  </div>
  <div class="connection-node theme-creativity" id="node-creativity-theme" data-x="740" data-y="400">
    <h3>Creativity</h3>
    <span class="node-type">Quote Theme</span>
  </div>
  <div class="connection-node theme-future" id="node-future-theme" data-x="420" data-y="440">
    <h3>Future</h3>
    <span class="node-type">Quote Theme</span>
  </div>

  <!-- ============================================
       KEY CONCEPTS — purple
       ============================================ -->
  <div class="connection-node theme-identity" id="node-double-perspective" data-x="200" data-y="360">
    <h3>Double Perspective</h3>
    <span class="node-type">Framework</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-nostalgia" data-x="620" data-y="440">
    <h3>Nostalgia</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-forgetting" data-x="700" data-y="460">
    <h3>Forgetting</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-collective-memory" data-x="620" data-y="380">
    <h3>Collective Memory</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-personal-memory" data-x="700" data-y="380">
    <h3>Personal Memory</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-epoch" data-x="660" data-y="340">
    <h3>Millennial Epoch</h3>
    <span class="node-type">Era</span>
  </div>
  <div class="connection-node theme-intimacy" id="node-millennials" data-x="700" data-y="320">
    <h3>Millennials</h3>
    <span class="node-type">Concept</span>
  </div>

  <!-- ============================================
       RESEARCHERS — chartreuse
       ============================================ -->
  <div class="connection-node theme-place" id="node-derrida" data-x="60" data-y="180">
    <h3>Derrida</h3>
    <span class="node-type">Researcher</span>
  </div>
  <div class="connection-node theme-place" id="node-berners-lee" data-x="60" data-y="260">
    <h3>Berners-Lee</h3>
    <span class="node-type">Researcher</span>
  </div>
  <div class="connection-node theme-place" id="node-manoff" data-x="140" data-y="300">
    <h3>Manoff</h3>
    <span class="node-type">Researcher</span>
  </div>
  <div class="connection-node theme-place" id="node-tosic" data-x="100" data-y="460">
    <h3>Tošić</h3>
    <span class="node-type">Researcher</span>
  </div>
  <div class="connection-node theme-place" id="node-ismail" data-x="40" data-y="420">
    <h3>Ismail</h3>
    <span class="node-type">Researcher</span>
  </div>
  <div class="connection-node theme-place" id="node-vlassenroot" data-x="160" data-y="480">
    <h3>Vlassenroot</h3>
    <span class="node-type">Researcher</span>
  </div>

  <!-- ============================================
       CONTRIBUTORS — orchid
       ============================================ -->
  <div class="connection-node theme-identity" id="node-memory-workers" data-x="640" data-y="220">
    <h3>Memory Workers</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-identity" id="node-angela" data-x="720" data-y="60">
    <h3>Angela Mendoza</h3>
    <span class="node-type">Contributor</span>
  </div>
  <div class="connection-node theme-identity" id="node-jon" data-x="760" data-y="120">
    <h3>Jon Tobias</h3>
    <span class="node-type">Contributor</span>
  </div>
  <div class="connection-node theme-identity" id="node-alana" data-x="760" data-y="180">
    <h3>Alana Rodriguez</h3>
    <span class="node-type">Contributor</span>
  </div>
  <div class="connection-node theme-identity" id="node-abenet" data-x="720" data-y="240">
    <h3>a.benét</h3>
    <span class="node-type">Contributor</span>
  </div>
  <div class="connection-node theme-identity" id="node-sam" data-x="760" data-y="300">
    <h3>Sam Yaziji</h3>
    <span class="node-type">Contributor</span>
  </div>
  <div class="connection-node theme-identity" id="node-jack" data-x="720" data-y="360">
    <h3>Jack Hinzo</h3>
    <span class="node-type">Contributor</span>
  </div>

  <!-- ============================================
       PLATFORMS — cyan
       ============================================ -->
  <div class="connection-node theme-web" id="node-platforms" data-x="300" data-y="280">
    <h3>Platforms</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-web" id="node-myspace" data-x="220" data-y="320">
    <h3>MySpace</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-facebook" data-x="300" data-y="360">
    <h3>Facebook</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-twitter" data-x="380" data-y="340">
    <h3>Twitter / X</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-tumblr" data-x="260" data-y="400">
    <h3>Tumblr</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-instagram" data-x="340" data-y="420">
    <h3>Instagram</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-tiktok" data-x="420" data-y="400">
    <h3>TikTok</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-youtube" data-x="380" data-y="460">
    <h3>YouTube</h3>
    <span class="node-type">Platform</span>
  </div>
  <div class="connection-node theme-web" id="node-email" data-x="300" data-y="480">
    <h3>Email</h3>
    <span class="node-type">Platform</span>
  </div>

  <!-- ============================================
       CONCEPTS — various
       ============================================ -->
  <div class="connection-node theme-loss" id="node-memes" data-x="40" data-y="340">
    <h3>Memes</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-loss" id="node-virality" data-x="100" data-y="300">
    <h3>Virality</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-loss" id="node-participation" data-x="40" data-y="380">
    <h3>Participation</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-loss" id="node-remix" data-x="120" data-y="360">
    <h3>Remix Culture</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-surveillance" data-x="500" data-y="420">
    <h3>Surveillance</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-algorithms" data-x="560" data-y="400">
    <h3>Algorithms</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-corporations" data-x="600" data-y="440">
    <h3>Corporations</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-censorship" data-x="660" data-y="420">
    <h3>Censorship</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-digital-sobriety" data-x="560" data-y="480">
    <h3>Digital Sobriety</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-web" id="node-smartphones" data-x="480" data-y="460">
    <h3>Smartphones</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-loss" id="node-platform-death" data-x="220" data-y="440">
    <h3>Platform Death</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-creativity" id="node-fandom" data-x="80" data-y="480">
    <h3>Fandom</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-web" id="node-aesthetics" data-x="160" data-y="420">
    <h3>Internet Aesthetics</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-identity" id="node-algorithmic-self" data-x="580" data-y="340">
    <h3>Algorithmic Self</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-place" id="node-place-memory" data-x="160" data-y="520">
    <h3>Place Memory</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-datafication" data-x="520" data-y="520">
    <h3>Datafication</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-web" id="node-cloud" data-x="600" data-y="500">
    <h3>Cloud</h3>
    <span class="node-type">Concept</span>
  </div>
  <div class="connection-node theme-future" id="node-ai" data-x="460" data-y="520">
    <h3>AI</h3>
    <span class="node-type">Concept</span>
  </div>

  <!-- ============================================
       SITE PAGES — pink
       ============================================ -->
  <div class="connection-node theme-future" id="node-the-trunk" data-x="420" data-y="380">
    <h3>The Trunk</h3>
    <span class="node-type">Archive</span>
  </div>
  <div class="connection-node theme-future" id="node-blessings" data-x="340" data-y="240">
    <h3>Blessings</h3>
    <span class="node-type">Page</span>
  </div>
  <div class="connection-node theme-future" id="node-index" data-x="500" data-y="240">
    <h3>Index</h3>
    <span class="node-type">Collection</span>
  </div>

<script>
(function() {
  const container = document.getElementById('connections-map');
  const svg = document.getElementById('connections-svg');
  const nodes = container.querySelectorAll('.connection-node');

  const connections = [
    // Center to everything
    { from: 'node-memory', to: 'node-social-archive' },
    { from: 'node-memory', to: 'node-the-trunk' },
    { from: 'node-memory', to: 'node-double-perspective' },
    { from: 'node-memory', to: 'node-personal-memory' },
    { from: 'node-memory', to: 'node-collective-memory' },
    { from: 'node-memory', to: 'node-epoch' },
    { from: 'node-memory', to: 'node-millennials' },
    { from: 'node-memory', to: 'node-forgetting' },
    { from: 'node-memory', to: 'node-nostalgia' },
    { from: 'node-memory', to: 'node-place-memory' },
    { from: 'node-memory', to: 'node-memory-workers' },

    // Archive sections to timeline categories
    { from: 'node-upgrade-you', to: 'node-tech-category' },
    { from: 'node-going-viral', to: 'node-culture-category' },
    { from: 'node-going-viral', to: 'node-tech-category' },
    { from: 'node-the-parasocial', to: 'node-culture-category' },
    { from: 'node-the-parasocial', to: 'node-politics-category' },
    { from: 'node-broken-record', to: 'node-culture-category' },
    { from: 'node-broken-record', to: 'node-economics-category' },
    { from: 'node-between-you-and-i', to: 'node-local-category' },
    { from: 'node-between-you-and-i', to: 'node-culture-category' },
    { from: 'node-ai-reception', to: 'node-tech-category' },
    { from: 'node-ai-reception', to: 'node-culture-category' },

    // Archive sections to quote themes
    { from: 'node-upgrade-you', to: 'node-web-theme' },
    { from: 'node-upgrade-you', to: 'node-identity-theme' },
    { from: 'node-going-viral', to: 'node-web-theme' },
    { from: 'node-going-viral', to: 'node-creativity-theme' },
    { from: 'node-going-viral', to: 'node-intimacy-theme' },
    { from: 'node-the-parasocial', to: 'node-identity-theme' },
    { from: 'node-the-parasocial', to: 'node-intimacy-theme' },
    { from: 'node-broken-record', to: 'node-future-theme' },
    { from: 'node-broken-record', to: 'node-loss-theme' },
    { from: 'node-between-you-and-i', to: 'node-place-theme' },
    { from: 'node-between-you-and-i', to: 'node-loss-theme' },
    { from: 'node-between-you-and-i', to: 'node-intimacy-theme' },
    { from: 'node-ai-reception', to: 'node-future-theme' },
    { from: 'node-ai-reception', to: 'node-creativity-theme' },

    // Archive sections to concepts
    { from: 'node-upgrade-you', to: 'node-smartphones' },
    { from: 'node-upgrade-you', to: 'node-platforms' },
    { from: 'node-going-viral', to: 'node-memes' },
    { from: 'node-going-viral', to: 'node-virality' },
    { from: 'node-going-viral', to: 'node-participation' },
    { from: 'node-going-viral', to: 'node-remix' },
    { from: 'node-the-parasocial', to: 'node-platforms' },
    { from: 'node-the-parasocial', to: 'node-instagram' },
    { from: 'node-broken-record', to: 'node-nostalgia' },
    { from: 'node-between-you-and-i', to: 'node-place-memory' },
    { from: 'node-between-you-and-i', to: 'node-local-category' },
    { from: 'node-ai-reception', to: 'node-ai' },
    { from: 'node-ai-reception', to: 'node-censorship' },

    // Social Archive to its sections
    { from: 'node-social-archive', to: 'node-upgrade-you' },
    { from: 'node-social-archive', to: 'node-going-viral' },
    { from: 'node-social-archive', to: 'node-the-parasocial' },
    { from: 'node-social-archive', to: 'node-broken-record' },
    { from: 'node-social-archive', to: 'node-between-you-and-i' },
    { from: 'node-social-archive', to: 'node-ai-reception' },

    // The Trunk to its collections
    { from: 'node-the-trunk', to: 'node-social-archive' },
    { from: 'node-the-trunk', to: 'node-epoch' },
    { from: 'node-the-trunk', to: 'node-blessings' },
    { from: 'node-the-trunk', to: 'node-index' },
    { from: 'node-the-trunk', to: 'node-memory-workers' },

    // Platforms to each other and concepts
    { from: 'node-platforms', to: 'node-myspace' },
    { from: 'node-platforms', to: 'node-facebook' },
    { from: 'node-platforms', to: 'node-twitter' },
    { from: 'node-platforms', to: 'node-tumblr' },
    { from: 'node-platforms', to: 'node-instagram' },
    { from: 'node-platforms', to: 'node-tiktok' },
    { from: 'node-platforms', to: 'node-youtube' },
    { from: 'node-platforms', to: 'node-email' },
    { from: 'node-platforms', to: 'node-corporations' },
    { from: 'node-platforms', to: 'node-algorithms' },
    { from: 'node-myspace', to: 'node-nostalgia' },
    { from: 'node-myspace', to: 'node-platform-death' },
    { from: 'node-tumblr', to: 'node-fandom' },
    { from: 'node-tumblr', to: 'node-aesthetics' },
    { from: 'node-tumblr', to: 'node-platform-death' },
    { from: 'node-instagram', to: 'node-aesthetics' },
    { from: 'node-instagram', to: 'node-algorithmic-self' },
    { from: 'node-tiktok', to: 'node-algorithms' },
    { from: 'node-tiktok', to: 'node-algorithmic-self' },
    { from: 'node-facebook', to: 'node-corporations' },
    { from: 'node-twitter', to: 'node-censorship' },

    // Contributors
    { from: 'node-memory-workers', to: 'node-angela' },
    { from: 'node-memory-workers', to: 'node-jon' },
    { from: 'node-memory-workers', to: 'node-alana' },
    { from: 'node-memory-workers', to: 'node-abenet' },
    { from: 'node-memory-workers', to: 'node-sam' },
    { from: 'node-memory-workers', to: 'node-jack' },
    { from: 'node-angela', to: 'node-place-theme' },
    { from: 'node-angela', to: 'node-identity-theme' },
    { from: 'node-angela', to: 'node-loss-theme' },
    { from: 'node-jon', to: 'node-place-theme' },
    { from: 'node-jon', to: 'node-loss-theme' },
    { from: 'node-jon', to: 'node-creativity-theme' },
    { from: 'node-jon', to: 'node-web-theme' },
    { from: 'node-alana', to: 'node-place-theme' },
    { from: 'node-alana', to: 'node-web-theme' },
    { from: 'node-alana', to: 'node-intimacy-theme' },
    { from: 'node-abenet', to: 'node-place-theme' },
    { from: 'node-abenet', to: 'node-identity-theme' },
    { from: 'node-abenet', to: 'node-loss-theme' },
    { from: 'node-sam', to: 'node-identity-theme' },
    { from: 'node-sam', to: 'node-creativity-theme' },
    { from: 'node-sam', to: 'node-web-theme' },
    { from: 'node-jack', to: 'node-place-theme' },
    { from: 'node-jack', to: 'node-web-theme' },

    // Concepts to each other
    { from: 'node-memes', to: 'node-virality' },
    { from: 'node-memes', to: 'node-participation' },
    { from: 'node-memes', to: 'node-remix' },
    { from: 'node-memes', to: 'node-collective-memory' },
    { from: 'node-virality', to: 'node-platforms' },
    { from: 'node-participation', to: 'node-memory-workers' },
    { from: 'node-remix', to: 'node-creativity-theme' },
    { from: 'node-surveillance', to: 'node-corporations' },
    { from: 'node-surveillance', to: 'node-datafication' },
    { from: 'node-surveillance', to: 'node-politics-category' },
    { from: 'node-algorithms', to: 'node-platforms' },
    { from: 'node-algorithms', to: 'node-attention' },
    { from: 'node-corporations', to: 'node-platforms' },
    { from: 'node-corporations', to: 'node-economics-category' },
    { from: 'node-censorship', to: 'node-politics-category' },
    { from: 'node-platform-death', to: 'node-loss-theme' },
    { from: 'node-platform-death', to: 'node-forgetting' },
    { from: 'node-digital-sobriety', to: 'node-surveillance' },
    { from: 'node-digital-sobriety', to: 'node-datafication' },
    { from: 'node-datafication', to: 'node-cloud' },
    { from: 'node-datafication', to: 'node-algorithms' },
    { from: 'node-cloud', to: 'node-smartphones' },
    { from: 'node-ai', to: 'node-platforms' },
    { from: 'node-ai', to: 'node-censorship' },
    { from: 'node-ai', to: 'node-creativity-theme' },
    { from: 'node-ai', to: 'node-future-theme' },
    { from: 'node-nostalgia', to: 'node-culture-category' },
    { from: 'node-nostalgia', to: 'node-forgetting' },
    { from: 'node-forgetting', to: 'node-loss-theme' },
    { from: 'node-collective-memory', to: 'node-epoch' },
    { from: 'node-collective-memory', to: 'node-millennials' },
    { from: 'node-personal-memory', to: 'node-double-perspective' },
    { from: 'node-double-perspective', to: 'node-memory' },
    { from: 'node-epoch', to: 'node-millennials' },
    { from: 'node-millennials', to: 'node-nostalgia' },
    { from: 'node-place-memory', to: 'node-place-theme' },
    { from: 'node-place-memory', to: 'node-local-category' },
    { from: 'node-fandom', to: 'node-participation' },
    { from: 'node-fandom', to: 'node-identity-theme' },
    { from: 'node-aesthetics', to: 'node-culture-category' },
    { from: 'node-algorithmic-self', to: 'node-identity-theme' },

    // Researchers
    { from: 'node-derrida', to: 'node-forgetting' },
    { from: 'node-derrida', to: 'node-nostalgia' },
    { from: 'node-berners-lee', to: 'node-platforms' },
    { from: 'node-berners-lee', to: 'node-web-theme' },
    { from: 'node-manoff', to: 'node-censorship' },
    { from: 'node-tosic', to: 'node-social-archive' },
    { from: 'node-tosic', to: 'node-memory-workers' },
    { from: 'node-ismail', to: 'node-memes' },
    { from: 'node-ismail', to: 'node-participation' },
    { from: 'node-vlassenroot', to: 'node-platforms' },

    // Environment connections
    { from: 'node-environment-category', to: 'node-local-category' },
    { from: 'node-environment-category', to: 'node-politics-category' },
    { from: 'node-environment-category', to: 'node-future-theme' },

    // Blessings
    { from: 'node-blessings', to: 'node-memory-workers' },
    { from: 'node-blessings', to: 'node-intimacy-theme' },
    { from: 'node-blessings', to: 'node-identity-theme' },

    // Index
    { from: 'node-index', to: 'node-the-trunk' },
  ];

  function positionNodes() {
    nodes.forEach(node => {
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
  // Center
  'node-memory': {
    title: 'Memory',
    type: 'Center',
    description: 'The central concept of the archive. Everything orbits around how memory is created, preserved, distorted, and transmitted.',
    link: null
  },

  // Archive Sections
  'node-social-archive': {
    title: 'The Social Archive',
    type: 'Collection',
    description: 'Screenshots, posts, photographs, and digital debris — evidence of how people recorded their lives online during the millennial epoch.',
    link: '/Trunk/archive/'
  },
  'node-upgrade-you': {
    title: 'Upgrade You',
    type: 'Archive Section',
    description: 'Screenshots of new features, updates, and the moments technology changed how we communicate without asking first.',
    link: '/Trunk/archive/'
  },
  'node-going-viral': {
    title: 'Going Viral',
    type: 'Archive Section',
    description: 'Memes, remixes, and the stuff we all passed around until it became part of how we talk.',
    link: '/Trunk/archive/'
  },
  'node-the-parasocial': {
    title: 'The Parasocial',
    type: 'Archive Section',
    description: 'When celebrities started feeling like friends and presidents started tweeting like exes.',
    link: '/Trunk/archive/'
  },
  'node-broken-record': {
    title: 'Broken Record',
    type: 'Archive Section',
    description: 'The sequels, the reboots, the comfort watches we return to like a favorite song.',
    link: '/Trunk/archive/'
  },
  'node-between-you-and-i': {
    title: 'Between You & I',
    type: 'Archive Section',
    description: 'Conversations meant for one person. Local references. The stuff that wasn\'t supposed to be for everyone.',
    link: '/Trunk/archive/'
  },
  'node-ai-reception': {
    title: 'AI Reception',
    type: 'Archive Section',
    description: 'Watching the literary world figure out how it feels about artificial intelligence, one submission guideline at a time.',
    link: '/Trunk/archive/'
  },

  // Timeline Categories
  'node-tech-category': {
    title: 'Technology',
    type: 'Timeline Category',
    description: 'The tools that shaped the epoch — from the Commodore 64 to ChatGPT. Technology doesn\'t just record experience, it changes what we remember and how.',
    link: '/Trunk/epoch/'
  },
  'node-politics-category': {
    title: 'Politics',
    type: 'Timeline Category',
    description: 'The laws, elections, conflicts, and policies that shaped the conditions millennials came of age under.',
    link: '/Trunk/epoch/'
  },
  'node-culture-category': {
    title: 'Culture',
    type: 'Timeline Category',
    description: 'The shared symbols, stories, and moments that connect people across the epoch.',
    link: '/Trunk/epoch/'
  },
  'node-economics-category': {
    title: 'Economics',
    type: 'Timeline Category',
    description: 'The crashes, the debt, the gig economy — economic precarity as a defining generational condition.',
    link: '/Trunk/epoch/'
  },
  'node-local-category': {
    title: 'Local Memory',
    type: 'Timeline Category',
    description: 'The neighborhoods, landmarks, and communities that hold memory at the street level.',
    link: '/Trunk/epoch/'
  },
  'node-environment-category': {
    title: 'Environment',
    type: 'Timeline Category',
    description: 'Climate strikes, disasters, data centers, extinction — the physical world reacting to the epoch.',
    link: '/Trunk/epoch/'
  },

  // Quote Themes
  'node-place-theme': {
    title: 'Place',
    type: 'Quote Theme',
    description: '"You can\'t google my hood." The locations where memory takes root.',
    link: '/Trunk/drivers/#place'
  },
  'node-loss-theme': {
    title: 'Loss',
    type: 'Quote Theme',
    description: '"How do you phantom limb a street?" Things that disappeared — buildings, people, neighborhoods, versions of self.',
    link: '/Trunk/drivers/#loss'
  },
  'node-intimacy-theme': {
    title: 'Intimacy',
    type: 'Quote Theme',
    description: '"I stepped on Zac Efron and Vanessa Hudgens every day until their faces became indiscernible." Friendship, family, vulnerability.',
    link: '/Trunk/drivers/#intimacy'
  },
  'node-web-theme': {
    title: 'Web',
    type: 'Quote Theme',
    description: '"I can\'t even find a picture of them on Google to prove they were real." Experiences mediated, preserved, distorted, or erased by digital life.',
    link: '/Trunk/drivers/#web'
  },
  'node-identity-theme': {
    title: 'Identity',
    type: 'Quote Theme',
    description: '"I grew up to love ghetto." Race, gender, culture, faith, and the ongoing work of becoming oneself.',
    link: '/Trunk/drivers/#identity'
  },
  'node-creativity-theme': {
    title: 'Creativity',
    type: 'Quote Theme',
    description: '"I thought poetry was what you went to when you wanted to talk about what you thought god was." Art, poetry, music, and the drive to make meaning.',
    link: '/Trunk/drivers/#creativity'
  },
  'node-future-theme': {
    title: 'Future',
    type: 'Quote Theme',
    description: '"San Diego of the future, my hope is that you still hold space for community." What comes next — transition, technology, hope, and the unknown.',
    link: '/Trunk/drivers/#future'
  },

  // Key Concepts
  'node-double-perspective': {
    title: 'Double Perspective',
    type: 'Framework',
    description: 'The experience self and the narrator self. Memory requires both — the one who lived it and the one who looks back. Neither controls the other.',
    link: '/Trunk/notes/'
  },
  'node-nostalgia': {
    title: 'Nostalgia',
    type: 'Concept',
    description: 'A longing for the past that shapes how people remember, interpret, and preserve experience. Monetized, weaponized, and genuinely felt.',
    link: null
  },
  'node-forgetting': {
    title: 'Forgetting',
    type: 'Concept',
    description: 'Derrida called it the death drive — the violence of forgetting that haunts every archive. Forgetting is as important to memory as remembering.',
    link: null
  },
  'node-collective-memory': {
    title: 'Collective Memory',
    type: 'Concept',
    description: 'The shared memory of a group, community, or generation. What we remember together shapes cultural identity.',
    link: null
  },
  'node-personal-memory': {
    title: 'Personal Memory',
    type: 'Concept',
    description: 'The recollection of individual experience. The raw material that storytelling, testimony, and memoir are built from.',
    link: null
  },
  'node-epoch': {
    title: 'Millennial Epoch',
    type: 'Era',
    description: 'The period from 1982 to the present — the events, technologies, and conditions that shaped millennials and those following.',
    link: '/Trunk/epoch/'
  },
  'node-millennials': {
    title: 'Millennials',
    type: 'Concept',
    description: 'The generation born during the transition from analog to digital life. Named after the turn of the millennium.',
    link: null
  },

  // Researchers
  'node-derrida': {
    title: 'Derrida',
    type: 'Researcher',
    description: 'Wrote Archive Fever, a Russian doll of a thesis about memory, authority, and the death drive. Reading his book exhaustively is the only way to truly consume it.',
    link: null
  },
  'node-berners-lee': {
    title: 'Berners-Lee',
    type: 'Researcher',
    description: 'Proposed the World Wide Web at CERN in 1989. His vision was a universal linked information system — an archive for everyone.',
    link: null
  },
  'node-manoff': {
    title: 'Manoff',
    type: 'Researcher',
    description: 'Wrote about archives and democracy — no political power without control of the archive. Archives are not neutral.',
    link: null
  },
  'node-tosic': {
    title: 'Tošić',
    type: 'Researcher',
    description: 'Introduced parallel truths — the idea that subjective archiving can lead to objective research results. Social media users as curators of history.',
    link: null
  },
  'node-ismail': {
    title: 'Ismail',
    type: 'Researcher',
    description: 'Studied born-digital memes as archival discourse. Memes are cultural units of transmission — dynamic, interactive, participatory.',
    link: null
  },
  'node-vlassenroot': {
    title: 'Vlassenroot',
    type: 'Researcher',
    description: 'Researched web archiving and social media — what counts as born-digital heritage and how we preserve it.',
    link: null
  },

  // Contributors
  'node-memory-workers': {
    title: 'Memory Workers',
    type: 'Concept',
    description: 'Anyone who records, preserves, interprets, or transmits memory. Not just archivists — social media users, writers, family members.',
    link: '/Trunk/drivers/'
  },
  'node-angela': {
    title: 'Angela Mendoza',
    type: 'Contributor',
    description: 'Chicana writer from Roseland. "You can\'t google my hood." Her testimony documents immigrant communities, displacement, and the meaning of home.',
    link: '/Drivers/Angela/'
  },
  'node-jon': {
    title: 'Jon Tobias',
    type: 'Contributor',
    description: 'Poet from El Cajon. "How do you phantom limb a street?" His work explores memory, vulnerability, and the ghosts of places that disappear.',
    link: '/Drivers/Jon/'
  },
  'node-alana': {
    title: 'Alana Rodriguez',
    type: 'Contributor',
    description: 'Poet from Chula Vista. "I can\'t even find a picture of them on Google to prove they were real." Her work documents girlhood, loss, and the irreplaceable.',
    link: '/Drivers/Alana/'
  },
  'node-abenet': {
    title: 'a.benét',
    type: 'Contributor',
    description: 'Black poet from City Heights. "Boundaries don\'t exist." Her work maps identity, community, and the streets that raised her.',
    link: '/Drivers/abenet/'
  },
  'node-sam': {
    title: 'Sam Yaziji',
    type: 'Contributor',
    description: 'Poet and musician from Miami. "I\'ve always been a lay archivist." His work bridges faith, philosophy, and the digital age.',
    link: '/Drivers/Sam/'
  },
  'node-jack': {
    title: 'Jack Hinzo',
    type: 'Contributor',
    description: 'Photographer from San Diego. "You can\'t redo a Polaroid." His work captures the melancholy underneath the sunshine.',
    link: '/Drivers/Jack/'
  },

  // Platforms
  'node-platforms': {
    title: 'Platforms',
    type: 'Concept',
    description: 'The digital spaces where contemporary memory is created, shared, and sometimes lost. Platforms organize participation — and ownership.',
    link: null
  },
  'node-myspace': {
    title: 'MySpace',
    type: 'Platform',
    description: 'The first social network to reach global usership among millennials. Customizable, chaotic, intimate — like inviting a friend into your bedroom.',
    link: null
  },
  'node-facebook': {
    title: 'Facebook',
    type: 'Platform',
    description: 'Built around personal profiles and social connections. Became a major archive of everyday life — and one of the largest corporations on earth.',
    link: null
  },
  'node-twitter': {
    title: 'Twitter / X',
    type: 'Platform',
    description: 'Short-form public communication. A record of reactions, events, and public discourse — and a case study in what happens when one person buys the archive.',
    link: null
  },
  'node-tumblr': {
    title: 'Tumblr',
    type: 'Platform',
    description: 'The engine of internet aesthetics, fandom, and GIF culture. The adult content ban destroyed community archives overnight.',
    link: null
  },
  'node-instagram': {
    title: 'Instagram',
    type: 'Platform',
    description: 'Photo sharing as social communication. The platform that turned everyday life into curated performance.',
    link: null
  },
  'node-tiktok': {
    title: 'TikTok',
    type: 'Platform',
    description: 'Short-form video driven by algorithmic discovery. The first platform the U.S. government tried to ban outright.',
    link: null
  },
  'node-youtube': {
    title: 'YouTube',
    type: 'Platform',
    description: 'A video-sharing platform that serves as both entertainment network and public archive. Gangnam Style, the first billion-view video.',
    link: null
  },
  'node-email': {
    title: 'Email',
    type: 'Platform',
    description: 'One of the most durable forms of personal recordkeeping. Family threads, birth announcements, the archive we don\'t think of as an archive.',
    link: null
  },

  // Concepts
  'node-memes': {
    title: 'Memes',
    type: 'Concept',
    description: 'Images, phrases, and cultural references that spread through imitation and adaptation. Ismail calls them units of collective cultural memory.',
    link: null
  },
  'node-virality': {
    title: 'Virality',
    type: 'Concept',
    description: 'The rapid spread of content through networks. Speed and reach increase archival value — the more people see it, the more it matters.',
    link: null
  },
  'node-participation': {
    title: 'Participation',
    type: 'Concept',
    description: 'The act of contributing to shared cultural spaces. Audiences become creators, curators, and archivists.',
    link: null
  },
  'node-remix': {
    title: 'Remix Culture',
    type: 'Concept',
    description: 'The practice of adapting, combining, and reusing cultural materials. Creativity as an ongoing conversation rather than a singular act.',
    link: null
  },
  'node-surveillance': {
    title: 'Surveillance',
    type: 'Concept',
    description: 'The collection and monitoring of personal data. Snowden revealed the scale. Our phones confirmed it. The archive is also a surveillance state.',
    link: null
  },
  'node-algorithms': {
    title: 'Algorithms',
    type: 'Concept',
    description: 'The rules that sort, recommend, and prioritize what we see. Algorithms shape visibility, attention, and ultimately memory.',
    link: null
  },
  'node-corporations': {
    title: 'Corporations',
    type: 'Concept',
    description: 'The companies that own the platforms where digital memory is stored. Their decisions shape access, visibility, and preservation.',
    link: null
  },
  'node-censorship': {
    title: 'Censorship',
    type: 'Concept',
    description: 'The restriction, removal, or suppression of information. What gets deleted from the archive and why.',
    link: null
  },
  'node-digital-sobriety': {
    title: 'Digital Sobriety',
    type: 'Concept',
    description: 'A renewed contemplation on how to develop digital productions — using technology with more intention and less extraction.',
    link: null
  },
  'node-smartphones': {
    title: 'Smartphones',
    type: 'Concept',
    description: 'A computer in your hand. Turned everyday life into a continuously documented experience.',
    link: null
  },
  'node-platform-death': {
    title: 'Platform Death',
    type: 'Concept',
    description: 'What happens when a platform shuts down. MySpace, Vine, Tumblr\'s communities — years of culture and memory gone.',
    link: null
  },
  'node-fandom': {
    title: 'Fandom',
    type: 'Concept',
    description: 'Communities formed around shared cultural obsessions. Fandoms generate their own archives, traditions, and collective memory.',
    link: null
  },
  'node-aesthetics': {
    title: 'Internet Aesthetics',
    type: 'Concept',
    description: 'The visual styles and creative conventions that emerge online. Each era of the internet has its own look.',
    link: null
  },
  'node-algorithmic-self': {
    title: 'Algorithmic Self',
    type: 'Concept',
    description: 'The version of a person represented through data, profiles, and platform activity. Shaped by both user behavior and the systems that track it.',
    link: null
  },
  'node-place-memory': {
    title: 'Place Memory',
    type: 'Concept',
    description: 'Memory connected to specific locations. Places hold experiences long after the events that created them have passed.',
    link: null
  },
  'node-datafication': {
    title: 'Datafication',
    type: 'Concept',
    description: 'The process of converting human activity into measurable data. Experience becomes information that can be stored, analyzed, and sold.',
    link: null
  },
  'node-cloud': {
    title: 'Cloud',
    type: 'Concept',
    description: 'Remote storage that allows memory to persist beyond individual devices. Convenient, invisible, owned by corporations.',
    link: null
  },
  'node-ai': {
    title: 'AI',
    type: 'Concept',
    description: 'Artificial intelligence — the latest technology reshaping authorship, labor, and what it means to create. The epoch\'s newest turning point.',
    link: null
  },

  // Site Pages
  'node-the-trunk': {
    title: 'The Trunk',
    type: 'Archive',
    description: 'The research core of the project. Timeline, Social Archive, Field Notes, Connections — the question of what happens when memory, history, and platforms converge.',
    link: '/Trunk/'
  },
  'node-blessings': {
    title: 'Blessings',
    type: 'Page',
    description: 'A memorial and a reminder of the people whose work left an impression. Look what we made.',
    link: '/blessings/'
  },
  'node-index': {
    title: 'Index',
    type: 'Collection',
    description: 'Key terms, researchers, and concepts from across the archive. A quick reference for the ideas that shape the Trunk.',
    link: null
  }
};

// Show preview near the clicked node
container.addEventListener('click', function(e) {
  if (hasMoved) return;
  const node = e.target.closest('.connection-node');
  if (!node) {
    closePreview();
    return;
  }
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

  // Position popup near the clicked node
  const nodeRect = node.getBoundingClientRect();
  const containerRect = container.getBoundingClientRect();
  const previewWidth = 300;
  const previewHeight = 200;

  let left = nodeRect.left - containerRect.left + nodeRect.width + 16;
  let top = nodeRect.top - containerRect.top;

  // Keep popup within container bounds
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

// Close preview
function closePreview() {
  document.getElementById('node-preview').style.display = 'none';
}

  positionNodes();
  window.addEventListener('resize', drawLines);
})();
</script>
</div>

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/notes/">← Dig thru the glove box</a>
  <a href="/Trunk/">Back to Trunk →</a>
</div>