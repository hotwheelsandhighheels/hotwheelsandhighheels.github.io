---
layout: default
title: Submit
permalink: /submit/
sitemap: false
---

<div class="survey-container">

  <h1>Gas Pump</h1>

  <p>Drop something in!</p>
  <p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">
    <strong>Before you send something:</strong> submissions are reviewed before anything is published. Please do not submit private messages, images of minors, medical/legal information, addresses, or sensitive personal information unless it is your own material and you are comfortable with me reviewing it. If you are not sure, tell me in the context box.
  </p>
  <hr>

  <form action="https://formspree.io/f/mwvjwgjy" method="POST" enctype="multipart/form-data" class="submit-form">

<input type="hidden" name="_subject" value="New HW&Hh archive submission">
<!-- File -->
<label for="file">File <span class="form-optional">(screenshot, image, gif)</span></label>
<p class="form-hint">Upload the artifact if you have it. If you only have a link, use the source/link field below.</p>
<input type="file" id="file" name="file" accept="image/*,.gif">

<!-- Source link -->
<label for="source_link">Source / link <span class="form-optional">(optional, but helpful)</span></label>
<p class="form-hint">If this came from Tumblr, Twitter/X, Tenor, GIPHY, Reddit, Instagram, YouTube, a blog, or another platform, paste the link if you have it.</p>
<input type="url" id="source_link" name="source_link" placeholder="https://...">

<!-- Title -->
<label for="title">Title <span class="form-optional">(optional)</span></label>
<p class="form-hint">Give this artifact a name, or I'll come up with one.</p>
<input type="text" id="title" name="title">

<!-- Origin -->
<label for="origin">Where did this come from?</label>
<select id="origin" name="origin" required>
  <option value="">— pick one —</option>
  <option value="hw-original">I made this</option>
  <option value="hw-screenshot">My own screenshot / from my own device</option>
  <option value="hw-photo">My own photo</option>
  <option value="hw-meme">Meme / remix I made</option>
  <option value="web-tumblr">Tumblr</option>
  <option value="web-twitter-x">Twitter / X</option>
  <option value="web-tenor">Tenor</option>
  <option value="web-giphy">GIPHY</option>
  <option value="web-instagram">Instagram</option>
  <option value="web-reddit">Reddit</option>
  <option value="web-meme">Meme / remix I found online</option>
  <option value="web-screenshot">Screenshot I found online</option>
  <option value="web-photo">Photo I found online</option>
  <option value="other">Other / not sure</option>
</select>

<!-- Creator / account -->
<label for="creator">Creator / account / username <span class="form-optional">(optional, if known)</span></label>
<p class="form-hint">If you know who posted or made it, include the name, handle, or account. If you don't know, write “unknown.”</p>
<input type="text" id="creator" name="creator" placeholder="e.g. @username, unknown, deleted account">

<!-- Date -->
<label for="date">Date <span class="form-optional">(when this is from, when it was posted, or when you saved it)</span></label>
<input type="text" id="date" name="date" placeholder="e.g. 03-15-2014, June 2026, circa 2012">

<!-- Capture / saved date -->
<label for="capture_date">When did you capture, save, reblog, or screenshot it? <span class="form-optional">(optional)</span></label>
<input type="text" id="capture_date" name="capture_date" placeholder="e.g. saved 05-27-2015, reblogged circa 2014">

<!-- Context -->
<label for="context">Context <span class="form-required">*</span></label>
<p class="form-hint">What is this? Where did it come from? Why did you save it? What do you remember about it?</p>
<textarea id="context" name="context" rows="5" required></textarea>

<!-- Significance -->
<label for="significance">Why it matters</label>
<p class="form-hint">What does this show about life in the millennial epoch? Skip if you're not sure.</p>
<textarea id="significance" name="significance" rows="3"></textarea>

<!-- Restrictions -->
<label for="restrictions">Restrictions or concerns <span class="form-optional">(optional)</span></label>
<p class="form-hint">Tell me if anything should be blurred, anonymized, kept private, credited carefully, or reviewed before publication.</p>
<textarea id="restrictions" name="restrictions" rows="3"></textarea>

<!-- Themes -->

<fieldset class="form-fieldset">
  <legend>What themes does this touch? <span class="form-optional">(optional — check all that apply)</span></legend>

<label class="form-checkbox"><input type="checkbox" name="themes" value="Place"> Place</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Loss"> Loss</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Intimacy"> Intimacy</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Web"> Web</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Identity"> Identity</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Expression"> Expression</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Future"> Future</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Care"> Care</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Witness"> Witness</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Surveillance"> Surveillance</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Emergence"> Emergence</label> <label class="form-checkbox"><input type="checkbox" name="themes" value="Threshold"> Threshold</label>

</fieldset>


<!-- Timeline Categories -->
<fieldset class="form-fieldset">
  <legend>What timeline categories does this fit? <span class="form-optional">(optional — check all that apply)</span></legend>

  <label class="form-checkbox"><input type="checkbox" name="categories" value="Technology"> Technology</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Politics"> Politics</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Culture"> Culture</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Economy"> Economy</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Environment"> Environment</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Local Memory"> Local Memory</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Documentation"> Documentation</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Science & Health"> Science &amp; Health</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Law & Justice"> Law &amp; Justice</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Conflict & Security"> Conflict &amp; Security</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Infrastructure & Exploration"> Infrastructure &amp; Exploration</label>
  <label class="form-checkbox"><input type="checkbox" name="categories" value="Care"> Care</label>
</fieldset>

<!-- Ownership / rights -->
<fieldset class="form-fieldset">
  <legend>I can confirm this is: <span class="form-required">*</span></legend>

  <label class="form-radio">
    <input type="radio" name="ownership" value="mine" required>
    My own content / I made this
  </label>

  <label class="form-radio">
    <input type="radio" name="ownership" value="captured">
    Content I saved, screenshotted, reblogged, or captured from my own device/account
  </label>

  <label class="form-radio">
    <input type="radio" name="ownership" value="public-web">
    Public web content / meme / GIF / remix I found online
  </label>

  <label class="form-radio">
    <input type="radio" name="ownership" value="unsure">
    I'm not sure / provenance is unclear
  </label>
</fieldset>

<!-- Sensitivity -->
<fieldset class="form-fieldset">
  <legend>Privacy / sensitivity check <span class="form-required">*</span></legend>

  <label class="form-radio">
    <input type="radio" name="sensitivity" value="no-sensitive-info" required>
    To my knowledge, this does not include private messages, minors, addresses, medical/legal information, or sensitive identifying details.
  </label>

  <label class="form-radio">
    <input type="radio" name="sensitivity" value="contains-sensitive-info">
    This may include private, identifying, or sensitive information. Please review before any publication.
  </label>

  <label class="form-radio">
    <input type="radio" name="sensitivity" value="not-sure">
    I'm not sure. Please treat this as review-only unless we discuss it.
  </label>
</fieldset>

<!-- Consent / review -->
<fieldset class="form-fieldset">
  <legend>Submission agreement <span class="form-required">*</span></legend>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_review" value="yes" required>
    I understand that submitting something does not guarantee publication. It will be reviewed first.
  </label>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_store" value="yes" required>
    I give Hot Wheels &amp; High Heels permission to receive, store, review, describe, and catalog this submission as part of the project archive.
  </label>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_publish" value="yes" required>
    If selected, I give Hot Wheels &amp; High Heels permission to publish, display, quote, describe, preserve, and discuss this submission in relation to the project, unless I have listed restrictions above.
  </label>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_rights" value="yes" required>
    I understand that “found online” or “saved by me” describes provenance, not ownership. I have provided as much source/context information as I can.
  </label>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_web" value="yes" required>
    I understand that public web publication may be shared, screenshotted, linked, cached, indexed, or archived by third parties. HW&amp;Hh can revise or remove its own pages but cannot fully control outside copies.
  </label>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_age" value="yes" required>
    I am at least 18 years old, or I have permission from a parent/guardian to submit.
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
```

  </form>

  <p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">
    submissions are processed through Formspree and sent to alejandra@hotwheelsandhighheels.com
  </p>

</div>

<!-- TRUNK NAVIGATION -->

<div class="driver-nav">
  <a href="/Trunk/scratch-paper">← Dig thru the glove box</a>
  <a href="/blessings/">Epochal Showcase →</a>
</div>
