---
layout: default
title: Style Guide
permalink: /style-guide/
sitemap: false
---

<!-- ============================================
     HOT WHEELS & HIGH HEELS — STYLE GUIDE
     Hidden page — not indexed by search engines (sitemap: false)
     Use this as a reference for every component available on the site.
     To use any component, copy the HTML block and paste into your markdown file.
     ============================================ -->

<!-- ============================================
     TYPOGRAPHY
     ============================================ -->

## Typography

# H1 — Playfair Display Italic Pink
## H2 — Cormorant Garamond Purple
### H3 — Lora Uppercase Purple

This is a paragraph in Lora light. _This is italic._ **This is bold.** This is a [pink link](#) that underlines on hover.

---

<!-- ============================================
     BLOCKQUOTE
     Pull quotes from interviews or poems.
     Usage: wrap text in > in markdown
     ============================================ -->

## Blockquote

<blockquote class="pull-quote">
  "The speed limit is 140mph but some cars go faster than that."
</blockquote>

---

<!-- ============================================
     IMAGE CAPTION
     Use below any image that needs a credit or description.
     Usage: add <p class="caption"> below your image markdown
     ============================================ -->

## Image Caption

![example](/assets/site/Banner.PNG)
<p class="caption">Photo by Kimberly Tobias — banner image</p>

---

<!-- ============================================
     TAG / BADGE
     For categorizing posts or labeling content.
     Usage: <span class="tag">label</span>
     ============================================ -->

## Tags

<span class="tag">poetry</span>
<span class="tag">interview</span>
<span class="tag">san diego</span>

---

<!-- ============================================
     CALLOUT BOX
     For highlighted notes, asides, or editor's notes.
     Usage: <div class="callout">your text</div>
     ============================================ -->

## Callout Box

<div class="callout">
  <p><em>Editor's note:</em> This interview has been lightly edited for clarity and length.</p>
</div>

---

<!-- ============================================
     WORD BANK / TAG CLOUD
     Borderless grid of words or terms.
     Usage: <ul class="ugh-list"> with <li> items
     ============================================ -->

## Word Bank

<ul class="ugh-list">
  <li>flash</li>
  <li>salvage</li>
  <li>velocity</li>
  <li>chrome</li>
  <li>asphalt</li>
  <li>stiletto</li>
  <li>throttle</li>
  <li>lace</li>
  <li>ignition</li>
  <li>gloss</li>
  <li>torque</li>
  <li>lipstick</li>
</ul>

---

<!-- ============================================
     AUDIO PLAYER
     For contributor recordings, poems read aloud, or sound clips.
     Usage: replace the src with your actual audio file path.
     Audio files go in /assets/sounds/
     ============================================ -->

## Audio Player

<div class="audio-player">
  <p class="audio-label">listen</p>
  <audio controls>
    <source src="/assets/sounds/Engine_Start_4runner.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</div>

---

<!-- ============================================
     VIDEO EMBED
     For embedded YouTube or Vimeo videos.
     Usage: replace the src with your actual embed URL.
     Get embed URL from YouTube: Share > Embed > copy src value only
     ============================================ -->

## Video Embed

<div class="video-wrap">
  <iframe
    src="https://www.youtube.com/embed/dQw4w9WgXcQ"
    title="Video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>

---

<!-- ============================================
     COVER PHOTO LIGHTBOX
     Clickable link that opens cover photo full screen.
     Usage: copy this entire block to the bottom of a contributor post.
     Change the img src and alt for each contributor.
     ============================================ -->

## Cover Photo Lightbox

<span class="cover-photo-link" onclick="openLightbox()">cover photo</span>

<div class="lightbox" id="lightbox" onclick="closeLightbox()">
  <span class="lightbox-close">close</span>
  <img src="/assets/drivers/Jon_Cover.jpg" alt="Jon Tobias cover photo">
</div>

<script>
function openLightbox() {
  document.getElementById('lightbox').classList.add('open');
}
function closeLightbox() {
  document.getElementById('lightbox').classList.remove('open');
}
</script>

---

<!-- ============================================
     HORIZONTAL RULE DIVIDER
     Pink 0.5px line used between bio and interview content.
     Usage: *** in markdown or <hr> in HTML
     ============================================ -->

## Divider

***

<!-- ============================================
     SUBSCRIBE FORM
     Buttondown email signup form.
     Usage: paste this wherever you want a signup form.
     Already on the Drivers page and Revving Up page.
     ============================================ -->

## Subscribe Form

<form
  action="https://buttondown.com/api/emails/embed-subscribe/hotwheelsandhighheels"
  method="post"
  class="embeddable-buttondown-form"
>
  <label for="bd-email">Enter your email</label>
  <input type="email" name="email" id="bd-email" />
  <input type="submit" value="Subscribe" />
  <p>
    <a href="https://buttondown.com/refer/hotwheelsandhighheels" target="_blank">
      Powered by Buttondown.
    </a>
  </p>
</form>
<!-- ============================================
     ACCORDION
     ============================================ -->

***

## Accordion

<div class="accordion">
  <button class="accordion-header" onclick="toggleAccordion(this)">
    Section Title <span class="accordion-icon">+</span>
  </button>
  <div class="accordion-content">
    <p>Content goes here. Can be any HTML — paragraphs, lists, images, whatever.</p>
  </div>
</div>
<script>
function toggleAccordion(header) {
  const content = header.nextElementSibling;
  const icon = header.querySelector('.accordion-icon');
  content.classList.toggle('open');
  icon.textContent = content.classList.contains('open') ? '−' : '+';
}
</script>