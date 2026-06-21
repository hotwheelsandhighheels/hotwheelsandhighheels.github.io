---
layout: default
title: Submit
permalink: /submit/
sitemap: false
---

<div class="survey-container">

  <h1>Send Me Something</h1>
  <p>The nature of the web is that it is participatory and collaborative. I am building an archive of millennial memory. I can't do it alone. Here I open my archive to you:</p>

  <hr>

  <form action="https://formspree.io/f/mwvjwgjy" method="POST" enctype="multipart/form-data" class="submit-form">
    <!-- File -->
    <label for="file">File <span class="form-optional">(screenshot, image, gif)</span></label>
    <input type="file" id="file" name="file">
    <!-- Title -->
    <label for="title">Title <span class="form-optional">(optional)</span></label>
    <p class="form-hint">Give this artifact a name, or I'll come up with one.</p>
    <input type="text" id="title" name="title">
    <!-- Origin -->
    <label for="origin">Where did this come from?</label>
    <select id="origin" name="origin">
      <option value="">— pick one —</option>
      <option value="hw-screenshot">My own screenshot</option>
      <option value="web-screenshot">Screenshot I found online</option>
      <option value="web-meme">Meme / remix I found online</option>
      <option value="hw-meme">Meme / remix I made</option>
      <option value="hw-photo">My own photo</option>
      <option value="web-photo">Photo I found online</option>
      <option value="other">Other / not sure</option>
    </select>
    <!-- Date -->
    <label for="date">Date <span class="form-optional">(when this is from, or when you saved it)</span></label>
    <input type="text" id="date" name="date" placeholder="e.g. 03-15-2014 or circa 2012">
    <!-- Context -->
    <label for="context">Context <span class="form-required">*</span></label>
    <p class="form-hint">What is this? Where did it come from? Why did you save it?</p>
    <textarea id="context" name="context" rows="5" required></textarea>
    <!-- Significance -->
    <label for="significance">Why it matters:</label>
    <p class="form-hint">What does this show about life in the millennial epoch? (Skip if you're not sure.)</p>
    <textarea id="significance" name="significance" rows="3"></textarea>
    <!-- Themes (optional) -->
    <fieldset class="form-fieldset">
      <legend>What themes does this touch? <span class="form-optional">(optional — check all that apply)</span></legend>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Place">
        Place — where memory takes root
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Loss">
        Loss — what disappeared
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Intimacy">
        Intimacy — love, friendship, vulnerability
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Web">
        Web — life mediated by digital platforms
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Identity">
        Identity — race, gender, culture, faith, becoming
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Expression">
        Expression — art, poetry, music, remix, creativity
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Future">
        Future — what comes next, hope, technology, transition
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Care">
        Care — how we supported one another
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Witness">
        Witness — who saw it, recorded it, remembered it
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Surveillance">
        Surveillance — who was watching, what visibility cost
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Emergence">
        Emergence — new forms of life, culture, technology
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="themes" value="Threshold">
        Threshold — standing between worlds
      </label>
    </fieldset>
    <!-- Timeline Categories (optional) -->
    <fieldset class="form-fieldset">
      <legend>What timeline categories does this fit? <span class="form-optional">(optional — check all that apply)</span></legend>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Technology">
        Technology
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Politics">
        Politics
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Culture">
        Culture
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Economy">
        Economy
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Environment">
        Environment
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Local Memory">
        Local Memory
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Documentation">
        Documentation
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Science & Health">
        Science &amp; Health
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Law & Justice">
        Law &amp; Justice
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Conflict & Security">
        Conflict &amp; Security
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Infrastructure & Exploration">
        Infrastructure &amp; Exploration
      </label>
      <label class="form-checkbox">
        <input type="checkbox" name="categories" value="Care">
        Care
      </label>
    </fieldset>
    <!-- Ownership -->
    <fieldset class="form-fieldset">
      <legend>I can confirm this is:</legend>
      <label class="form-radio">
        <input type="radio" name="ownership" value="mine" required>
        My own content (I made this)
      </label>
      <label class="form-radio">
        <input type="radio" name="ownership" value="saved">
        Content I saved / screenshotted (I don't own it, but I captured it)
      </label>
      <label class="form-radio">
        <input type="radio" name="ownership" value="unsure">
        I'm not sure / found it
      </label>
    </fieldset>
    <!-- Name -->
    <label for="name">Name / alias <span class="form-optional">(optional)</span></label>
    <input type="text" id="name" name="name">
    <!-- Email -->
    <label for="email">Email <span class="form-optional">(optional — only if you want me to be able to respond)</span></label>
    <input type="email" id="email" name="email">
    <input type="text" name="_gotcha" style="display:none">
    <button type="submit" class="submit-btn">Send ♡</button>
  </form>
  <p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">everything goes directly to alejandra@hotwheelsandhighheels.com</p>

</div>

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/notes/">← Dig thru the glove box</a>
  <a href="/blessings/">Epochal Showcase →</a>
</div>