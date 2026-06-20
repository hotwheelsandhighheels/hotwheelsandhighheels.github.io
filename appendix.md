# APPENDIX: Quick Reference

---

## Color Hex Codes

| Color | Dark Mode | Light Mode | CSS Variable |
|-------|-----------|------------|-------------|
| Pink | `#ff00a3` | `#ff00a3` | `--pink` |
| Purple | `#a300ff` | `#a300ff` | `--purple` |
| Off-white | `#f5f0f5` | — | `--text` |
| Off-black | `#0a0608` | — | `--bg` |
| Place (chartreuse) | `#8fd3c7` | `#4f8f85` | `--theme-place` |
| Loss (coral) | `#ff8c69` | `#d96b48` | `--theme-loss` |
| Intimacy (gold) | `#ffe066` | `#b8860b` | `--theme-intimacy` |
| Web (cyan) | `#4df0ff` | `#008fb3` | `--theme-web` |
| Identity (orchid) | `#ffb3ff` | `#9b5ca9` | `--theme-identity` |
| Expression (mint) | `#7fffd4` | `#2ca88f` | `--theme-expression` |
| Future (silver) | `#e6e6e6` | `#666666` | `--theme-future` |
| Care (cherry blossom) | `#ffb7c5` | `#c96f84` | `--theme-care` |
| Witness (lavender) | `#c7b6ff` | `#7a6bc2` | `--theme-witness` |
| Surveillance (blue) | `#8fa8ff` | `#4f6fd6` | `--theme-surveillance` |
| Emergence (emerald) | `#9dff9a` | `#3aa33a` | `--theme-emergence` |
| Threshold (pale violet) | `#d6d0ff` | `#6f68b8` | `--theme-threshold` |

---

## System Pairings

| Theme | Timeline Category | Color |
|-------|-------------------|-------|
| Place | Local Memory | Chartreuse |
| Loss | Environment | Coral |
| Intimacy | Documentation | Gold |
| Web | Technology | Cyan |
| Identity | Politics | Orchid |
| Expression | Culture | Mint |
| Future | Economy | Silver |
| Care | Care | Cherry Blossom |
| Witness | Law & Justice | Lavender |
| Surveillance | Conflict & Security | Blue |
| Emergence | Science & Health | Emerald |
| Threshold | Infrastructure & Exploration | Pale Violet |

---

## tagMap (archive.md JavaScript)

```js
const tagMap = {
  // Quote Themes (12)
  'Place': 'place',
  'Loss': 'loss',
  'Intimacy': 'intimacy',
  'Web': 'web',
  'Identity': 'identity',
  'Expression': 'expression',
  'Future': 'future',
  'Care': 'care',
  'Witness': 'witness',
  'Surveillance': 'surveillance',
  'Emergence': 'emergence',
  'Threshold': 'threshold',

  // Archive Sections (6)
  'Upgrade You': 'place',
  'Going Viral': 'identity',
  'The Parasocial': 'expression',
  'Broken Record': 'loss',
  'Between You & I': 'intimacy',
  'AI': 'tech',

  // Timeline Categories (13)
  'Technology': 'tech',
  'Politics': 'politics',
  'Culture': 'expression',
  'Economy': 'economics',
  'Environment': 'environment',
  'Local Memory': 'local',
  'Documentation': 'documentation',
  'Science & Health': 'science',
  'Law & Justice': 'justice',
  'Conflict & Security': 'security',
  'Infrastructure & Exploration': 'infrastructure',
  'Care': 'care'
};

---

## Font Stack

| Element | Font | Weight | Size | Color |
|---------|------|--------|------|-------|
| H1 | Playfair Display italic | 400 | 32pt (varies) | `--pink` |
| H2 | Cormorant Garamond | 600 | 24pt | `--purple` |
| H3 | Lora | 500 | 12pt, 0.2em ls, uppercase | `--purple` |
| Body | Lora | 400 | 14pt, 1.75 lh | `--text` |
| Nav logo | Cormorant Garamond | 400 | 13pt, 0.22em ls, uppercase | `--purple` |
| Nav links | Lora | 400 | 11pt, 0.18em ls, uppercase | `--text` |

---

## Breakpoints

- **Desktop:** > 600px (default)
- **Mobile:** max-width: 600px

---

## Key CSS Classes (by section)

**Section 3 — Global:**
`.editor-name` — Ale's name on About page (nowrap, responsive)
`.ride-link` — "Come ride with us" on home page
`.about-page` `.trunk-page` — centered, responsive H1s

**Section 7 — Contributors:**
`.bio-card` `.bio-image` `.bio-text` — contributor bio layout
`.gallery` `.gallery-card` `.gallery-overlay` — driver gallery grid
`.lightbox` `.lightbox.open` `.lightbox-close` — cover photo lightbox
`.driver-nav` — previous/next navigation

**Section 8 — Components:**
`.pull-quote` — Cormorant italic, pink left border
`.tag` — purple pill tag
`.callout` — pink left border box
`.accordion` `.accordion-header` `.accordion-content` — expandable sections

**Section 11 — Quote System:**
`.tag-place` `.tag-loss` `.tag-intimacy` `.tag-web` `.tag-identity` `.tag-creativity` `.tag-future` — theme text colors
`.tag-quote` `.tag-quote.tag-place` (etc.) — colored quote blocks
`.timeline-tag` — base pill styles (shared across all pills)

**Section 13 — Trunk Dashboard:**
`.trunk-dashboard` `.trunk-card` `.trunk-card-full` — grid layout

**Section 14 — Artifact System:**
`.artifact` `.artifact-media` `.artifact-context` — artifact layout
`.artifact-description` `.artifact-significance` `.artifact-meta` — metadata
`.artifact-slideshow` `.artifact-slide` — slideshow

**Section 15 — Connections Map:**
`.connections-container` `.connection-node` `.center-node`
`.node-preview` `.node-preview-content`

**Section 16 — Timeline:**
`.timeline` `.timeline-entry` `.timeline-entry.left` `.timeline-entry.right`
`.timeline-year` `.timeline-era` `.timeline-legend`

**Section 21 — MySpace:**
`.connect-links` `.interests-toggle` `.myspace-interests` `.interests-table`

**Section 23 — Secret Links:**
`.secret-link` `a.secret-link`

---

## Key JavaScript Functions

| Function | Location | Purpose |
|----------|----------|---------|
| `toggleTheme()` | default.html, post.html | Light/dark mode switch |
| `toggleMenu()` | header.html | Mobile hamburger menu |
| `revTheEngine()` | footer.html | 4Runner audio + shake |
| `toggleInterests(el)` | post.html | MySpace ✦ dropdown |
| `openLightbox()` / `closeLightbox()` | post.html | Contributor photo lightbox |
| `openBlessingLightbox()` / `closeBlessingLightbox()` | default.html | Blessings image lightbox |
| `selectAllText(element)` | default.html | Survey copy-paste |
| `changeArtifactSlide(id, dir)` | archive.md | Artifact slideshow navigation |
| `updateArtifactMetadata(sectionId)` | archive.md | Metadata display update |
| `changeSlide(dir)` | archive.md | AI Reception slideshow |
| `toggleAccordion(header)` | notes.md | Reading notes accordions |

---

## Archive Section Artifact Counts

| Section | Count |
|---------|:-----:|
| Upgrade You | 5 |
| Going Viral | 6 |
| The Parasocial | 2 |
| Broken Record | 0 |
| Between You & I | 2 |
| AI Reception | 42 |

---

## Page URLs

| Page | URL |
|------|-----|
| Home | `/` |
| About | `/About/` |
| Drivers Gallery | `/Drivers/` |
| Trunk Dashboard | `/Trunk/` |
| Timeline | `/Trunk/epoch/` |
| Social Archive | `/Trunk/archive/` |
| Drivers Quotes | `/Trunk/drivers/` |
| Field Notes | `/Trunk/notes/` |
| Connections | `/Trunk/connections/` |
| Revving Up | `/revving-up/` |
| Submit | `/submit/` |
| Blessings | `/blessings/` |
| meAF | `/meAF/` |
| Style Guide | `/style-guide/` |
| 404 | `/404/` |

---

## Hidden Pages (sitemap: false)

meAF, Blessings, Submit, Style Guide, all 7 surveys, 404

---

*End of Appendix.*