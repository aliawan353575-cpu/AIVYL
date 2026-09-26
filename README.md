# AIVYLOX — Crypto AI Prompt Pro Pack 2026

Static site: `index.html`, `style.css`, `script.js`. No build step — deploy as-is to GitHub Pages (or any static host).

## Folder structure

```
/
├── index.html
├── style.css
├── script.js
├── README.md
└── assets/
    ├── favicon.svg        (placeholder geometric mark — replace with a real logo if you have one)
    └── images/            (empty — add real product/OG images here if you want them)
```

## Deploying to GitHub Pages

1. Push these files to the root of a repo (or a `/docs` folder, set accordingly in repo settings).
2. In the repo's **Settings → Pages**, set the source branch/folder.
3. No build process is required — it's plain HTML/CSS/JS.

## Things to update before launch

All of these are marked with clear placeholder text in `index.html` — search for the bracketed text below.

| What | Where in `index.html` | Placeholder text |
|---|---|---|
| Wallet addresses | Payment section (`#payment`) | `[VERIFIED USDT TRC20 ADDRESS]`, `[VERIFIED USDT BEP20 ADDRESS]`, `[VERIFIED USDC BEP20 ADDRESS]`, `[VERIFIED USDC SOLANA ADDRESS]` — replace both the visible text **and** the `data-address` attribute on each `<code>` element |
| Order form URL | "Already paid?" CTA and footer | `[ORDER FORM URL]` |
| Contact / Privacy / Terms pages | Footer links | `[CONTACT PAGE URL]`, `[PRIVACY POLICY URL]`, `[TERMS OF SERVICE URL]` |
| Price | Pricing section (`#pricing`) | `$12.50` current / `$41.99` regular — edit directly |
| Offer expiration | Pricing section, `.pricing-expiry` paragraph | Currently empty. Only add a date here if you have a real, verified expiration — do not add a countdown or fake urgency |
| Favicon / logo | `<link rel="icon">` in `<head>`, and `.brand-mark` in CSS | Replace `assets/favicon.svg` with a real mark if one exists |
| Testimonials | Trust section (`#trust`) | A placeholder comment marks where to add a real testimonial block once you have genuine customer quotes — do not add fabricated ones |
| Product mockup | Hero (`.mockup-glass`) and Product Value section (`.ebook-mockup`) | Currently built with CSS only (no image dependency). If you'd rather use a real product photo/render, replace the `.mockup-glass` or `.ebook-face` markup with an `<img>` pointing to `assets/images/` |

## Image asset requirements (optional)

The site currently ships with **zero image dependencies** — the hero mockup and ebook cover are built entirely in CSS so the page loads fast and never breaks on a missing file. If you want to swap in real imagery:

- **Hero product mockup**: 800×800px minimum, transparent PNG or WebP, under 200KB
- **Ebook / product cover**: 3:4 portrait ratio, WebP preferred
- **OG/social share image**: 1200×630px, add an `og:image` meta tag once you have one
- Use `loading="lazy"` on any `<img>` you add below the fold

## Notes

- All copy avoids profit promises, guarantees, fake scarcity, and fabricated social proof, per the brand brief.
- The delivery/verification window (12–24 hours) and the "manual verification" language are stated explicitly in the payment flow and FAQ — keep this consistent if the actual process changes.
- The disclaimer near the footer should not be edited to soften its language without legal review.
