---
layout: post
title: First Last
description: An interview with First Last, one sentence about who they are and what they do.
published: false
---

<!-- ============================================
     HOT WHEELS & HIGH HEELS — CONTRIBUTOR TEMPLATE
     
     Copy this file, rename it to the contributor's first name (e.g. Jon.md)
     and save it in the /Drivers/ folder.
     
     Replace everything in ALL CAPS with real content.
     Delete any sections that don't apply (poem section if no poem).
     ============================================ -->

<!-- COVER PHOTO BANNER — click to expand -->
<img class="banner" 
     src="/assets/drivers/FIRSTNAME_Cover.jpg" 
     alt="DESCRIBE THE COVER PHOTO" 
     onclick="openLightbox()" 
     style="cursor: url('/assets/svg/cursor.svg') 8 2, auto; margin-bottom: 24px;">

<h1 class="driver-name">First Last</h1>

<!-- BIO CARD — photo on left, biography on right (stacks vertically on mobile) -->
<div class="bio-card">
  <div class="bio-image">
    <img src="/assets/drivers/FIRSTNAME_Profile.jpg" alt="DESCRIBE THE PROFILE PHOTO">
  </div>
  <div class="bio-text">
    <p>BIOGRAPHY GOES HERE. Use <strong>bold</strong> for book titles, <em>italics</em> for publication names.</p>
    
    <p class="connect-links">
      <!-- EXAMPLE: 1 link -->
      <!-- <a href="https://www.instagram.com/HANDLE">Instagram</a> -->
      <!-- <span class="interests-toggle" onclick="toggleInterests(this)">✦</span> -->
      
      <!-- EXAMPLE: 2 links -->
      <!-- <a href="https://www.instagram.com/HANDLE">Instagram</a> -->
      <!-- <span class="interest-separator">✦</span> -->
      <!-- <a href="https://www.amazon.com/dp/ASIN">Book Title</a> -->
      <!-- <span class="interests-toggle" onclick="toggleInterests(this)">✦</span> -->
      
      <!-- EXAMPLE: 3 links -->
      <!-- <a href="https://sites.google.com/view/username">Website</a> -->
      <!-- <span class="interest-separator">✦</span> -->
      <!-- <a href="https://www.instagram.com/HANDLE">Instagram</a> -->
      <!-- <span class="interest-separator">✦</span> -->
      <!-- <a href="https://bsky.app/profile/HANDLE">Bluesky</a> -->
      <!-- <span class="interests-toggle" onclick="toggleInterests(this)">✦</span> -->
    </p>

    <!-- MYSPACE INTERESTS TABLE — hidden behind the last ✦ -->
    <div class="myspace-interests">
      <table class="interests-table">
        <tr>
          <td>general</td>
          <td>THINGS THEY LIKE, HOBBIES, VIBES</td>
        </tr>
        <tr>
          <td>music</td>
          <td>BANDS, ARTISTS, SONGS</td>
        </tr>
        <tr>
          <td>movies</td>
          <td>FAVORITE FILMS</td>
        </tr>
        <tr>
          <td>television</td>
          <td>SHOWS THEY LOVE</td>
        </tr>
        <tr>
          <td>books</td>
          <td>FAVORITE READS</td>
        </tr>
        <tr>
          <td>heroes</td>
          <td>FAMILY, TEACHERS, WRITERS, INSPIRATIONS</td>
        </tr>
      </table>
    </div>
  </div>
</div>

<hr>

<!-- ============================================
     INTERVIEW CONTENT
     H3 for questions (small uppercase purple)
     Regular paragraph text for answers
     Repeat as many times as needed
     ============================================ -->

### INTERVIEW QUESTION ONE

Answer to question one goes here.

### INTERVIEW QUESTION TWO

Answer to question two goes here.

<!-- Add more question/answer pairs as needed -->

<!-- ============================================
     POEM SECTION (DELETE THIS SECTION IF NO POEM)
     The H1 heading creates an anchor link automatically.
     "# A Poem by First Last" becomes #a-poem-by-first-last
     This is what the Drivers page poetry links point to.
     ============================================ -->

# A Poem by First Last

## Poem Title

Poem text goes here.

Line breaks in markdown need two spaces at the end of each line  
or a blank line between stanzas.

<!-- DRIVER NAVIGATION — update Previous and Next based on gallery order -->
<div class="driver-nav">
  <a href="/Drivers/PREVIOUS_DRIVER/">← Previous Driver</a>
  <a href="/Drivers/NEXT_DRIVER/">Next Driver →</a>
</div>

<!-- LIGHTBOX — hidden by default, opens when banner is clicked -->
<div class="lightbox" id="lightbox" onclick="closeLightbox()">
  <span class="lightbox-close">close</span>
  <img src="/assets/drivers/FIRSTNAME_Cover.jpg" alt="DESCRIBE THE COVER PHOTO">
</div>

<script>
function openLightbox() {
  document.getElementById('lightbox').classList.add('open');
}
function closeLightbox() {
  document.getElementById('lightbox').classList.remove('open');
}
</script>