---
layout: default
title: Scratch Paper - Hot Wheels & High Heels
permalink: /Trunk/scratch-paper/
---

# Scratch Paper


<div class="scratch-grid" id="scratch-grid">

  <!-- POST-IT TEMPLATE

  SOLO NOTE:
  <article class="post-it pink">
    <p>Your short note here.</p>
  </article>

  LONG NOTE:
  <article class="post-it purple">
    <p>Short preview sentence.</p>
    <details>
      <summary>read more</summary>
      <p>Longer note text here.</p>
    </details>
  </article>

  STACK:
  <div class="post-stack" data-stack="stack-name">
    <article class="post-it pink">
      <p>First note.</p>
    </article>
    <article class="post-it purple">
      <p>Second note.</p>
    </article>
    <button type="button" class="stack-next">next →</button>
  </div>

  -->

  <!-- Post-0001 — double perspective -->
  <article class="post-it pink" data-post-id="Post-0001">
    <p>Whenever there is a memory being remembered we are performing the double perspective.</p>
    <details>
      <summary>read more</summary>
      <p>An archive, any archive, performs the double perspective <i>because</i> it is an archive. It is a memory aid; it does memory work.</p>
    </details>
  </article>

  <!-- Post-0002 + Post-0003 — accidentalarchivist stack -->
  <div class="post-stack" data-stack="accidentalarchivist">
    <article class="post-it purple" data-post-id="Post-0002" data-group-id="accidentalarchivist">
      <p>You will never find me. You will always find me.</p>
    </article>

    <article class="post-it pink" data-post-id="Post-0003" data-group-id="accidentalarchivist">
      <p>You are the documentary.</p>
    </article>

    <button type="button" class="stack-next">next →</button>
  </div>

  <!-- Post-0004 + Post-0005 — archons stack -->
  <div class="post-stack" data-stack="archons">
    <article class="post-it pink" data-post-id="Post-0004" data-group-id="archons">
      <p>"There is no political power without control of the archive, if not memory." (Manoff)</p>
    </article>

      <article class="post-it purple" data-post-id="Post-0005" data-group-id="archons">
      <p>"They have the power to interpret the archives... but in an unnatural fashion, that is to say in making the law or in making people respect the law." (Derrida)</p>
    </article>

    <button type="button" class="stack-next">next →</button>
  </div>

  <!-- Post-0006 + Post-0007 — internet culture stack -->
  <div class="post-stack" data-stack="internet-culture">
    <article class="post-it purple" data-post-id="Post-0006" data-group-id="internet-culture">
      <p>Born-digital objects, like memes, share these characteristics: virality, mutability, and intertextuality. (Ismail)</p>
    </article>

      <article class="post-it pink" data-post-id="Post-0007" data-group-id="internet-culture">
      <p>It is sometimes the case that memes develop into something foreign from their original value.</p>
      <details>
        <summary>read more</summary>
        <p>Often times, only a small insignificant piece of the whole gets taken and misinterpreted, and repeated to death.</p>
      </details>
    </article>

    <button type="button" class="stack-next">next →</button>
  </div>

  <!-- Post-0008 — artificial intelligence -->
  <article class="post-it purple" data-post-id="Post-0008" data-group-id="artificial-intelligence">
    <p>I think people accept that AI is here, what they don't accept is being "tricked" by AI.</p>
    <details>
      <summary>read more</summary>
      <p>The labelling of AI content is for transparency. The user gets to decide whether or not to interact with AI generated content.</p>
    </details>
  </article>

  <!-- Post-0009 — family -->
  <article class="post-it pink" data-post-id="Post-0009" data-group-id="family">
    <p>Where are my family's objects? Who keeps the archive?</p>
    <details>
      <summary>read more</summary>
      <p>What do we even do with all of this? Why did we want it? Why do we keep it? Why do we say that someday we will sit and sort through an archive that gets larger and uncontrollable with each passing day?</p>
    </details>
  </article>

  <!-- Post-0010 + Post-0011 — double-perspective stack -->
  <div class="post-stack" data-stack="double-perspective">
    <article class="post-it purple" data-post-id="Post-0010" data-group-id="double-perspective">
      <p>Richard Hugo says "Music doesn't conform to truth, truth conforms to music."</p>
    </article>

    <article class="post-it pink" data-post-id="Post-0011" data-group-id="double-perspective">
      <p>Literal truth versus literary truth... there is curation involved.</p>
    </article>

    <button type="button" class="stack-next">next →</button>
  </div>

  <!-- Post-0012 — archive fever -->
  <article class="post-it pink" data-post-id="Post-0012" data-group-id="archivefever">
    <p>We planned what was Instagramable. We directed what was Tweetable.</p>
    <details>
      <summary>read more</summary>
      <p>We used angles and filters and captions to force perspective. We became God, the creator. We created. We influenced. We locked ourselves in archival fever.</p>
    </details>
  </article>

</div>

<a href="https://www.zotero.org/groups/6565887/millennial_epoch/library" target="_blank" rel="noopener">Bibliography</a>

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/back-roads/">← Check the road map</a>
  <a href="/submit/">Fill my gas tank →</a>
</div>

<style>
.scratch-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(190px, 1fr));
  gap: 18px;
  margin: 32px 0;
}

.post-it,
.post-stack {
  aspect-ratio: 1 / 1;
}

.post-it {
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  padding: 18px;
  border-radius: 4px;
  overflow: auto;
  font-family: 'Lora', serif;
  font-size: 11pt;
  line-height: 1.45;
  position: relative;
  color: inherit;
}

.post-it p {
  margin: 0 0 10px 0;
  font-size: 11pt;
  line-height: 1.45;
  font-weight: 600;
  color: inherit;
}

.post-it details {
  margin-top: 8px;
  color: inherit;
}

.post-it summary {
  cursor: pointer;
  font-size: 9pt;
  font-style: italic;
  opacity: 0.75;
  color: inherit;
}

.post-it.pink {
  background: rgba(255, 0, 163, 0.2);
  border: 0.5px solid rgba(255, 0, 163, 0.4);
  box-shadow: 2px 2px 8px rgba(255, 0, 163, 0.15);
  color: var(--pink);
}

.post-it.purple {
  background: rgba(163, 0, 255, 0.2);
  border: 0.5px solid rgba(163, 0, 255, 0.4);
  box-shadow: 2px 2px 8px rgba(163, 0, 255, 0.15);
  color: var(--purple);
}

.post-stack {
  position: relative;
}

.post-stack .post-it {
  position: absolute;
  inset: 0;
}

.post-stack .post-it::before {
  content: "";
  position: absolute;
  inset: 6px -6px -6px 6px;
  border: 0.5px solid currentColor;
  opacity: 0.25;
  z-index: -1;
}

.stack-next {
  position: absolute;
  right: 10px;
  bottom: 10px;
  z-index: 5;
  background: transparent;
  border: none;
  color: currentColor;
  font-family: 'Lora', serif;
  font-size: 8pt;
  font-style: italic;
  padding: 0;
  cursor: pointer;
  opacity: 0.7;
}

.stack-next:hover {
  opacity: 1;
  text-decoration: underline;
  color: inherit;
}

.post-stack:has(.post-it.pink:not([hidden])) {
  color: var(--pink);
}

.post-stack:has(.post-it.purple:not([hidden])) {
  color: var(--purple);
}


@media (max-width: 600px) {
  .scratch-grid {
    grid-template-columns: repeat(auto-fill, minmax(145px, 1fr));
    gap: 12px;
  }

  .post-it {
    padding: 14px;
  }

  .post-it p {
    font-size: 10pt;
  }
}
</style>

<script>
(function() {
  const stacks = document.querySelectorAll('.post-stack');

  stacks.forEach(stack => {
    const notes = Array.from(stack.querySelectorAll('.post-it'));
    const button = stack.querySelector('.stack-next');
    let current = 0;

    function showNote(index) {
      notes.forEach((note, i) => {
        note.hidden = i !== index;
      });

      current = index;
    }

    if (button && notes.length > 1) {
      button.addEventListener('click', function() {
        const next = (current + 1) % notes.length;
        showNote(next);
      });
    }

    showNote(0);
  });
})();
</script>