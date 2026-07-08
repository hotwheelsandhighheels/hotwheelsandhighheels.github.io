---
layout: default
title: Submit
permalink: /submit/
sitemap: false
---

<div class="survey-container">

  <h1>The Pump</h1>
<p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">
    <strong>Before you send something:</strong> Please do not submit private messages, images of minors, medical/legal information, addresses, or sensitive personal information unless it is your own material and you are comfortable with me reviewing it. <br>Any concerns should be noted in restrictions field. 
  </p>
  <hr>

  <form action="https://formspree.io/f/mwvjwgjy" method="POST" enctype="multipart/form-data" class="submit-form">

<input type="hidden" name="_subject" value="New HW&Hh archive submission">
<!-- File -->
<label for="file">File: </label>
<p class="form-hint">Upload. Or input link below.</p>
<input type="file" id="file" name="file" accept="file_extension,audio/*,video/*,image/*,.gif,media_type">

<!-- Source link -->
<label for="source_link">Source link: </label>
<p class="form-hint">Share source link if possible.</p>
<input type="url" id="source_link" name="source_link" placeholder="https://...">

<!-- Title -->
<label for="title">Title: </label>
<input type="text" id="title" name="title">

<!-- Creator / account -->
<label for="creator">Creator / account / username: <span class="form-required">*</span></label>
<p class="form-hint">Don't know? Write “unknown.”</p>
<input type="text" id="creator" name="creator" placeholder="e.g. @username, unknown, deleted account">

<!-- Date -->
<label for="date">Date created: </label>
<input type="text" id="date" name="date" placeholder="e.g. 03-15-2014, June 2026, circa 2012">

<!-- Capture / saved date -->
<label for="capture_date">Date saved, reblogged, or screenshot: </label>
<input type="text" id="capture_date" name="capture_date" placeholder="e.g. saved 05-27-2015, reblogged circa 2014">

<!-- Context -->
<label for="context">Context: <span class="form-required">*</span></label>
<p class="form-hint">What's the lore?</p>
<textarea id="context" name="context" rows="5" required></textarea>

<!-- Significance -->
<label for="significance">Significance: </label>
<p class="form-hint">Why is it important?</p>
<textarea id="significance" name="significance" rows="3"></textarea>

<!-- Restrictions -->
<label for="restrictions">Restrictions: <span class="form-required">*</span></label>
<p class="form-hint">Should anything be blurred, anonymized, kept private, credited carefully, or reviewed before publication? <br> If no, type 'clear.'</p>
<textarea id="restrictions" name="restrictions" rows="3"></textarea>

<!-- Ownership / rights -->
<fieldset class="form-fieldset">
  <legend>This is: <span class="form-required">*</span></legend>

  <label class="form-radio">
    <input type="radio" name="ownership" value="mine" required>
    Your original content
  </label>

  <label class="form-radio">
    <input type="radio" name="ownership" value="captured">
    Content you saved, screenshotted, reblogged, or captured
  </label>

  <label class="form-radio">
    <input type="radio" name="ownership" value="public-web">
    Public web content
  </label>

  <label class="form-radio">
    <input type="radio" name="ownership" value="unsure">
    Other / Not sure
  </label>
</fieldset>

<!-- Sensitivity -->
<fieldset class="form-fieldset">
  <legend>Privacy / sensitivity check <span class="form-required">*</span></legend>

  <label class="form-radio">
    <input type="radio" name="sensitivity" value="no-sensitive-info" required>
    This does NOT include private messages, minors, addresses, medical/legal information, or sensitive identifying details.
  </label>

  <label class="form-radio">
    <input type="radio" name="sensitivity" value="contains-sensitive-info">
    This may include private, identifying, or sensitive information. Review before publication.
  </label>

  <label class="form-radio">
    <input type="radio" name="sensitivity" value="not-sure">
    Review-only.
  </label>
</fieldset>

<!-- Consent / review -->
<fieldset class="form-fieldset">
  <legend>Submission agreement <span class="form-required">*</span></legend>

  <label class="form-checkbox">
    <input type="checkbox" name="agreement_review" value="yes" required>
    By submitting, you give Hot Wheels &amp; High Heels permission to review and/or use this content for archival research & website publication. You also agree that you provided the best possible source/context information and are at least 18 years old or have permission from a parent/guardian to submit.
  </label>
</fieldset>

<!-- Email -->
<label for="email">Contact </label>
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
  <a href="/Trunk/">Back 2 Trunk →</a>
</div>
