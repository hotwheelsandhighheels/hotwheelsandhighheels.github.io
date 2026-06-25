---
layout: default
title: Double Perspective
permalink: /Trunk/dp/
title: Double Perspective - Hot Wheels & High Heels
---

# Double Perspective

This is a framework I built from combined notes on Vivian Gornick's *The Situation and the Story* and Phillip Lopate's *To Show and To Tell*. The theory doesn't have a name, but it's been written about — I just gave it a name and visualized it into a table.

The idea is simple: memory requires two selves. The one who lived it and the one who looks back. Neither controls the other. They're partners. The meaning lives in the space between them.

*Click each row to see what the partnership produces.*

---

<div class="double-perspective-interactive">

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Past</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Present</div>
  <div class="dp-result">Time</div>
</div>

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Reactive</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Organized</div>
  <div class="dp-result">Structure</div>
</div>

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Blind spots</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Self-awareness</div>
  <div class="dp-result">Insight</div>
</div>

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Objectivity</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Subjectivity</div>
  <div class="dp-result">Interpretation</div>
</div>

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Veracity / literal truth</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Authenticity / literary truth</div>
  <div class="dp-result">The story</div>
</div>

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Show</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Tell</div>
  <div class="dp-result">Narrative</div>
</div>

<div class="dp-row" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Situation / context</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Story / insight</div>
  <div class="dp-result">Meaning</div>
</div>

<div class="dp-row dp-summary" onclick="revealResult(this)" tabindex="0" role="button" aria-expanded="false">
  <div class="dp-experience">Experience Self</div>
  <div class="dp-connector">+</div>
  <div class="dp-narrator">Narrator Self</div>
  <div class="dp-result">Double Perspective</div>
</div>

</div>

<p style="text-align: center; font-size: 9pt; opacity: 0.5; margin-top: 32px;">Built from Gornick and Lopate. Named and visualized by Ale.</p>

---

## Where It Comes From

### Gornick — *The Situation and the Story*

The situation is the context or circumstance, sometimes the plot. The story is the insight, the wisdom, the thing one has come to say. Without detachment there can be no story. The narrator knows who is speaking and why she is speaking. Structure imposes order; order makes sentences more shapely. Memory is an organizing principle. Experience is only raw material.

### Lopate — *To Show and To Tell*

Turning oneself into a character is release from narcissism, not self-absorption. Allowing the reader to experience the past while benefiting from adult hindsight. Suspense in reflection — the thought process itself. Facts vs. truths: facts delimit, truths are what we make of them. Nonfiction thrives on daring, subjective flights of thought. Be curious about oneself. Self-curiosity grows from detachment. Follow your thoughts even if they lead to contradiction.

---

## How It Works in the Archive

The Drivers are the experience self — living it, reacting, no hindsight. They're the ones who were there.

The Trunk is the narrator self — organizing, interpreting, creating meaning from distance. It looks back at what the Drivers said and finds the patterns.

The timeline is the distance between them. The years that passed between living and telling.

Every artifact in the Social Archive was captured by an experience self and is being interpreted by a narrator self. The double perspective is happening on every page.

---

<!-- TRUNK NAVIGATION -->
<div class="driver-nav">
  <a href="/Trunk/notes/">← Dig thru the glove box</a>
  <a href="/Trunk/connections/">Check the road map →</a>
</div>

<script>
function revealResult(row) {
  const result = row.querySelector('.dp-result');
  const connector = row.querySelector('.dp-connector');
  const isOpen = row.getAttribute('aria-expanded') === 'true';
  
  if (isOpen) {
    result.classList.remove('revealed');
    connector.textContent = '+';
    row.setAttribute('aria-expanded', 'false');
  } else {
    result.classList.add('revealed');
    connector.textContent = '=';
    row.setAttribute('aria-expanded', 'true');
  }
}
</script>

<style>
.double-perspective-interactive {
  max-width: 800px;
  margin: 32px auto;
}

.dp-row {
  display: flex;
  align-items: center;
  padding: 12px 16px;
  margin-bottom: 4px;
  cursor: pointer;
  border-radius: 4px;
  transition: background 0.3s ease;
  border: 0.5px solid rgba(163, 0, 255, 0.1);
}

.dp-row:hover {
  background: rgba(255, 0, 163, 0.04);
  border-color: rgba(255, 0, 163, 0.2);
}

.dp-row:focus-visible {
  outline: 2px solid var(--pink);
  outline-offset: 2px;
}

.dp-experience,
.dp-narrator {
  flex: 1;
  font-family: 'Lora', serif;
  font-size: 13pt;
  color: var(--text);
  opacity: 0.85;
}

.dp-experience {
  text-align: right;
  padding-right: 16px;
}

.dp-narrator {
  text-align: left;
  padding-left: 16px;
}

.dp-connector {
  font-family: 'Cormorant Garamond', serif;
  font-size: 18pt;
  font-weight: 600;
  color: var(--pink);
  width: 32px;
  text-align: center;
  flex-shrink: 0;
  transition: all 0.3s ease;
}

.dp-result {
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-size: 14pt;
  color: var(--purple);
  opacity: 0;
  max-width: 0;
  overflow: hidden;
  white-space: nowrap;
  transition: all 0.4s ease;
  text-align: center;
}

.dp-result.revealed {
  opacity: 1;
  max-width: 200px;
  margin-left: 12px;
}

.dp-summary {
  margin-top: 12px;
  border-color: rgba(255, 0, 163, 0.25);
}

.dp-summary .dp-experience,
.dp-summary .dp-narrator {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 600;
  font-size: 15pt;
  color: var(--pink);
}

.dp-summary .dp-result {
  font-size: 16pt;
  color: var(--pink);
}

@media (max-width: 600px) {
  .dp-experience,
  .dp-narrator {
    font-size: 10pt;
  }
  
  .dp-connector {
    font-size: 14pt;
    width: 24px;
  }
  
  .dp-result {
    font-size: 11pt;
  }
  
  .dp-summary .dp-experience,
  .dp-summary .dp-narrator {
    font-size: 12pt;
  }
}
</style>