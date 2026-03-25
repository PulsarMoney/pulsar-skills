# Acc Ventures — Design System
> Reference document for AI agents building on-brand presentations, websites, and digital assets for Acc Ventures / Astrarizon.

---

## 1. Brand Identity

**Company:** Acc Ventures
**Parent company:** Astrarizon
**Tagline / positioning:** "Seeking Protagonists." — A research-driven crypto investment firm (founded 2017). Strategic partners for founders, offering collaborative investing, operational experience, distribution, and strategic partnerships.
**Sub-brands:** Acc Ventures (VC), Acc Labs (venture builder), Acc Podcast, Acc Ecosystem.

---

## 2. Logo & Wordmark

### Primary wordmark
- **Acc.Ventures** — written with a period between "Acc" and "Ventures"
- Typeset in **Geist Mono** (monospace), weight Regular
- Displayed in `#f5f5f5` (off-white) on dark backgrounds
- Sub-caption beneath logo: `AN ASTRARIZON COMPANY` in `#adadad`, Geist Mono Regular, 12px, uppercase

### Monogram / icon mark
- **`/Acc`** navigation device — a forward slash `/` in `#ff4f00` (brand orange) followed by the section name in `#f5f5f5`, typeset in **DM Sans**, 24–36px, tracking `-1.68px` to `-2.52px`, line-height `0.9`
- Used as both a logo variant and persistent navigation element

### Logomark (icon)
- Angular, spoked radial graphic (resembling a starburst / compass rose) — used on light and dark backgrounds
- On dark backgrounds: white/light version
- On white backgrounds: dark version

### Brand graphic — triple slash `/Acc`
- Three parallel diagonal lines in `#ff4f00`, used as a standalone decorative brand mark and divider

### Usage rules
- Never stretch or distort the wordmark
- Maintain clear space around the logo equal to the height of the "A" in Acc
- Preferred background: `#0d0d0d` (near black)

---

## 3. Colour Palette

### Primary colours

| Name | Hex | Usage |
|------|-----|-------|
| **Acc Black** | `#0d0d0d` | Primary background (all screens and slides) |
| **Acc Orange** | `#ff4f00` | Primary accent — CTAs, highlights, active states, slash marks |
| **Acc White** | `#f5f5f5` | Primary text and foreground elements |

### Secondary colours

| Name | Hex | Usage |
|------|-----|-------|
| **Off-white** | `#f7f7f7` | Body text, card foreground |
| **Near black** | `#1a1a1a` | Button text on light backgrounds, dark card overlays |
| **Deep charcoal** | `#2c2c2c` | Subtle dividers, graphic fills |
| **Mid grey** | `#898989` | Secondary body text, captions, metadata |
| **Dim grey** | `#adadad` | Sub-captions (e.g. "AN ASTRARIZON COMPANY") |
| **Muted grey** | `#545454` | Footer / legal text |
| **Light grey** | `#d9d9d9` | Neutral label chips on dark backgrounds |

### Accent / semantic

| Name | Hex | Usage |
|------|-----|-------|
| **Burnt orange (dark bg card)** | `#310` (`#331100`) | Portfolio card background for featured/active companies (e.g. Linera) |
| **Translucent white** | `rgba(245,245,245,0.2)` | Ghost/secondary buttons and translucent labels |

### Gradient (media overlay)
Used on podcast thumbnails and video cards:
```
linear-gradient(-61.46deg, #1a1a1a 0%, #ff4f00 100%)
blend-mode: color
```
This applies an orange colour cast to photo/video imagery, reinforcing brand identity.

---

## 4. Typography

### Font families

| Font | Role | Style | Source |
|------|------|-------|--------|
| **DM Sans** | Display / Headings | Variable, Regular, `'opsz' 14` | Google Fonts |
| **Geist Mono** | Body / UI / Labels | Regular, Medium | Vercel / Google Fonts |
| **Clash Grotesk** | Partner logos / co-brand | Medium | fontshare.com |
| **Font Awesome 6 Brands** | Social icons (LinkedIn, Telegram, X) | Regular | fontawesome.com |

### Type scale

| Role | Font | Size | Weight | Tracking | Line-height |
|------|------|------|--------|----------|-------------|
| **Hero / page title** | DM Sans | 36px | Regular | `-2.52px` | `0.9` |
| **Section heading** | DM Sans | 24px | Regular | `-1.68px` | `0.9` |
| **Sub-heading** | DM Sans | 22–24px | Regular | `-1.56px` | `0.9` |
| **Body / description** | Geist Mono | 12px | Regular | — | `1.2` |
| **Label / badge** | Geist Mono | 12px | Regular | `1.2px` | `1` |
| **Tag / category** | Geist Mono | 10px | Medium | `1px` | `15.262px` |
| **Footer / legal** | Geist Mono | 12px | Regular | `1.2px` | `1.5` |

### Typography rules
- **All caps** is used extensively for labels, badges, nav items, and CTAs — this is a core brand pattern
- **Letter-spacing:** Uppercase text always uses positive tracking (`1px`–`1.6px`); display text uses negative tracking
- **DM Sans** is exclusively for large-scale display text (headings, hero copy)
- **Geist Mono** is used for everything functional: body copy, UI labels, buttons, captions, navigation
- Headings frequently mix orange `/` accents with white text using `text-[0px]` span tricks to blend colours in a single paragraph

---

## 5. Layout & Spacing

### Grid
- **Canvas width:** 1440px (desktop)
- **Horizontal padding:** `24px` on each side
- **Inner content width:** `1392px`
- **Column structure:** Roughly 12-column equivalent with spacings of `24px` gaps

### Spacing scale (extracted from components)
| Token | Value | Usage |
|-------|-------|-------|
| `2px` | 2px | Tight element gaps |
| `4px` | 4px | Internal chip padding |
| `8px` | 8px | Button padding, card internal padding |
| `12px` | 12px | Button horizontal padding |
| `16px` | 16px | Section sub-gaps, card content gaps |
| `24px` | 24px | Column gutters, section internal padding |
| `32px` | 32px | Content block gaps |
| `40px` | 40px | Large section gaps |
| `80px` | 80px | Section vertical padding |

### Border-radius
- `1px` — buttons, labels, chips, card corners (sharp, almost square)
- `4px` — portfolio cards, image containers (slightly softened)
- `12802539px` (effectively `9999px`) — status dot indicators (fully round)

---

## 6. Components

### 6.1 Labels / Chips
Small badge elements used for categories, statuses, and CTAs.

**Variant: Orange (primary action)**
```
Background: #ff4f00
Text: #f5f5f5 or #1a1a1a
Font: Geist Mono Regular, 12px, uppercase, tracking 1.2px
Padding: 4px 8px
Border-radius: 1px
```
Example: `VENTURE STUDIO →`, `LINERA →`

**Variant: Light (neutral)**
```
Background: #f5f5f5 or #d9d9d9
Text: #1a1a1a
Font: Geist Mono Regular, 12px, uppercase, tracking 1.2px
Padding: 4px 8px
Border-radius: 1px
```
Example: `VENTURE CAPITAL`, `PI SQUARED`, `ALEX RADU`

**Variant: Ghost (translucent)**
```
Background: rgba(245,245,245,0.2)
Text: #f5f5f5
Font: Geist Mono Regular, 12px, tracking 1.2px
Padding: 4px 6px
Border-radius: 1px
```
Example: `→` arrow navigation links

### 6.2 Buttons

**Primary button (dark bg)**
```
Background: #f5f5f5
Text: #1a1a1a
Font: Geist Mono Medium, 12px, uppercase, tracking 1.2px
Padding: 8px 12px
Height: 32px
Border-radius: 1px
```
Example: `APPLY TODAY`, `DISCOVER FULL TEAM →`

**Primary button (CTA orange)**
```
Background: #ff4f00
Text: #1a1a1a
Font: Geist Mono Medium, 12px, uppercase, tracking 1.2px
Padding: 8px 12px
Height: 32px
Border-radius: 1px
```
Example: `APPLY TODAY` (on footer CTA)

**Status/alert banner**
```
Border: 1px solid #ff4f00
Background: transparent
Text: #ff4f00
Font: Geist Mono Medium, 10px, uppercase, tracking 1px
Leading dot: 6px circle, #ff4f00, opacity 90%
Padding: 8px
Border-radius: 1px
```
Example: `● $5,3M IN FUNDING ROUND OPEN`

### 6.3 Portfolio / Content Cards

**Featured card (highlighted)**
```
Background: #310 (dark burnt orange)
Border-radius: 1px
Padding: 4px
Height: 400px
Width: 448px
Top section: category tag (left) + date tag (right)
Middle: centered company logo on brand-tinted background
Bottom: orange label chip + description text (Geist Mono Regular, 12px, #f7f7f7)
```

**Standard card (outlined)**
```
Background: transparent
Border: 1px dashed #f5f5f5
Border-radius: 1px
Padding: 4px
Height: 400px
Width: 448px
Same layout as featured card; label chip uses #d9d9d9 background
Description text: #898989
```

**Team / person card**
```
Background: #f5f5f5 (photo fills card)
Border-radius: 4px
Height: 332px
Width: 333px
Photo: black & white, full-bleed
Bottom info bar (outside card):
  - Name chip: #d9d9d9 background, Geist Mono 12px, #1a1a1a
  - Social icons: LinkedIn, Telegram, X — Font Awesome 6 Brands, 15px, #898989
  - Role text: Geist Mono Regular, 12px, #898989
```

**Blog / article list item**
```
Border-bottom: 1px dashed #f7f7f7
Padding-bottom: 24px
Title: DM Sans Regular, 24px, #f5f5f5, tracking -1.68px, line-height 0.9
Description: Geist Mono Regular, 12px, #898989, line-height 1.2
Arrow CTA: Ghost label chip →
```

**Podcast / video thumbnail card**
```
Image with color overlay gradient: linear-gradient(-61.46deg, #1a1a1a 0%, #ff4f00 100%), blend-mode: color
Border-bottom: 6px solid #ff4f00
Play button icon centered over image
Title: DM Sans Regular, 24px, #f5f5f5
Platform label: neutral label chip (e.g. YOUTUBE)
```

### 6.4 Navigation

The `/Acc` navigation system uses a persistent left-side nav component on each page section:

```
Font: DM Sans Regular
Size: 24px
Tracking: -1.68px
Line-height: 0.9
Active item: full opacity, white #f5f5f5
Inactive items: opacity 20%, white

Prefix slash "/" : color #ff4f00
"Acc" text: color #f5f5f5

Example active: "/Acc Portfolio"
          dimmed siblings: "Ecosystem", "Blog", "Podcast", "Team"
```

Top navigation bar (footer/CTA sections):
```
Font: Geist Mono Regular, 12px, uppercase, tracking 1.2px
Color: #f7f7f7
Background: #0d0d0d
Items: ABOUT, ECOSYSTEM, PORTFOLIO, BLOG, TEAM
```

---

## 7. Imagery & Media Style

### Photography
- **Black and white** portrait photography for team members
- High contrast, cropped tightly to face/upper body
- Backgrounds are neutral or dark

### Podcast / video thumbnails
- Full-colour source images with brand gradient overlay applied via CSS `mix-blend-mode: color`
- Gradient: `linear-gradient(-61.46deg, #1a1a1a 0%, #ff4f00 100%)`
- Creates a dark-to-orange tint that unifies all media imagery

### Decorative graphics
- **Triple diagonal slash `///`** — orange lines (`#ff4f00`), used as a brand motif
- **Spoked starburst / compass rose** — the Acc icon mark, used large and ghosted as a background element
- **Connecting line graphics** — thin dotted/dashed lines with dot endpoints, used to illustrate ecosystem relationships (VC → Venture Studio → Acc Labs)
- **Large watermark text** — "Acc.Ventures" at very large scale (opacity ~15%) as a background element on the footer/CTA section

---

## 8. Tone of Voice & Copy Style

- **Bold, terse, and technical** — copy reads like it's for sophisticated crypto founders, not consumers
- **Uppercase for all UI text** — buttons, labels, navigation, and metadata always ALL CAPS
- **First-person plural** — "We strive to be strategic partners…", "We support founders…"
- **Founder-centric messaging** — "Seeking Protagonists.", "Andurance in the game"
- **Section titles use the `/Acc` format** — e.g. `/Acc Portfolio`, `/Acc Blog`, `/Acc Team`
- **Dates and metadata** are always shown on cards (e.g. `DEC 2025`)
- **Funding headline format:** `$X,XM IN FUNDING ROUND OPEN` (Geist Mono Medium, 10px, orange)

---

## 9. Section Templates

### Hero / Above the fold
```
Background: #0d0d0d
Left: /Acc logo wordmark + "AN ASTRARIZON COMPANY" caption + triple-slash graphic
Right: Body copy in Geist Mono, 16px, #f5f5f5, tracking 1.6px, uppercase
Accent cursor: | in #ff4f00 at end of body text
```

### About / Mission section
```
Background: #0d0d0d
Left (25% col): /Acc nav device
Center-left: Body paragraph (Geist Mono 12px, #898989, line-height 1.2)
Center: /Acc monogram large icon with connecting line diagram
Right: Entity card (Venture Studio) with icon + label chip + description + portfolio logos
Bottom-left: VENTURE CAPITAL entity with label + description
Bottom-center-right: ACC LABS entity with label + description
```

### Portfolio grid
```
Background: #0d0d0d
Header row: /Acc nav + funding status banner + APPLY TODAY button
Cards: 3-column grid, 448px wide, 400px tall
Card spacing: 24px gap
```

### Blog section
```
Background: #0d0d0d
Left half: Article list with dashed-border rows
Right half: Featured article with image card
```

### Podcast section
```
Background: #0d0d0d
Left: Large featured episode card with gradient image + bottom-border orange
Right: 2×2 grid of smaller podcast cards
```

### Team section
```
Background: #0d0d0d
Left: /Acc Team heading + description text
Cards: Horizontal scroll or grid of 333px-wide portrait cards
CTA button top-right: DISCOVER FULL TEAM →
```

### Footer / CTA
```
Background: #0d0d0d
Center: "Seeking Protagonists." (DM Sans 36px) + "$X,XM IN FUNDING ROUND OPEN" (Geist Mono 10px, orange) + APPLY TODAY button (orange)
Nav: ABOUT / ECOSYSTEM / PORTFOLIO / BLOG / TEAM (Geist Mono, uppercase, top)
Large watermark: "Acc.Ventures" in DM Sans, very large, low opacity ~15%, bottom
Legal: "2026 ACC VENTURES - AN ASTRARIZON COMPANY. ALL RIGHTS RESERVED." (Geist Mono 12px, #545454)
```

---

## 10. CSS Custom Properties (Design Tokens)

```css
:root {
  /* Colours */
  --color-bg-primary:         #0d0d0d;
  --color-bg-dark:            #1a1a1a;
  --color-bg-card-featured:   #310;        /* burnt orange dark */
  --color-bg-charcoal:        #2c2c2c;

  --color-accent-orange:      #ff4f00;
  --color-accent-orange-dim:  rgba(255, 79, 0, 0.9);

  --color-text-primary:       #f5f5f5;
  --color-text-secondary:     #f7f7f7;
  --color-text-muted:         #898989;
  --color-text-dim:           #adadad;
  --color-text-footer:        #545454;
  --color-text-dark:          #1a1a1a;

  --color-border-dashed:      #f5f5f5;     /* for dashed outlines */
  --color-label-neutral:      #d9d9d9;
  --color-ghost-bg:           rgba(245, 245, 245, 0.2);

  /* Typography */
  --font-display:             'DM Sans', sans-serif;
  --font-mono:                'Geist Mono', monospace;
  --font-brand:               'Clash Grotesk', sans-serif;
  --font-icons:               'Font Awesome 6 Brands';

  --text-hero:                36px;
  --text-heading:             24px;
  --text-subheading:          22px;
  --text-body:                12px;
  --text-label:               12px;
  --text-tag:                 10px;

  --tracking-display:         -2.52px;
  --tracking-heading:         -1.68px;
  --tracking-label:           1.2px;
  --tracking-tag:             1px;
  --tracking-body-upper:      1.6px;

  --leading-display:          0.9;
  --leading-body:             1.2;
  --leading-legal:            1.5;

  /* Spacing */
  --space-1:                  2px;
  --space-2:                  4px;
  --space-3:                  8px;
  --space-4:                  12px;
  --space-5:                  16px;
  --space-6:                  24px;
  --space-7:                  32px;
  --space-8:                  40px;
  --space-9:                  80px;

  /* Borders */
  --radius-sharp:             1px;
  --radius-soft:              4px;
  --radius-full:              9999px;

  /* Layout */
  --canvas-width:             1440px;
  --content-width:            1392px;
  --canvas-padding:           24px;
  --col-gap:                  24px;

  /* Media */
  --gradient-brand-overlay:   linear-gradient(-61.46deg, #1a1a1a 0%, #ff4f00 100%);
}
```

---

## 11. Tailwind Config Reference

If using Tailwind CSS, extend the config as follows:

```js
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        'acc-black':    '#0d0d0d',
        'acc-dark':     '#1a1a1a',
        'acc-charcoal': '#2c2c2c',
        'acc-orange':   '#ff4f00',
        'acc-white':    '#f5f5f5',
        'acc-off-white':'#f7f7f7',
        'acc-grey':     '#898989',
        'acc-dim':      '#adadad',
        'acc-muted':    '#545454',
        'acc-neutral':  '#d9d9d9',
        'acc-featured': '#310',
      },
      fontFamily: {
        display: ['"DM Sans"', 'sans-serif'],
        mono:    ['"Geist Mono"', 'monospace'],
        brand:   ['"Clash Grotesk"', 'sans-serif'],
      },
      letterSpacing: {
        'display':  '-2.52px',
        'heading':  '-1.68px',
        'label':    '1.2px',
        'tag':      '1px',
        'wide':     '1.6px',
      },
      lineHeight: {
        'display': '0.9',
        'tight':   '1.2',
        'legal':   '1.5',
      },
      borderRadius: {
        'sharp': '1px',
        'soft':  '4px',
      },
    },
  },
}
```

---

## 12. Key Do's and Don'ts

### Do's
- ✅ Use `#0d0d0d` as the default background for all surfaces
- ✅ Use `#ff4f00` exclusively for primary CTAs, active states, and the `/` accent
- ✅ Write all UI text (buttons, labels, nav) in **ALL CAPS** with Geist Mono
- ✅ Use DM Sans for large display headings only
- ✅ Use the `/Acc [Section]` pattern for all section titles
- ✅ Apply the brand gradient overlay (`mix-blend-mode: color`) to all photography and video thumbnails
- ✅ Use `border-dashed` with `#f5f5f5` for outlined/inactive card states
- ✅ Use `1px` border-radius for all interactive elements (sharp, purposeful)
- ✅ Apply negative letter-spacing (`-1.68px` to `-2.52px`) to all DM Sans display text
- ✅ Use positive letter-spacing (`1px`–`1.6px`) to all Geist Mono uppercase text
- ✅ Convert team photography to black & white

### Don'ts
- ❌ Do not use white (`#ffffff`) — always use `#f5f5f5` or `#f7f7f7`
- ❌ Do not use pure black (`#000000`) — always use `#0d0d0d`
- ❌ Do not use rounded corners (`>4px`) on interactive elements
- ❌ Do not use DM Sans for body text or labels
- ❌ Do not use Geist Mono for large display headings
- ❌ Do not use color photography without the brand gradient overlay
- ❌ Do not use any colours outside the defined palette
- ❌ Do not use lowercase for button or label text
- ❌ Do not place the logo on any background other than `#0d0d0d` or pure white without testing contrast

---

## 13. Presentation Slide Rules

When building Acc Ventures presentations:

- **Slide background:** Always `#0d0d0d`
- **Slide title:** DM Sans, 36px, `#f5f5f5`, tracking `-2.52px`, prefixed with `/ ` in orange
- **Body text:** Geist Mono, 12–16px, `#898989` (secondary) or `#f5f5f5` (primary)
- **Data labels / callouts:** Orange chip label `#ff4f00`, Geist Mono Medium 10–12px, ALL CAPS
- **Dividers:** 1px dashed `#f5f5f5` or thin solid `#2c2c2c`
- **Charts:** Use `#ff4f00` as primary data colour, `#f5f5f5` as secondary
- **Footer:** Geist Mono 12px, `#545454`, "ACC VENTURES — AN ASTRARIZON COMPANY"
- **Slide number / metadata:** Geist Mono 10px, `#545454`, top-right

---

*Last updated: March 2026 — extracted from Figma file `pf8r0P5h5xktlhsPDWfN5E` (Brand Identity + Landing Page)*
