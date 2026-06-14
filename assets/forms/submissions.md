---
layout: default
title: Submit
permalink: /submit/
sitemap: false
---

<div class="survey-container">

  <h1>Send Me Something</h1>
  <p>anything from the millennial epoch.</p>

  <hr>

  <form action="https://formspree.io/f/mwvjwgjy" method="POST" enctype="multipart/form-data" class="submit-form">
    <label for="name">Name / alias <span class="form-optional">(optional)</span></label>
    <input type="text" id="name" name="name">
    <label for="email">Email <span class="form-required">*</span></label>
    <input type="email" id="email" name="email" required>
    <label for="file">File <span class="form-optional">(screenshot, image, gif)</span></label>
    <input type="file" id="file" name="file">
    <label for="category">This feels like it belongs under…</label>
    <select id="category" name="category">
      <option value="">— pick one if you want —</option>
      <option value="Upgrade You">Upgrade You</option>
      <option value="Going Viral">Going Viral</option>
      <option value="The Parasocial">The Parasocial</option>
      <option value="Broken Record">Broken Record</option>
      <option value="Between You & I">Between You & I</option>
      <option value="AI Reception">AI Reception</option>
      <option value="Not sure">Not sure</option>
    </select>
    <label for="context">Context <span class="form-required">*</span></label><br>
    <p class="form-hint">What is this? Where did it come from? Why did you save it?</p>
    <textarea id="context" name="context" rows="5" required></textarea>
    <label for="significance">Why it matters:</label><br>
    <p class="form-hint">What does this show about life in the millennial epoch? (Skip if you're not sure.)</p>
    <textarea id="significance" name="significance" rows="3"></textarea>
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
    <label for="date">Date <span class="form-optional">(when this is from, or when you saved it)</span></label>
    <input type="text" id="date" name="date" placeholder="e.g. 03-15-2014 or circa 2012">
    <input type="text" name="_gotcha" style="display:none">
    <button type="submit" class="submit-btn">Send it ✦</button>
  </form>

  <p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">everything goes directly to alejandra@hotwheelsandhighheels.com</p>

</div>