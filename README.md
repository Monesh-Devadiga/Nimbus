# Nimbus - Responsive Landing Page

A single landing page built with **pure HTML + CSS** (no JavaScript, no frameworks).
  
## Live preview
 
Live in: https://samplenimbus.netlify.app/  
OR   
Open `index.html` in any browser or  
run a local server:
 
```
npx serve .
# or
python -m http.server 8000
```

## Existed Files

| File | Purpose |
|------|---------|
| `index.html` | Semantic page structure: header, hero, features, how-it-works, pricing, FAQ, CTA and footer |
| `styles.css` | Mobile-first styles with CSS Grid + Flexbox and two media queries |

## Responsive strategy

Designed **mobile-first**: base styles target small screens, then scale up with two breakpoints.

| Breakpoint | Target | Key changes |
|------------|--------|-------------|
| Base (< 640px) | Mobile | Single column, hamburger menu (checkbox hack), stacked cards |
| `min-width: 640px` | Tablet | 2-column feature grid, 3-column pricing row, 2-column footer |
| `min-width: 1024px` | Desktop | Inline nav replaces hamburger, split hero layout, 3-column feature grid |

Techniques used:

- **CSS Grid** — features, pricing, showcase, footer layouts
- **Flexbox** — navigation, buttons, logo strip, hero actions
- **`clamp()`** — fluid typography that scales smoothly between breakpoints
- **Checkbox hack** — working mobile menu without JavaScript
- **`<details>`/`<summary>`** — accessible FAQ accordion without JS

## Test it at 3 widths

Resize the browser (or use DevTools device toolbar) at approximately:

1. **Mobile:** 375 × 812
2. **Tablet:** 768 × 1024
3. **Desktop:** 1440 × 900

Screenshots for each breakpoint are included in `/screenshots`.

## What I learned

- Structuring a page mobile-first keeps CSS smaller than "desktop-first + overrides"
- Grid's `auto-fit`/explicit columns make card layouts adapt with almost no media queries
- Flexbox handles component-level alignment; Grid handles page-level layout

---------------------------------------------------------------------------------------------------------------------
Designed and Managed By: 
  [@Monesh Devadiga](https://github.com/Monesh-Devadiga)  
CSE Student [@SCEM](https://www.sahyadri.edu.in/), Mangalore
