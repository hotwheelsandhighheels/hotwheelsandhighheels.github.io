---
layout: default
title: Blessings
permalink: /blessings/
sitemap: false
---

<div class="survey-container">

  <h1>Look What We Made</h1>
  <blockquote class="pull-quote">And I have presented it to you as a memorial and as a reminder [a memorial and a reminder, the one and the other at once, the one in the other, and we have, perhaps, in the economy of these two words the whole of archival law]</blockquote><p>from Derrida's <i>Archive Fever</i>, pg. 23</p>

  <hr>

  <h2>Blessings</h2>
  <p>If you know someone whose creative work is <em>epoch-making</em>, tell me about them. These are your teachers, cousins, peers & friends, someone who posted online, a community voice or a neighbor. (Find my entry below as a sample while I work on this page.)</p>

  <form action="https://formspree.io/f/xpqeggbv" method="POST" class="submit-form">

    <label for="nominee-name">Who do you want to include? <span class="form-required">*</span></label>
    <input type="text" id="nominee-name" name="nominee-name" required>

    <label for="epoch">What about them or their work is epoch-making? <span class="form-required">*</span></label>
    <p class="form-hint">What did they make, build, write, or create that captures something true about life in this millennium? This could be a specific project or their entire body of work.</p>
    <textarea id="epoch" name="epoch" rows="5" required></textarea>

    <label for="connection">How can I connect with them and/or their work? <span class="form-required">*</span></label>
    <p class="form-hint">Website, social media, portfolio, article, or any other way to find them and what they've made.</p>
    <textarea id="connection" name="connection" rows="3" required></textarea>

    <label class="form-checkbox">
      <input type="checkbox" name="driver-consideration" value="yes">
      I think this person should also be considered for a Driver feature (full interview).
    </label>

    <input type="text" name="_gotcha" style="display:none">

    <button type="submit" class="submit-btn">Submit ♡</button>

  </form>

  <p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">entries go directly to alejandra@hotwheelsandhighheels.com</p>

  <hr>
  <!-- ============================================
       ALE — EXAMPLE ENTRY
       ============================================ -->

  <div class="blessing-card">
    <div class="blessing-image">
      <img src="/assets/blessings/hwhh.png" alt="Hot Wheels & High Heels banner" onclick="openBlessingLightbox('/assets/blessings/hwhh.png')" style="cursor: url('/assets/svg/cursor.svg') 8 2, auto;">
    </div>
    <div class="blessing-text">
      <h2>Alejandra Hernández</h2>
      <p class="blessing-project"><a href="https://hotwheelsandhighheels.com">Hot Wheels & High Heels</a></p>
      <p>Memory worker. Poet. Building an archive of the millennial epoch from what started out as love poems to a generation.</p>
      <p class="blessing-note">If I can archive myself, I can ask others to let me archive them too.</p>
    </div>
  </div>

  <!-- ============================================
       ADD MORE BLESSING CARDS BELOW
       Copy the block above and replace the content
       ============================================ -->

  <!--
  <div class="blessing-card">
    <div class="blessing-image">
      <img src="/assets/blessings/FILENAME.png" alt="DESCRIPTION">
    </div>
    <div class="blessing-text">
      <h2>NAME</h2>
      <p class="blessing-project"><a href="URL">PROJECT NAME</a></p>
      <p>ONE-LINE DESCRIPTION OF WHO THEY ARE AND WHAT THEY MADE.</p>
      <p class="blessing-note">WHY YOU WANT TO REMEMBER THEM.</p>
    </div>
  </div>
  -->

<!-- LIGHTBOX -->
<div class="lightbox" id="blessing-lightbox" onclick="closeBlessingLightbox()">
  <span class="lightbox-close">close</span>
  <img src="" alt="Site preview" id="blessing-lightbox-img">
</div>

<div class="driver-nav">
  <a href="/Trunk/">← Back to Trunk</a>
  <a href="/submit/">Other submissions →</a>
</div>