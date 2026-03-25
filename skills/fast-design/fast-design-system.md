# FAST Design System
> A reference guide for AI agents building on-brand presentations, websites, and visual assets for **Fast** — the payment layer for the agentic economy.

---

## 1. Brand Overview

**Fast** is the payment layer for the agentic economy. Built by Pi² Labs, Fast enables billions of AI agents to move money globally and securely at internet speed.

### One-Sentence Description
> Fast is a payment layer that enables billions of AI agents to move money globally and securely at internet speed.

### Boilerplate (Short)
> Fast is the payment layer for the agentic economy. Billions of AI agents are already transacting at machine speed—booking services, paying for compute, settling microtransactions in real time. That future needs a payment layer built for agents, not humans. That layer is Fast. 200K+ TPS. Sub-100ms finality. Formally verified. Learn more at **fast.xyz**

### Key Stats
- 200,000+ TPS (transactions per second)
- Sub-100ms finality
- Formally verified
- Website: fast.xyz

### Name Usage
- Always refer to the company as **"Fast"** or **"Fast by Pi² Labs"**
- The logo should be instantly recognizable in all contexts and sizes
- When referring to the parent company, use **Pi² Labs** or **Pi Labs**

---

## 2. Color Palette

The core palette is minimal, precise, and built for clarity. Use it consistently across all brand touchpoints.

### Primary Colors

| Name         | Hex       | Usage                                                   |
|--------------|-----------|---------------------------------------------------------|
| **Dark**     | `#0D0F13` | Primary backgrounds (dark mode), deep contrast          |
| **Text Dark**| `#2B2C2F` | Primary text, UI elements, dark containers              |
| **Brand**    | `#A1B0CF` | Accent color, CTAs, interactive elements (use sparingly)|
| **Text**     | `#5F6672` | Body text, secondary labels, muted elements             |
| **Border**   | `#E9EBF0` | Light backgrounds, borders, section dividers            |
| **Light**    | `#F6F8FA` | Page backgrounds, light surfaces, button text on dark   |

### CSS Custom Properties
```css
:root {
  --color-dark:       #0D0F13;
  --color-text-dark:  #2B2C2F;
  --color-brand:      #A1B0CF;
  --color-text:       #5F6672;
  --color-border:     #E9EBF0;
  --color-light:      #F6F8FA;
}
```

### Color Usage Rules
- **Dark (#0D0F13)** — Use for full-bleed dark section backgrounds and dark logo variant backgrounds
- **Text Dark (#2B2C2F)** — Use for all headings, nav items, buttons, and primary body copy
- **Brand (#A1B0CF)** — Reserved for accent moments: links in boilerplate, hover states, and interactive highlights. Use sparingly.
- **Text (#5F6672)** — Default body text, subheadings, form labels, footer text
- **Border/Light (#E9EBF0 / #F6F8FA)** — Page backgrounds, cards, dividers, button backgrounds in light contexts

### Dark Overlays & Gradients
Fast uses subtle gradient overlays on buttons and containers for depth:
```css
/* Primary dark button gradient */
background-image:
  linear-gradient(242deg, rgba(246,248,250,0.25) 49.7%, rgba(200,207,216,0.25) 14.7%, rgba(227,229,234,0.25) 18%, rgba(246,248,250,0.25) 43.1%, rgba(222,227,232,0.25) 77.3%),
  linear-gradient(180deg, rgba(95,102,114,0.05) 0%, rgba(95,102,114,0) 100%),
  linear-gradient(90deg, #2B2C2F 0%, #2B2C2F 100%);

/* Light button / card gradient */
background-image:
  linear-gradient(256deg, rgba(246,248,250,0.25) 0%, rgba(200,207,216,0.25) 0%, rgba(227,229,234,0.25) 18%, rgba(246,248,250,0.25) 43.1%, rgba(222,227,232,0.25) 77.3%),
  linear-gradient(180deg, rgba(95,102,114,0) 0%, rgba(95,102,114,0.05) 100%),
  linear-gradient(90deg, #F6F8FA 0%, #F6F8FA 100%);
```

### Dividers
- **Horizontal dividers** — `rgba(0,0,0,0.05)`, 1px tall, full width or 1174px within the content column
- **Vertical dividers** — `rgba(0,0,0,0.05)`, 2px wide, 16px tall

---

## 3. Typography

Fast uses two primary typefaces: **General Sans Variable** for headings and brand text, and **Inter** for UI labels, download text, and secondary copy.

### Typefaces

| Font                        | Role                              | Notes                              |
|-----------------------------|-----------------------------------|------------------------------------|
| **General Sans Variable**   | Primary brand font                | Headlines, nav, buttons, body copy |
| **Inter**                   | Secondary / UI font               | Labels, captions, footer links     |
| **Font Awesome 6 Pro**      | Icon font                         | Nav chevrons and UI icons          |

### Type Scale

| Style          | Font                            | Weight    | Size        | Line Height   | Tracking          |
|----------------|---------------------------------|-----------|-------------|---------------|-------------------|
| **H1 / Hero**  | General Sans Variable           | Medium    | ~70–70.5px  | 68.4px        | –                 |
| **H2 / Section**| General Sans Variable          | Medium    | 36px        | 1.1 (39.6px)  | –1.8px            |
| **H3 / Name**  | Inter                           | Regular   | ~27px       | 42px          | –0.7px            |
| **H3 / Title** | Inter                           | Regular   | ~19px       | 30px          | –1px              |
| **Body**       | General Sans Variable           | Regular   | 16px        | 1.3 (20.8px)  | –0.16px           |
| **Nav**        | General Sans Variable           | Regular   | 14px        | 20px          | –0.42px           |
| **CTA Button** | General Sans Variable           | Medium    | 16px        | ~0.92         | –0.48px           |
| **Label / Tag**| General Sans Variable           | Semibold  | 12px        | 1.3           | +0.36px uppercase |
| **Button Tag** | Inter                           | Medium    | 14px        | 20px          | –0.35px uppercase |
| **Footer Link**| Inter                           | Regular   | ~13–14px    | 20px          | –                 |
| **Copyright**  | Inter                           | Regular   | ~13px       | 20px          | –                 |

### Typography Rules
- Hero headings use **General Sans Variable Medium**, very large (~70px), tight to the page
- Section headings use **General Sans Variable Medium at 36px**, tracking –1.8px
- Body copy uses **General Sans Variable Regular at 16px**, line-height 1.3, tracking –0.16px
- Section labels (e.g., "Brand Assets", "Founder Bios") are **uppercase, Semibold, 12px, tracking +0.36px, opacity 0.8**
- Download/format buttons use **Inter Medium, uppercase, 14px** on dark pill buttons
- Footer category labels are **uppercase, ~12px, opacity 0.3**

---

## 4. Logo

### Logo Variants
| Variant        | Background   | Use Case                                     |
|----------------|--------------|----------------------------------------------|
| **Dark logo**  | White/Light  | Light backgrounds, presentations, web        |
| **Light logo** | `#0D0F13`    | Dark backgrounds, dark slides, dark UI       |

### Logo Clear Space
- Maintain clear space around the logo equal to the **height of the "F" mark**
- Nothing should break the limit of this clear space
- The logo consists of four letterforms: **F**, **A**, **S**, **T**

### Logo Usage Rules
- Only use approved logo files (SVG preferred, PNG for raster contexts)
- Do not recolor, distort, rotate, or add effects to the logo
- When referring to the company in text, use **"Fast"** or **"Fast by Pi² Labs"**
- The footer uses oversized, opacity-reduced individual letter marks (F, A, S, T) as decorative brand elements

---

## 5. Layout & Spacing

### Grid System
- **Canvas width:** 1440px
- **Content column:** 1176px wide (centered, with 1px left/right borders at `rgba(0,0,0,0.05)`)
- **Content padding (horizontal):** 132px each side (1440 – 1176 = 264px total)
- **Inner content padding:** 48px left padding for text blocks within sections

### Spacing Scale (from design)
| Token     | Value  | Usage                              |
|-----------|--------|------------------------------------|
| `xs`      | 2px    | Inner dot indicators               |
| `sm`      | 6px    | Gap between nav icon + label       |
| `md`      | 12px   | Gap between buttons in groups      |
| `lg`      | 16px   | Gap between heading and body text  |
| `xl`      | 24px   | Gap between social icons, sections |
| `2xl`     | 32px   | Content group gaps                 |
| `3xl`     | 48px   | Internal section padding           |
| `4xl`     | 60px   | Section top/bottom padding         |
| `5xl`     | 80px   | Section vertical padding           |

### Section Structure
Each major section follows this pattern:
1. **Horizontal divider** — `rgba(0,0,0,0.05)`, 1px
2. **Section container** — 1176px wide, bordered left/right, `padding: 80px 1px`
3. **Section label row** — uppercase eyebrow label
4. **Content blocks** — heading + body text on left, visual asset on right (or full-width)

---

## 6. Components

### Navigation Bar
- **Height:** 64px
- **Background:** Light (`#F6F8FA`) with gradient overlay
- **Layout:** Logo left | Nav links center | CTA button right
- **Padding:** `px-132px py-2px`
- **Logo:** Left-aligned at 56.7px wide, 20px tall
- **Nav links:** General Sans Regular 14px, tracking –0.42px, color `#2B2C2F`, with chevron-down icons
- **CTA button:** Dark pill (see Button — Primary Dark below)

### Buttons

#### Primary Dark (CTA)
```css
background: linear-gradient(...), #2B2C2F;
border: 0.5px solid rgba(246,248,250,0.15);
border-radius: 90px;
padding: 14px 24px;
font: General Sans Variable Medium, 16px;
color: #F6F8FA;
letter-spacing: -0.48px;
box-shadow: 0px 1px 1px rgba(0,0,0,0.1);
```

#### Secondary Light (Outlined)
```css
background: linear-gradient(...), #F6F8FA;
border: 1px solid #C8CFD8;
border-radius: 999px;
padding: 12.5px 24.5px;
font: General Sans Variable Medium, ~15px;
color: #2B2C2F;
text-shadow: 0px 0.3px 0px rgba(255,255,255,0.49);
letter-spacing: -0.48px;
```

#### Format Tag Button (PNG/SVG/etc.)
```css
background: #2B2C2F;
border-radius: 999px;
padding: 8px 14px;
font: Inter Medium, 14px uppercase;
color: #FFFFFF;
letter-spacing: -0.35px;
```

### Color Swatch Display
- Vertical bars at equal widths, full height container
- Color hex labels at bottom: **Inter Medium, ~12–13px, tracking –0.35px**
- Dark swatches (#0D0F13, #2B2C2F, #5F6672) use **white text**
- Light swatches (#A1B0CF, #E9EBF0) use **#2B2C2F text**

### Logo Display Cards
- **Light variant card:** White background, 1px border `rgba(0,0,0,0.1)`, 180×180px container, logo centered
- **Dark variant card:** `#0D0F13` background, same border, same dimensions
- Below each card: "Download" label + PNG/SVG format buttons

### Section Labels (Eyebrow)
```css
font: General Sans Variable Semibold, 12px uppercase;
letter-spacing: 0.36px;
color: #5F6672;
opacity: 0.8;
```

### Founder Bio Cards
- **Name:** Inter Regular, ~27px, `#2B2C2F`, tracking –0.7px
- **Title:** Inter Regular, ~19px, `#5F6672`, tracking –1px
- **Photo:** Gradient overlay from `#C8CFD8` (top, 3.57%) to `#5F6672` (bottom), 245×285px
- **Social icons:** 24×24px SVGs, spaced 24px apart (X, LinkedIn, GitHub, Google Scholar, Wikipedia)

### Horizontal Dividers
```css
background: rgba(0,0,0,0.05);
height: 1px;
width: 1174px; /* or full width in footer */
```

### Footer Navigation
- **Layout:** 4 columns with decorative large letter marks (F, A, S, T) at 50% opacity
- **Category label:** Inter Regular, ~12px, uppercase, `rgba(43,44,47,0.3)`
- **Link text:** Inter Regular, ~13–14px, `#2B2C2F`, line-height 20px
- **Spacing:** 48px gap between letter mark and link list

### Footer Bottom Bar
- Social icons centered, separated by vertical dividers (`rgba(0,0,0,0.05)`, 2×16px)
- Icons: X, Telegram, Discord, YouTube, LinkedIn — each 25px, padded 48px on each side
- Copyright: Inter Regular, ~13px, `rgba(95,102,114,0.6)`, centered
- Decorative metallic liquid animations on left and right edges

---

## 7. Iconography & Social

### Social Platforms
Fast is present on the following platforms (use brand-specific SVG icons):
- **X (Twitter)** — `fast-x.svg`
- **LinkedIn** — `fast-linked.svg`
- **Telegram** — `fast-telegram.svg`
- **Discord** — `fast-discord.svg`
- **YouTube** — `fast-youtube.svg`
- **GitHub** — `ico_github.svg`
- **Google Scholar** — `ico_google_scholar-dark.svg`

### Icon Sizes
- **Footer social bar:** 25×25px (Discord: 25×18.75px, YouTube: 25×17px)
- **Founder bio social links:** 24×24px
- **Nav chevron:** 12px (Font Awesome 6 Pro Light)

---

## 8. Motion & Effects

### Background Treatment
The page uses a subtle radial gradient on the main background:
```css
background-image:
  url(/* SVG radial gradient, color rgba(192,196,204,0.15) */),
  linear-gradient(90deg, #E9EBF0 0%, #E9EBF0 100%),
  linear-gradient(90deg, #FFFFFF 0%, #FFFFFF 100%);
```

### Metallic Liquid Animations
- Footer features animated metallic liquid video assets on the left and right edges
- These are `400px` wide, positioned at the very bottom corners
- They create a premium, fluid visual effect

### Blur Effects
- Heading text blocks use `blur-[0px]` — structurally present but visually clean (suggest the system supports blur transitions)
- Hover overlays on buttons use `opacity: 0` circular overlays ready for transition on hover

### Logo Animation
- The "Group 2" frame in the hero contains the FAST wordmark with measurement lines (horizontal and vertical), suggesting a "measured precision" aesthetic for animated reveals

---

## 9. Voice & Messaging

### Tone
- **Technical confidence** — Uses precise numbers (200K+ TPS, Sub-100ms, 25+ years)
- **Visionary but grounded** — "Billions of AI agents" but backed by formal verification
- **Minimal and direct** — Short sentences, no fluff

### Key Messages
1. Fast is built for agents, not humans
2. Internet-speed payments, globally
3. Formally verified and secure
4. The infrastructure layer the agentic economy needs

### Messaging Hierarchy
| Level           | Example                                                                                             |
|-----------------|-----------------------------------------------------------------------------------------------------|
| **One-liner**   | "Fast is a payment layer that enables billions of AI agents to move money globally and securely at internet speed." |
| **Boilerplate** | Full paragraph (see Section 1 above) ending with "fast.xyz"                                        |
| **Tagline feel**| "200K+ TPS. Sub-100ms finality. Formally verified."                                                |

### Domain
- Website: **fast.xyz**
- In running text, render as a **semibold link** in `#6B7EA3` (slightly lighter brand blue)

---

## 10. Founders

### Grigore Rosu — Co-Founder & CEO
- Ph.D. Computer Science, UCSD
- Former NASA spacecraft software engineer
- UIUC Professor — invented the **K Framework** for formal verification
- Founded **Runtime Verification** (2010), secured billions in DeFi assets
- Building Fast as culmination of 25+ years of formal verification expertise

### Sriram Vishwanath — Co-Founder
- Byers Chair for Computer Engineering, **Georgia Tech**
- Former Professor, UT Austin
- IEEE Fellow & Technical Fellow at MITRE Labs
- 300+ publications, 19,000+ citations
- Serial entrepreneur, 3 exits, advises $1B+ startups
- Ph.D. Stanford; M.S. Caltech; B.Tech. IIT Madras

---

## 11. Press & Contact

**Press Inquiries CTA:** "For any PR & media inquiries, please [Contact Us]"
- CTA button: Primary Dark style (see Buttons section)
- Press contact email: See fast.xyz media kit

---

## 12. AI Agent Usage Guide

When building any asset for Fast, follow these directives:

### Do
- Use the 5-color palette exclusively — no off-brand colors
- Default to **light backgrounds** (`#F6F8FA` / `#E9EBF0`) for websites and presentations
- Use **dark backgrounds** (`#0D0F13`) for high-impact sections or dark-mode slides
- Apply **General Sans Variable** for all headings and key brand text
- Keep layouts minimal with generous whitespace
- Use precise language with numbers (TPS, latency, verification)
- Brand accent (`#A1B0CF`) should be used for **1–2 elements max per screen**
- Buttons should use the gradient treatment, not flat fills
- Dividers should be subtle: `rgba(0,0,0,0.05)`, never a hard line

### Don't
- Don't use more than 5 colors on a single surface
- Don't use decorative fonts or display typefaces not in the system
- Don't add drop shadows beyond the approved `0px 1px 1px rgba(0,0,0,0.1)` button shadow
- Don't place the logo on busy backgrounds
- Don't write marketing copy that makes promises beyond the stated specs
- Don't refer to the company as anything other than "Fast" or "Fast by Pi² Labs"
- Don't use gradients for text (body text is always flat color)

### Slide Decks
- Slide canvas: 16:9 (1920×1080px or 1280×720px)
- Use `#0D0F13` dark slides for impact; `#F6F8FA` light slides for content
- Hero text: General Sans Variable Medium, 64–80pt
- Body text: General Sans Variable Regular, 18–22pt, color `#5F6672`
- Accent elements: `#A1B0CF` for highlights, callouts, or data points
- Section dividers: 1px `rgba(0,0,0,0.1)` horizontal rules

### Websites
- Max content width: 1176px, centered on 1440px canvas
- Page background: `#E9EBF0` to `#F6F8FA`
- Section padding: 80px vertical, 132px horizontal
- Typography: implement General Sans Variable via font loading or variable font file
- Borders: use `rgba(0,0,0,0.05)` for all structural borders and dividers

### Social Graphics
- Background: either `#0D0F13` (dark) or `#F6F8FA` (light)
- Text: use brand color `#A1B0CF` for highlights in dark mode
- Always include the Fast wordmark
- Keep copy under 10 words for social headers

---

## 13. File References

| Asset                    | Format | Notes                                     |
|--------------------------|--------|-------------------------------------------|
| Logo (dark on light)     | SVG, PNG | Use on white/light backgrounds           |
| Logo (light on dark)     | SVG, PNG | Use on `#0D0F13` backgrounds             |
| Social icons             | SVG    | X, LinkedIn, Telegram, Discord, YouTube  |
| Footer letterforms       | SVG    | F, A, S, T — decorative, 50% opacity     |
| Metallic liquid          | WebM   | Footer edge animations                   |
| Founder portraits        | IMG    | Gradient overlay: `#C8CFD8` → `#5F6672` |

---

*This document was generated from the FAST Figma design file (node: Media Kit) on 2026-03-25. Always defer to the Figma source of truth for pixel-perfect specifications.*
