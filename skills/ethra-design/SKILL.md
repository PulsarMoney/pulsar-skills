---
name: ethra-design
description: Create distinctive, production-grade frontend interfaces for Ethra Protocol. Use this skill when the user asks to build components, pages, or applications regarding Ethra. Generates polished code following Ethra's maritime shipping finance aesthetic with a warm, institutional tone.
---

## Mission
This skill guides creation of distinctive, production-grade frontend interfaces for Ethra Protocol — a real-world asset (RWA) platform focused on maritime shipping finance. Implement real working code with exceptional attention to Ethra's warm, institutional design language.

## Rules

### Do
- prefer semantic tokens over raw values
- preserve visual hierarchy using the dual-typeface system (Zodiak + Gotham)
- keep interaction states explicit
- use the warm cream background as the default surface color
- maintain the institutional, trust-evoking tone throughout

### Don't
- Don't use cold/stark white backgrounds. Ethra uses warm cream (#f8f4eb) as the base.
- Don't mix up the typefaces — Zodiak is for headings/display, Gotham is for body/UI text.
- Don't use placeholder letter-circles for asset icons. Always use real logos (see "Asset Logos" section).
- Don't use bright/saturated accent colors outside the defined palette. Ethra's palette is muted and institutional.

## Style Foundations
- Visual style: warm, institutional, trust-evoking maritime finance aesthetic
- Art direction: clean editorial layouts with generous whitespace
- Typefaces: Zodiak (display/headings) + Gotham (body/UI)

### Icons
- Library: **Lucide** (https://lucide.dev)
- HTML/vanilla: load via CDN `https://unpkg.com/lucide@latest`
- React: use `lucide-react` package
- Default stroke-width: 1.5. Default size: 20px. Adjust per context.
- Always use Lucide icons for UI actions and feature illustrations. Never use emoji or raw unicode symbols as icon replacements.

### Typography

#### Display / Headings (Zodiak)
- Hero / Display: Zodiak Bold, 64px, -3% tracking, line-height: none
- Heading 1: Zodiak Extrabold, 76px, line-height: 76px
- Heading 2: Zodiak Bold, 40px, -3% tracking, line-height: none
- Heading 3: Zodiak Bold, 24px, line-height: 28px
- Heading 4: Zodiak Bold, 18px, -3% tracking, line-height: none

#### Body / UI (Gotham)
- Body Large: Gotham Book, 16px, -0.64px tracking, line-height: 1.3
- Body Small: Gotham Book, 14px, -0.42px tracking, line-height: 16px
- Label / Overline: Gotham Medium, 12px, 20% tracking, uppercase, line-height: 1.4
- Button: Gotham Medium, 12px, -3% tracking, line-height: 16px
- Caption: Gotham Book, 12px, -3% tracking, line-height: 16px

### Color Palette

#### Core Colors
- Background (cream): #f8f4eb — default page/surface background
- Primary Dark (navy): #18304a — headings, primary text, dark sections
- Secondary Blue: #264468 — secondary dark surfaces, hero backgrounds
- Green Accent: #4c8d49 — success states, ecosystem/growth indicators
- Gray Text: #5c5c5c — body text, secondary content
- Light Gray: #d2d2d2 — borders, dividers, subtle UI elements

#### Accent Colors
- Bronze: #bf8a46 — premium/highlight accents, CTAs
- Light Gold: #efcf96 — soft gold for secondary highlights
- Blue Tint: rgba(80, 146, 225, 0.15) — card containers, tinted sections

#### Text Colors by Context
- On dark backgrounds (navy/blue): #f8f4eb (cream) or #ffffff (white)
- On light backgrounds (cream): #18304a (navy) for headings, #5c5c5c (gray) for body
- Green accent text: #4c8d49 for ecosystem/reward elements
- Overline/label on light: #18304a (navy) or #4c8d49 (green)

### Spacing Scale
- Spacing scale: 8pt baseline grid
- Border radius: 16px (cards), 12px (containers), 8px (buttons/inputs), 4px (small elements)

### Asset Logos (crypto, fiat, stocks)
Never use placeholder circles with letters. Always use real logos:
- **Crypto tokens**: `https://coin-images.coingecko.com/coins/images/{id}/small/{filename}.png`. Common: Bitcoin `1/small/bitcoin.png`, Ethereum `279/small/ethereum.png`, USDC `6319/small/usdc.png`, USDT `325/small/Tether.png`.
- **Fiat currencies**: `https://flagcdn.com/w80/{country_code}.png`. Map: EUR=`eu`, USD=`us`, GBP=`gb`.
- Display in circular container (`border-radius: 50%`, `object-fit: cover`). 36px in lists, 48px in detail views.

### Brand Mark
- Wordmark: "Ethra" — likely set in Zodiak Bold
- Color: Primary Dark (#18304a) on light backgrounds, cream (#f8f4eb) on dark backgrounds

## Accessibility
WCAG 2.2 AA, keyboard-first interactions, visible focus states

## Writing Tone
Institutional, confident, measured. Evokes trust and expertise in maritime shipping finance. No emojis, no hype. Text should feel like it belongs in a premium financial prospectus — authoritative but accessible.

## When programming design systems
- Don't use magic numbers / strings. Always define the brand guides in the code to be structured. If you use Tailwind, the colors should be defined in the tailwind.config file.
- Define Ethra's color tokens as semantic variables (e.g., `--ethra-bg`, `--ethra-primary`, `--ethra-accent-green`).
- Import Zodiak and Gotham fonts appropriately. Zodiak is available from foundry sources; Gotham requires a license or use a similar alternative like `Inter` for body if Gotham is unavailable.
