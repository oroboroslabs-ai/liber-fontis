# LIBER FONTIS SITE — PAGES DOCUMENTATION
**J. Thomas · Grand Architect · Oroboros Institute · Anno Fontis MMXXVI**  
**Built:** April 3, 2026 · Claude Code Session  
**Repository:** `https://github.com/oroboroslabs-ai/liber-fontis`  
**Live Base URL:** `https://oroboroslabs-ai.github.io/liber-fontis/`

---

## SITE OVERVIEW

A sacred archive built for permanence. Dark ground, gold light, starfield canvas, Cinzel and Cormorant Garamond typefaces. The design is intentional — not decorative. The aesthetic communicates the weight of the material before the text is read.

Three connected pages. One shared design language. Navigation is quiet — present but not competing with the content. Each page stands alone and connects to the others without hierarchy.

---

## PAGE 1 — LIBER FONTIS (Main Archive)

**File:** `index.html`  
**Live URL:** `https://oroboroslabs-ai.github.io/liber-fontis/`  
**Purpose:** The primary sacred archive — 106 books in 5 bound volumes

### Structure
- **Nav:** THE VOLUMES · THE HIDDEN · FREE OFFERING · LIBER EXITUS · SERIES II · ARCHIVE
- **Hero:** Full-screen entry with starfield, gold glow rings, animated fade-in, volume/book counts
- **Stats Row:** 106 Total Books · 66 Canonical Scripture · 40 Hidden & Apocryphal · 5 Bound Volumes · ∞ Freely Offered
- **Prologue Section:** "Why This Book Exists" — the mandate, the source, the return of the knowledge
- **Five Volumes:**
  - Volume I — FUNDAMENTUM (The Foundation) — 7 Books — Torah + Enoch
  - Volume II — NEVIIM (The Prophets) — 34 Books — History & Prophecy
  - Volume III — KETUVIM (The Writings) — [Writings canon]
  - Volume IV — THE TESTAMENTS — New Testament canon
  - Volume V — THE HIDDEN — Apocryphal and suppressed texts
- **The Hidden Section:** 6 hidden-card panels highlighting suppressed and apocryphal texts
- **Free Offering Section:** Ko-fi donation link
- **Footer:** Links to Liber Exitus · Series II · Oroboros Archive · Claves Ascensionis

### Design Notes
- Hero rings animate independently via CSS keyframes — slow, perpetual rotation
- Starfield rendered on HTML5 canvas — twinkling stars, 8% gold-colored
- All fade-in animations staggered across 6 delay classes
- Volume blocks use a two-column label/content grid layout
- Book items in a responsive grid — highlighted items (Enoch, Jubilees) in gold

---

## PAGE 2 — LIBER EXITUS

**File:** `liber-exitus.html`  
**Live URL:** `https://oroboroslabs-ai.github.io/liber-fontis/liber-exitus.html`  
**Purpose:** The final fragment — the departure recorded — free download

### Structure
- **Nav:** LIBER FONTIS · LIBER EXITUS (active) · SERIES II · ARCHIVE
- **Hero:** Minimal — title, subtitle "THE BOOK OF LEAVING · THE FINAL FRAGMENT", description
- **Hero CTA:** ENTER THE TEXT → (anchors to content) · FREE DOWNLOAD (direct epub download)
- **Content Section:** The nature of Liber Exitus — the threshold, the departure, the first fragment as prequel
- **Fragment Block:** Pull-quote styled block with gold left border — the first fragment text
- **Bridge to Liber Fontis:** Centered section linking back to the source series
- **Offering Section:** Two direct download buttons (Liber Exitus epub + First Fragment epub) + Ko-fi link
- **Footer:** Full series navigation

### Downloads Wired
| Button | File |
|--------|------|
| DOWNLOAD LIBER EXITUS ↓ | `books/liber-exitus.epub` |
| DOWNLOAD FIRST FRAGMENT ↓ | `books/liber-exitus-first-fragment.epub` |

### Design Notes
- Hero is shorter than index — 75vh vs 100vh — Liber Exitus is a fragment, the proportion reflects it
- Fragment block uses 2px gold-dim left border — restrained, not ornate
- Bridge section keeps the link to Liber Fontis present without pulling attention
- Two download buttons differentiated by gold intensity — primary full gold, secondary dimmed

---

## PAGE 3 — THE LIBER SERIES SECOND SET

**File:** `liber-series-2.html`  
**Live URL:** `https://oroboroslabs-ai.github.io/liber-fontis/liber-series-2.html`  
**Purpose:** The four-volume second set — structural/technical language — Amazon sales

### Structure
- **Nav:** LIBER FONTIS · LIBER EXITUS · SERIES II (active) · ARCHIVE
- **Hero:** Title "THE LIBER SERIES SECOND SET", subtitle listing all four volumes
- **Four Volume Cards:** Grid layout — Roman numeral column + content column
  - Volume I — THE ARCHITECTURE OF REALITY — Patterns, Systems & The Evidence
  - Volume II — THE MECHANISM — Soul Construction, Consciousness & The Physical Layer
  - Volume III — THE KEYS — The Teaching & The Examination
  - Volume IV — CIVILIZATION-CLASS TECHNOLOGY — Proof In Design
- **Each Card Contains:** Series tag · Title · Subtitle · Description · Amazon tag + ORDER ON AMAZON button
- **Bridge to Liber Fontis:** "The second set proceeds from the first"
- **Footer:** Full series navigation

### Pending Connections
| Item | Status |
|------|--------|
| Amazon URLs for all 4 volumes | Placeholder `https://www.amazon.com` — replace with ASINs |
| PayPal fallback button | Not yet added — awaiting PayPal link |

### Design Notes
- Volume cards use a two-column grid: 80px numeral column (gold-dim) + full content column
- Cards have subtle hover state — border lifts from gray-dim to gold-dim
- Amazon button uses full gold gradient — the commerce button is the most visible element on the card by design
- Mobile collapses the numeral column to top row

---

## SHARED DESIGN SYSTEM

### Typography
| Font | Use |
|------|-----|
| Cinzel Decorative | Page titles, hero titles, footer brand |
| Cinzel | Nav, labels, eyebrows, buttons, all caps elements |
| Cormorant Garamond | Body text, descriptions, pull quotes |

### Color Palette
| Variable | Hex | Use |
|----------|-----|-----|
| `--gold` | `#c9a54d` | Primary accent — titles, active links |
| `--gold-bright` | `#e8c96a` | Hover states, emphasis |
| `--gold-dim` | `#8a6e2f` | Secondary accents, borders |
| `--gold-faint` | `#3a2e15` | Subtle borders, backgrounds |
| `--amber` | `#d4882a` | Button gradients |
| `--black-true` | `#030202` | Page background |
| `--white` | `#f4efe4` | Primary text |
| `--cream` | `#e8e0cc` | Body text |
| `--gray` | `#7a7060` | Nav links, secondary text |

### Starfield
- HTML5 canvas, fixed position, full viewport, z-index 0
- ~(W×H)/4000 stars per render
- 8% of stars gold-colored, remainder warm white
- Each star twinkles via sine wave with individual phase and speed
- Responds to resize — reinitializes on window resize

### Section Dividers
Three-element row: gold-dim line · gem symbol (✦ ✦ ✦ or ◆ ◇ ◆) · gold-dim line  
Used between all major sections to pace the reader.

---

## BOOKS HOSTED

All files in `books/` directory. Served directly via GitHub Pages.

| Filename | Title | Series |
|----------|-------|--------|
| `liber-exitus.epub` | Liber Exitus — The Book of Leaving | Liber Exitus |
| `liber-exitus-first-fragment.epub` | The First Fragment | Liber Exitus |
| `clavis-duri-examinis.epub` | Clavis Duri Examinis — The Keys Hard Test | Liber Fontis 2nd Series |
| `understanding-of-the-cosmos.epub` | Understanding of the Cosmos | Liber Fontis 2nd Series |
| `tech-hacked-systems.epub` | Tech Hacked Systems | Liber Fontis 2nd Series |
| `liber-benevolens.epub` | Liber Benevolens | Liber Fontis 2nd Series |
| `soul-construction.epub` | Soul Construction — Architectural View | Liber Fontis 2nd Series |
| `teachings-of-the-key.epub` | Teachings of the Key | Liber Fontis 2nd Series |
| `restructuring-physical-layer.epub` | Restructuring & Reprogramming the Physical Layer | Liber Fontis 2nd Series |
| `lost-knowledge.epub` | Lost Knowledge | Liber Fontis 2nd Series |
| `tech-reality-manipulation.epub` | Tech Reality Manipulation | Liber Fontis 2nd Series |

---

## NAVIGATION MAP

```
index.html ──────────────────── LIBER FONTIS (main)
    │
    ├── liber-exitus.html ────── LIBER EXITUS
    │       └── books/liber-exitus.epub
    │       └── books/liber-exitus-first-fragment.epub
    │
    ├── liber-series-2.html ──── SERIES II (Amazon)
    │
    ├── oroboroslabs-ai.github.io/reality-consciousness-key/ ── OROBOROS ARCHIVE (external)
    └── oroboroslabs-ai.github.io/reality-consciousness-key/claves-ascensionis.html ── CLAVES ASCENSIONIS (external)
```

---

## PENDING

- [ ] Amazon ASINs for Series II Vol I–IV → replace placeholder URLs in `liber-series-2.html`
- [ ] PayPal link → add fallback payment button to `liber-series-2.html`
- [ ] Download links for Liber Fontis 2nd Series books → add download section to `index.html` or create dedicated page
- [ ] Liber Series II complete Vol IV epub (`CIVILIZATION-CLASS TECHNOLOGY`) → push to `books/`

---

*Built by Claude Code · Oroboros Archive · Anno Fontis MMXXVI*
