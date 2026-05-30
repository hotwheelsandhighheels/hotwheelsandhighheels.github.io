---
layout: default
title: Trunk
permalink: /Trunk/
---

<div class="wiki-page">

<h1>Trunk</h1>

<p class="wiki-intro">An ongoing collection of research and reference material re: memory work. This is a living document — sections will grow over time.</p>

<!-- TABLE OF CONTENTS
     Add new sections here as you write them.
     href="#anchor-name" jumps to that section on the page.
     anchor names must match the id="" on the heading below. -->
<div class="wiki-toc">
  <h3>Contents</h3>
  <ol class="wiki-toc-list">
    <li><a href="#millennial-epoch">The Millennial Epoch</a>
      <ol>
        <li><a href="#wordbank">How Many of You Have Ever Felt Personally Victimized By... </a></li>
      </ol>
    </li>
    <li><a href="#social-archive">The Social Archive</a>
      <ol>
        <li><a href="#borndigital">Born Digital Content</a></li>
        <li><a href="#AIcontent">AI Content Reception</a></li>
      </ol>
    </li>
    <li><a href="#bibliography">Bibliography</a>
    </li>
  </ol>
</div>

<hr>

<!-- ============================================
     SECTION 1 — THE MILLENNIAL EPOCH
     ============================================ -->

<h2 id="millennial-epoch">The Millennial Epoch</h2>

<p>Separate from the millennial age cohort, and much like the volta in poetry, an epoch references a turn in history characterized by dramatic change in perspective.</p>

<!-- 1.1 -->
<h3 id="wordbank">How many of you have ever felt personally victimized by [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;]</h3>

<p>In 2004, a well known cult-classic called <strong>Mean Girls</strong> graced our screens with the above quote. Fittingly, the characters in the movie are the eldest of an age cohort, dubbed <em>Millennials</em> by pop-sociologists Neil Howe and William Strauss, that came of age at the turn of the millennium. The lives of these individuals, and those succeeding them, have been dictated by a confluence of sociopolitical and -economic events. Such as:</p>

<ul class="ugh-list">
  <li>Post-Late-Capitalism</li>
  <li>Ronald Reagan</li>
  <li>War on Drugs</li>
  <li>Maturity Ratings</li>
  <li>Columbine</li>
  <li>y2k</li>
  <li>9/11</li>
  <li>Hurricane Katrina</li>
  <li>2008 Market Crash</li>
  <li>Gig Economy</li>
  <li>Data Colonialism</li>
  <li>Resilience Narrative</li>
  <li>White Supremacy</li>
  <li>Police Brutality</li>
  <li>MAGA</li>
  <li>Covid-19</li>
  <li>Artificial Intelligence</li>
</ul>

<!-- ADD MORE 1.x SECTIONS HERE as the essay grows
     Pattern:
     <h3 id="your-anchor">1.2 Your Section Title</h3>
     <p>Content here.</p>
     <hr>
-->

<!-- ============================================
     SECTION 2 — THE SOCIAL ARCHIVE
     ============================================ -->

<h2 id="social-archive">The Social Archive</h2>

<p>It is a marker of 21st century life that a large percentage of our cultural history has been digitally recorded online. The web can then be classified as an archive. More importantly, the web allows us to participate in the accumulation of objects — what gets included or excluded is a communal effort, giving new depth to archival value.</p>

<p>The web was built on a vision of a universally-linked hypertext communications system. It has offered us a lot more than that. It is a network-informed economy. It is a history built on parallel truths. It is, by all intentions, participatory.</p>

<h3 id="borndigital">Born Digital Content</h3>
<h4 id="memes">Memes</h4>

<!-- 2.1 -->
<h3 id="AIcontent">AI Content Reception</h3>

<p>A comparison of stances on AI generated content. Collected for reference and research.</p>

<!-- SLIDESHOW
     To add images:
     1. Put screenshots in /assets/AI
     2. Duplicate a .slide block below
     3. Update data-total to match new count
     Replace placeholder images with your actual screenshots. -->

<div class="slideshow" id="slideshow" data-current="1" data-total="6">

  <div class="slide active">
    <img src="/assets/AI/huffpost.png" alt="AI submission guidelines screenshot">
    <p class="caption">HuffPost</p>
  </div>
  <div class="slide">
    <img src="/assets/AI/chestnutreview.png" alt="AI submission guidelines screenshot">
    <p class="caption">Chestnut Review</p>
  </div>
  <div class="slide">
    <img src="/assets/AI/bluehorsepress.png" alt="Publication name submission guidelines">
    <p class="caption">Bluehorse Press</p>
  </div>
  <div class="slide">
    <img src="/assets/AI/cleavermagazine.png" alt="Publication name submission guidelines">
    <p class="caption">Cleaver Magazine</p>
  </div>
  <div class="slide">
    <img src="/assets/AI/indianapolisreview.png" alt="Publication name submission guidelines">
    <p class="caption">Indianapolis Review</p>
  </div>
  <div class="slide">
    <img src="/assets/AI/raleighreview.png" alt="Publication name submission guidelines">
    <p class="caption">Raleigh Review</p>
  </div>

  <!-- ADD MORE SLIDES HERE:
  <div class="slide">
    <img src="/assets/Images/submissions/pub2.jpg" alt="Publication name submission guidelines">
    <p class="caption">Publication name — key details here</p>
  </div>
  -->

<div class="slideshow-controls">
  <button class="slide-btn" onclick="changeSlide(-1)">&#8592;</button>
  <span class="slide-count"><span id="current">1</span> / <span id="total"></span></span>
  <button class="slide-btn" onclick="changeSlide(1)">&#8594;</button>
</div>

</div>

<script>
const slides = document.querySelectorAll('.slide');
document.getElementById('total').textContent = slides.length;

function changeSlide(direction) {
  const slideshow = document.getElementById('slideshow');
  const allSlides = slideshow.querySelectorAll('.slide');
  let current = parseInt(slideshow.getAttribute('data-current'));
  allSlides[current - 1].classList.remove('active');
  current = current + direction;
  if (current < 1) current = allSlides.length;
  if (current > allSlides.length) current = 1;
  allSlides[current - 1].classList.add('active');
  slideshow.setAttribute('data-current', current);
  document.getElementById('current').textContent = current;
}
</script>

<!-- ADD MORE 2.x SECTIONS HERE as the essay grows
     Pattern:
     <h3 id="your-anchor">2.2 Your Section Title</h3>
     <p>Content here.</p>
     <hr>
-->
<hr>
<p id="bibliography"><a href="https://www.zotero.org/groups/6565887/millennial_epoch">Bibliography</a></p>

</div>
