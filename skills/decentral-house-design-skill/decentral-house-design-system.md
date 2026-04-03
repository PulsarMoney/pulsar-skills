---
name: Decentral House Design System
description: Best practices for Decentral House on-brand-designs
metadata:
  tags: decentral, uxui, graphic
---

# Decentral House — Design System

> A comprehensive reference for AI agents and designers building on-brand assets for **Decentral House** — landing pages, sub-pages, presentation decks, social media visuals, and animations.

*Extracted from Figma source: `zjQsGcu1HnRDzdUJxeOFSP` · Node `2043:98` · April 2026*

---

## 1. Brand Overview

**Decentral House** is Geneva's premier innovation hub — a physical and community infrastructure for AI, FinTech, and Web3 pioneers.

### One-Sentence Description
> "The Premier Innovation Hub in Geneva."

### Tagline
> "A strategic base for AI, FinTech, and Web3 pioneers. Private Offices, Co-working, World-class Events, and a thriving community of innovators."

### Key Stats
- **9** Private Suites
- **850m²** Total Space
- **200+** Members
- **Up to 120** guests for events
- Location: **Geneva, Switzerland**

### Services
1. Events & Venue Rental
2. Domiciliation
3. Private Offices
4. Co-working & Community

### Name Usage
- Always refer to as **"Decentral House"** — never abbreviated
- The logo lockup includes a stylized lightning bolt mark alongside the wordmark

---

## 2. Color System

The palette is radically minimal: one bold green, two darks, and a grayscale. The green is the *only* accent — use it with intention.

### Core Palette

| Token | Name | Hex | Usage |
|-------|------|-----|-------|
| `--color-green` | Brand Green | `#54DC54` | CTAs, accents, bullets, hero period, stat numbers |
| `--color-black` | Near Black | `#1A1A1A` | Hero headings, primary dark text |
| `--color-dark` | Dark Background | `#121212` | Dark section backgrounds (pricing, community) |
| `--color-white` | White | `#FFFFFF` | Page backgrounds, button fills on green |
| `--color-gray-88` | Nav Gray | `#888888` | Nav links, muted labels, captions |
| `--color-gray-77` | Body Gray | `#777777` | Body text, descriptions |
| `--color-gray-55` | Secondary Text | `#555555` | Outline button text |
| `--color-gray-aa` | Label Gray | `#AAAAAA` | Stats labels, tertiary captions |
| `--color-border` | Border | `#DDDDDD` | Button outlines, subtle dividers |
| `--color-border-header` | Header Border | `#E8E8E8` | Header bottom border |

### CSS Custom Properties
```css
:root {
  --color-green:         #54DC54;
  --color-black:         #1A1A1A;
  --color-dark:          #121212;
  --color-white:         #FFFFFF;
  --color-gray-88:       #888888;
  --color-gray-77:       #777777;
  --color-gray-55:       #555555;
  --color-gray-aa:       #AAAAAA;
  --color-border:        #DDDDDD;
  --color-border-header: #E8E8E8;
}
```

### White Opacity Variants (Dark Surfaces)

Use exclusively inside `#121212` dark sections:

| Token | Value | Usage |
|-------|-------|-------|
| `--white-6` | `rgba(255,255,255,0.06)` | Feature list row dividers |
| `--white-15` | `rgba(255,255,255,0.15)` | Ghost button borders |
| `--white-35` | `rgba(255,255,255,0.35)` | Price suffix text (/year) |
| `--white-50` | `rgba(255,255,255,0.50)` | Feature list body text |
| `--white-60` | `rgba(255,255,255,0.60)` | Ghost button label text |

### Three Surface Modes

Every layout is built from exactly three surface types:

**1. Light (default)** — white `#FFFFFF` background with `#888` borders
**2. Brand Green** — `#54DC54` full-bleed background, white text on top
**3. Dark** — `#121212` background, white/opacity text, green accents

Never mix surfaces within a single section. Each section is fully committed to one mode.

### Color Rules
- Green is the **only** accent color — never use blue, orange, purple, or any secondary hue
- On green backgrounds: text is white or black only
- On dark backgrounds: text uses white opacity variants; `#54DC54` for labels and bullets
- Body text on light backgrounds: always `#777` or `#888`
- Headings on light backgrounds: always `#1A1A1A`

---

## 3. Typography

Decentral House uses **Manrope** as its sole brand typeface, with **Arial Bold** as a secondary utility font for ghost CTAs only.

### Typefaces

| Font | Role | Import |
|------|------|--------|
| **Manrope** | Primary — all headings, body, nav, buttons | Google Fonts or variable font |
| **Arial Bold** | Secondary — ghost button labels only | System font |

### Type Scale

| Style | Font | Weight | Size | Tracking | Line Height | Color (default) | Usage |
|-------|------|--------|------|----------|-------------|-----------------|-------|
| **Hero H1** | Manrope | Medium (500) | 72px | −2.16px | tight (1.0) | `#1A1A1A` | Main page headline |
| **Section H1 (Dark)** | Manrope | SemiBold (600) | 56px | −1.68px | tight | `#FFFFFF` | Section title on dark bg |
| **Service Title** | Manrope | SemiBold (600) | 48px | −1.44px | 0.95 | `#FFFFFF` | Active service name on green |
| **Body Large** | Manrope | Regular (400) | 18px | −0.54px | 1.6 | `#777777` | Hero subheading, intro text |
| **Body Section** | Manrope | Regular (400) | 17.5px | −0.525px | 1.3 | `#FFFFFF` | Copy on green/dark sections |
| **Pricing Number** | Manrope | Bold (700) | 40px | −1.2px | tight | `#FFFFFF` | CHF pricing display |
| **Stats Number** | Manrope | Regular (400) | 32px | −0.55px | 33px | `#54DC54` | Counter stats (9, 850m², 200+) |
| **Section Eyebrow** | Manrope | SemiBold (600) | 18px | +1.8px | tight | `#FFFFFF` | "OUR SERVICES" labels (uppercase) |
| **Tag / Location** | Manrope | Regular (400) | 12px | +1.2px | tight | `#888888` | "GENEVA, SWITZERLAND" (uppercase) |
| **Nav Link** | Manrope | Regular (400) | 13px | +0.52px | 19.5px | `#888888` | Navigation items (uppercase) |
| **CTA Button** | Manrope | Regular (400) | 14px | −0.42px | tight | `#000000` | Primary green button text |
| **Outline Button** | Manrope | Regular (400) | 14px | +0.28px | 21px | `#555555` | Secondary outline button |
| **Plan Label** | Manrope | SemiBold (600) | 12px | −0.36px | tight | `#54DC54` | "Community Member" / "Business Member" |
| **Feature Text** | Manrope | Regular (400) | 12px | −0.36px | 1.4 | `rgba(255,255,255,0.5)` | Pricing plan feature items |
| **Image Label** | Manrope | SemiBold (600) | 14px | +1.4px | tight | `#FFFFFF` | Photo overlay labels (uppercase) |
| **Stats Label** | Manrope | Regular (400) | 10px | +1.4px | 15px | `#AAAAAA` | Under-stats captions (uppercase) |
| **Ghost Button** | Arial | Bold (700) | 13px | 0 | normal | `rgba(255,255,255,0.6)` | Dark section "Get Started →" |
| **Price Suffix** | Manrope | Regular (400) | 14px | −0.42px | tight | `rgba(255,255,255,0.35)` | "/year" next to price |

### Typography Rules
- **Uppercase** is used for: nav links, section eyebrows, stats labels, location tags, image overlays — never for body copy
- The hero heading always ends with a green period (`#54DC54`) as a brand signature
- Negative tracking is standard for headings; positive tracking only for uppercase labels
- No decorative or serif fonts — ever
- Body copy line-height is always 1.3–1.6 depending on context

---

## 4. Logo

### Logo Components
- **Wordmark**: "DECENTRAL" + lightning bolt mark + "H" (or full "HOUSE")
- The lightning bolt serves as the brand mark/icon, rendered in `#54DC54` green
- Full lockup: `176px × 28px` at standard size

### Logo Variants

| Variant | Background | Usage |
|---------|------------|-------|
| **Default (dark text + green bolt)** | White / Light | Header, light presentations, social |
| **All-white** | `#121212` / Dark | Dark slides, dark footers |
| **All-black** | `#54DC54` green | Green section headers |

### Logo Usage Rules
- Minimum clear space: equal to the height of the "H" mark on all sides
- Do not recolor, rotate, or add effects to the logo
- Never place the logo on busy photographic backgrounds without a clear overlay
- Render the bolt mark in `#54DC54` whenever possible — it is the brand's most recognizable element

---

## 5. Layout & Spacing

### Grid System
- **Canvas width**: 1440px
- **Container width**: 1280px (centered, 80px padding on each side)
- **Inner content left padding**: 24px (within the 1280px container)
- **Two-column split**: copy column ~589px wide, visual column fills remainder

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-2` | 2px | Micro gaps (price gap) |
| `--space-5` | 5px | Bullet dot size |
| `--space-8` | 8px | Icon + label gap |
| `--space-9` | 9px | Service list item gap |
| `--space-10` | 10px | Indicator + label gap |
| `--space-12` | 12px | Tag internal padding (vertical) |
| `--space-13` | 13px | Ghost button padding |
| `--space-16` | 16px | Heading → description gap |
| `--space-24` | 24px | Button row gap, inner padding |
| `--space-32` | 32px | Card internal padding, nav gap |
| `--space-55` | 55px | Stats items gap |
| `--space-80` | 80px | Container horizontal padding |
| `--space-93` | 93px | Section vertical padding |

### Section Structure
Every scroll section follows this architecture:

```
[Full-width section — 1440px wide × 829px tall]
  ├── Left column (~589px): eyebrow label → headline → body → CTA
  └── Right column (~851px): full-bleed photo or interactive visual
```

For dark/centered sections (e.g. pricing):
```
[Full-width section — 1440px × 829px]
  ├── Centered heading block (top ~200px)
  └── Two pricing cards (side by side, ~300–360px each)
```

---

## 6. Components

### Navigation Bar
```css
height: 73px;
background: rgba(255, 255, 255, 0.90);
border-bottom: 1px solid #E8E8E8;
padding: 0 80px;
display: flex;
align-items: center;
justify-content: space-between;
```
- Logo: left-aligned, 176px × 28px
- Nav links: centered, Manrope Regular 13px, `#888`, uppercase, tracking +0.52px, gap 32px
- CTA button: right-aligned, green compact style

---

### Buttons

#### Primary CTA — Green
```css
background: #54DC54;
color: #000000;
font-family: Manrope, sans-serif;
font-weight: 400;
font-size: 14px;
letter-spacing: -0.42px;
padding: 18px 38px;
border-radius: 0;          /* ← SHARP CORNERS, no radius */
border: none;
```

#### Nav CTA — Green Compact
```css
background: #54DC54;
color: #000000;
font-family: Manrope, sans-serif;
font-weight: 400;
font-size: 13px;
letter-spacing: 0.39px;
padding: 10px 24px;
height: 39.5px;
border-radius: 0;
border: none;
```

#### Secondary — White Outline
```css
background: transparent;
color: #555555;
font-family: Manrope, sans-serif;
font-weight: 400;
font-size: 14px;
letter-spacing: 0.28px;
padding: 15px 33px;
height: 50px;
border: 1px solid #DDDDDD;
border-radius: 0;
```

#### White CTA (on Green Section)
```css
background: #FFFFFF;
color: #000000;
font-family: Manrope, sans-serif;
font-weight: 400;
font-size: 14px;
letter-spacing: -0.42px;
padding: 17px 32px;
border-radius: 0;
border: none;
/* Often includes a small arrow icon (15×15px) */
```

#### Ghost CTA (on Dark Section)
```css
background: transparent;
color: rgba(255, 255, 255, 0.60);
font-family: Arial, sans-serif;
font-weight: 700;
font-size: 13px;
letter-spacing: 0;
padding: 13px;
border: 1px solid rgba(255, 255, 255, 0.15);
border-radius: 0;
width: 100%;
text-align: center;
```

**Critical**: All buttons use `border-radius: 0` — the brand is defined by square, architectural corners.

---

### Pricing Cards (Dark Section)

```css
/* Section background */
background: #121212;

/* Card layout */
display: flex;
flex-direction: column;
gap: 16px;
padding: 32px;
width: ~360px;

/* Price */
font-family: Manrope, sans-serif;
font-weight: 700;
font-size: 40px;
letter-spacing: -1.2px;
color: #FFFFFF;

/* Plan label */
font-weight: 600;
font-size: 12px;
letter-spacing: -0.36px;
color: #54DC54;

/* Description */
font-weight: 400;
font-size: 12px;
letter-spacing: -0.36px;
color: #888888;
line-height: 1.4;

/* Feature list item */
height: 32px;
border-bottom: 1px solid rgba(255,255,255,0.06);
font-size: 12px;
color: rgba(255,255,255,0.5);
letter-spacing: -0.36px;

/* Bullet */
width: 5px; height: 5px;
border-radius: 2.5px;
background: #54DC54;
```

---

### Section Eyebrow / Label
```css
font-family: Manrope, sans-serif;
font-weight: 600;
font-size: 18px;
letter-spacing: 1.8px;
text-transform: uppercase;
color: #FFFFFF;           /* on green/dark sections */
/* or */
color: #888888;           /* on light sections */
font-size: 12px;
letter-spacing: 1.2px;
```

---

### Stats Block
```css
display: flex;
gap: 55px;
align-items: center;

/* Number */
font-family: Manrope;
font-weight: 400;
font-size: 32px;
letter-spacing: -0.55px;
line-height: 33px;
color: #54DC54;

/* Label */
font-size: 10px;
letter-spacing: 1.4px;
text-transform: uppercase;
color: #AAAAAA;
line-height: 15px;
```

---

### Service List (Green Section)
```css
/* Active item (large) */
font-family: Manrope;
font-weight: 600;
font-size: 48px;
letter-spacing: -1.44px;
line-height: 0.95;
color: #FFFFFF;
/* Preceded by a vertical bar indicator (~10.5×16px) */

/* Inactive items */
font-family: Manrope;
font-weight: 400;
font-size: 17.5px;
letter-spacing: -0.525px;
line-height: 1.3;
color: rgba(255, 255, 255, 0.50);
gap-between-items: 9px;
```

---

### Image Overlays
Text labels placed over photos in the hero:
```css
font-family: Manrope;
font-weight: 600;
font-size: 14px;
letter-spacing: 1.4px;
text-transform: uppercase;
color: #FFFFFF;
/* Positioned at bottom-right of each photo tile */
```

---

### Photo Sections
- Photos are used as large right-column fills (851px+ wide)
- Diagonal/angled masks cut across sections for dynamism
- Never use photos as decorative backgrounds with text on top unless there's a clear overlay
- People-focused photography: genuine community moments, workspace, events

---

## 7. Iconography

### Icon System
- Small inline icons: SVG, ~13–15px
- The lightning bolt in the logo is the primary brand icon
- Arrow icons (→) used in "Learn More" / "Get Started" buttons
- Location pin icon for "Geneva, Switzerland" tag (~13×13px)

### Icon Colors
- On light backgrounds: `#888` or `#54DC54`
- On green backgrounds: white
- On dark backgrounds: white or `#54DC54`

---

## 8. Photography & Visual Style

### Photography Tone
- Warm, candid, human-centered — people shaking hands, networking, collaborating
- Architectural/spatial shots for workspace interiors (natural light, modern finishes)
- Aerial/city shots for location context (Geneva rooftops)
- Never stock-photo looking; always authentic community feel

### Layout Technique — Diagonal Cuts
Sections use angled image masking (parallelogram clips) to create visual momentum:
```css
/* Example: hero right column */
clip-path: polygon(10% 0%, 100% 0%, 100% 100%, 0% 100%);
/* Adjust percentages to match the ~10° angle seen in the design */
```

### Image Treatment
- Photos appear with overlaid text labels (service names) in uppercase Manrope SemiBold
- No heavy filters or color grading — photos stay natural
- Grid of 2–4 photos is used in the hero: one large vertical + supporting smaller tiles

---

## 9. Motion & Animation

### Scroll Sections
- Page is structured as full-viewport-height scroll sections (each 829px)
- Sections should animate in sequentially on scroll
- Suggested: fade-up or translate-Y reveals, 0.4–0.6s ease-out

### Service Carousel
- The green section cycles through services; active one is large (48px), inactive ones shrink to 17.5px / 50% opacity
- Transition: smooth scale + opacity, ~0.3s ease

### Stats Counter
- Numbers (`9`, `850m²`, `200+`) should count up on entrance — reinforces data credibility
- Duration: ~1.2s per counter, ease-out

### Hover States
- Buttons: slight opacity reduction (0.85) or slight scale (1.02)
- Nav links: color shift from `#888` to `#1A1A1A`
- All transitions: `0.2s ease`

---

## 10. Section-by-Section Reference

### Hero Section (Light)
- Surface: white `#FFFFFF`
- Left: location tag → H1 (72px) → body text → button row → stats bar
- Right: 2-column photo grid with diagonal cuts and service labels
- Background: white, no pattern

### Events & Venue Rental Section (Green)
- Surface: `#54DC54` full-bleed
- Left: eyebrow → service list (active + inactive) → body text → white CTA button
- Right: full-bleed photograph (851px wide)
- Diagonal split at ~30% from right

### Community / Join Section (Light)
- Surface: white `#FFFFFF`
- Typically: left copy + right stats/photo grid
- Similar layout pattern to hero

### Community Membership Section (Dark)
- Surface: `#121212`
- Centered heading (56px) + description
- Two pricing cards side by side with a photo card between them
- Ghost CTAs at card bottom

### Event Calendar Section (Light)
- Surface: white
- List-based layout with dates and event names

### Testimonials Section (Light)
- Quote blocks with attribution
- Quote mark in `#54DC54`

### Footer (Dark)
- Surface: `#121212` or near-black
- Logo mark + nav links + social icons
- Copyright in muted white opacity text

---

## 11. Voice & Messaging

### Tone
- **Confident and precise** — Geneva's best, not just "a" coworking space
- **Community-first** — "Join Geneva's Most Connected Innovation Community"
- **Numbers-forward** — lead with 9 suites, 850m², 200+ members
- **Inclusive to tech ecosystem** — AI, FinTech, Web3 — not generic startup language

### Key Messages
1. "The Premier Innovation Hub in Geneva"
2. "A strategic base for AI, FinTech, and Web3 pioneers"
3. "Join Geneva's Most Connected Innovation Community"
4. "Private Offices, Co-working, World-class Events, and a thriving community of innovators"

### Messaging Hierarchy
| Level | Example |
|-------|---------|
| **Hero headline** | "The Premier Innovation Hub in Geneva." |
| **Section headline** | "Join Geneva's Most Connected Innovation Community." |
| **Body copy** | "Host innovation summits, workshops, and networking events. Professional AV, catering partners, and modular configurations up to 120 guests." |
| **CTA** | "Explore Our Services" / "Become a Member" / "Learn More →" |
| **Stat** | "200+ Members" / "850m² Total Space" |

### CTA Copy Patterns
- Primary CTA: Active verb + object — "Explore Our Services", "Become a Member"
- Secondary CTA: Community language — "Join the Community"
- Section CTA: Informational — "Learn More →", "Get Started →"

---

## 12. AI Agent Usage Guide

### Do
- Use **Manrope** for all text — every size, every weight
- Keep buttons **perfectly square** (border-radius: 0) — this is a signature of the brand
- Use `#54DC54` green as the **only** accent color
- Build layouts at **1440px canvas**, 1280px content container
- Use **three surfaces only**: white, green (`#54DC54`), dark (`#121212`)
- End hero headlines with a green period as a brand flourish
- Use **uppercase + positive tracking** for labels, eyebrows, and nav
- Use **negative tracking** for headings and buttons
- Prioritize **people photography** — events, connection, workspace

### Don't
- Don't add border-radius to buttons or cards (except 2.5px on bullet dots)
- Don't introduce colors outside the defined palette
- Don't use bold weight for body text
- Don't place the logo on busy photographic backgrounds without a backing
- Don't use rounded or pill-shaped buttons
- Don't use gradients for text
- Don't use more than one accent color per layout

---

### Slide Decks (16:9 — 1920×1080px)
- **Dark slides**: `#121212` background, white headings (56px+), `#54DC54` accents
- **Light slides**: white background, `#1A1A1A` headings, `#777` body
- **Green slides**: `#54DC54` background, white text — use for section dividers / impact moments
- Body text: Manrope Regular 18–22px, `#777` on light / white on dark
- Data/stats: Manrope Regular, stat in `#54DC54`, label in `#AAA` uppercase
- All layout elements flush to guides — no floating elements

### Landing Pages / Sub-pages
- Follow the scroll-section architecture (each section ~829px tall at desktop)
- Always begin with a hero on white, then alternate green/dark sections for rhythm
- Max content width: 1280px inside 1440px canvas
- Mobile: collapse two-column layouts to single column; maintain all type scale ratios

### Social Media Visuals
- **Square (1080×1080)**: headline-first, minimal. Green or dark background.
- **Story (1080×1920)**: large stat or quote centered, logo top or bottom
- Always include the Decentral House wordmark + bolt mark
- Keep body copy under 12 words for social headers
- Use the green period punctuation on social headlines where possible

### Animations & Motion Graphics
- Brand green flash on entrance: logo bolt animates in with a quick pulse of `#54DC54`
- Stat counters roll up from 0 to final value
- Section transitions: fade-up, 0.4s ease-out, stagger between elements
- Service selector: smooth cross-fade between active/inactive states
- Never use bouncy or playful easing — keep physics sharp and Swiss

---

## 13. Design Token Quick Reference

```css
/* === COLORS === */
--green:           #54DC54;
--black:           #1A1A1A;
--dark:            #121212;
--white:           #FFFFFF;
--gray-88:         #888888;
--gray-77:         #777777;
--gray-55:         #555555;
--gray-aa:         #AAAAAA;
--border:          #DDDDDD;
--border-header:   #E8E8E8;

/* White opacity (dark surfaces) */
--white-06:  rgba(255,255,255,0.06);
--white-15:  rgba(255,255,255,0.15);
--white-35:  rgba(255,255,255,0.35);
--white-50:  rgba(255,255,255,0.50);
--white-60:  rgba(255,255,255,0.60);

/* === TYPOGRAPHY === */
--font-primary:    'Manrope', sans-serif;
--font-secondary:  'Arial', sans-serif;

/* === SIZING === */
--canvas:          1440px;
--container:       1280px;
--section-height:  829px;
--header-height:   73px;

/* === SPACING === */
--space-8:   8px;
--space-16:  16px;
--space-24:  24px;
--space-32:  32px;
--space-55:  55px;
--space-80:  80px;
--space-93:  93px;
```

---

*Source: Figma file `zjQsGcu1HnRDzdUJxeOFSP`, node `Decentral House (2043:98)` — extracted April 2026. Always defer to the live Figma file for pixel-perfect specifications.*