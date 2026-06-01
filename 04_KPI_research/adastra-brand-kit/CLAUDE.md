# Adastra Brand Kit — Agent Instructions

You are applying the Adastra visual identity to a web project.

## What to do first

1. Look at the project — identify what kind it is (plain HTML, React, Next.js, Vue, etc.) and how CSS is handled (stylesheet, Tailwind, inline styles, etc.)
2. Apply the brand using whatever approach fits the existing project. Do not change any HTML structure, page layout, or content — only visual styles.

---

## How to apply the brand

### 1. Font

Load Montserrat from Bunny Fonts and set it as the site-wide font.

```html
<link rel="preconnect" href="https://fonts.bunny.net" />
<link href="https://fonts.bunny.net/css?family=montserrat:400,500,700&display=swap" rel="stylesheet" />
```

```css
body { font-family: "Montserrat", "Gotham", Arial, sans-serif; }
```

Use these weights only: `700` (headings, CTAs), `500` (body, labels), `400` (captions, intro text).

### 2. Colours

Import the token file and use its CSS variables:

```css
@import "./adastra-brand-kit/tokens/tokens-variables.css";
```

Or link it in HTML:
```html
<link rel="stylesheet" href="./adastra-brand-kit/tokens/tokens-variables.css" />
```

| Variable | Hex | Use for |
|---|---|---|
| `var(--color-ada-red)` | `#F9423A` | CTAs, accents, icons on light backgrounds |
| `var(--color-ada-blue)` | `#163B6E` | Headings, nav, dark sections, footer |
| `var(--color-ada-charcoal)` | `#424242` | Body text |
| `var(--color-ada-canvas)` | `#F4F4F4` | Page and section backgrounds |
| `var(--color-white)` | `#FFFFFF` | Cards, content areas |

Full list of variables (tints, gradients, shadows, radii, motion) is in `tokens/tokens-variables.css`.

### 3. Buttons

Primary CTA:
```css
background: var(--color-ada-red);
color: #fff;
font-weight: 700;
border-radius: var(--radius); /* 4px */
border: none;
```

Secondary (outline):
```css
background: transparent;
color: var(--color-ada-blue);
border: 2px solid var(--color-ada-blue);
border-radius: var(--radius);
font-weight: 700;
```

### 4. Border radius

Default is `var(--radius)` = **4px**. Keep corners crisp — this brand is geometric, not rounded.

### 5. Logo

Replace any existing logo or site name with the correct SVG variant:

```html
<!-- Light background (white, canvas) -->
<img src="./adastra-brand-kit/icons/logos/adastra-basic-red.svg" alt="Adastra" height="36" />

<!-- Dark background (navy, dark sections) -->
<img src="./adastra-brand-kit/icons/logos/adastra-basic-white.svg" alt="Adastra" height="36" />
```

All logo variants are in `icons/logos/`. Use `adastra-short-*.svg` when space is limited (mark only, no text).

### 6. Icons

Icons come in two colour variants — choose based on background:

- `icons/red/` → use on white or light backgrounds
- `icons/white/` → use on navy or dark backgrounds

```html
<img src="./adastra-brand-kit/icons/red/cloud.svg" width="24" height="24" alt="" aria-hidden="true" />
```

Browse `icons/red/` to find matching icon names. Common ones: `cloud`, `data`, `bar-chart`, `security`, `people`, `settings`, `code`, `ai`, `analytics`, `check`, `arrow-right`.

### 7. Text size

No text anywhere should be smaller than 16px. Audit and fix any smaller sizes.

### 8. Optional pre-built classes

If it fits the project, link `css/brand-classes.css` and use these ready-made classes:

| Class | What it renders |
|---|---|
| `ada-eyebrow` | Red uppercase label (use above headings) |
| `ada-btn-primary` | Red filled CTA button |
| `ada-btn-secondary` | Blue outline button |
| `ada-card` | White card with shadow |
| `ada-badge` | Red pill tag |
| `ada-section-navy` | Navy section background |
| `ada-section-gradient` | Red-to-navy gradient section |
| `ada-stat-number` | Large red metric/stat number |

---

## Rules

- Do not use any font other than Montserrat / Gotham
- Do not use `font-weight: 600` — not in the brand
- Do not use italic for emphasis (only for actual quotes)
- Do not use glow shadows or colour-tinted shadows
- Do not change page structure, layout, or content

---

## Kit structure

```
adastra-brand-kit/
├── tokens/
│   ├── tokens-variables.css   ← CSS variables — use this for any project
│   └── tokens-tailwind.css    ← Tailwind v4 @theme block — use for Tailwind projects
├── css/
│   └── brand-classes.css      ← Optional pre-built classes
├── icons/
│   ├── logos/                 ← Logo SVGs (red, white, black variants)
│   ├── red/                   ← 100+ icons for light backgrounds
│   └── white/                 ← 100+ icons for dark backgrounds
└── CLAUDE.md                  ← This file
```
