---
title: Performance
layout: default
nav_order: 7
---

# Performance

Almu targets **Lighthouse Performance ≥ 60** on mobile (Shopify Theme Store minimum). What we do, what you should do, and how to debug regressions.

## What Almu does out of the box

| Optimisation | Where |
| --- | --- |
| **Critical CSS inlined** | `assets/critical.css` is inlined in `<head>` — only above-the-fold styles |
| **Base CSS async-loaded** | `media="print"` swap trick — non-critical CSS doesn't block first paint |
| **JS deferred** | `theme.js` uses `defer="defer"` so it doesn't block parsing |
| **Font preload** | Primary font is preloaded with `<link rel="preload" as="font">` |
| **`font-display: swap`** | Fonts swap-in immediately rather than blocking text render |
| **Preconnect / dns-prefetch** | To Shopify CDN, fonts.shopifycdn.com, monorail-edge, checkout — TCP handshakes resolved before they're needed |
| **Lazy-load all non-LCP images** | `loading="lazy"` on every `<img>` that isn't the primary product image |
| **LCP image eager** | Primary product image uses `loading="eager" fetchpriority="high"` |
| **Width/height on every img** | Prevents CLS — Lighthouse credits this directly |
| **WebP** | Product images served as WebP via `image_url: format: 'webp'` where possible |
| **Self-hosted Swiper** | No external CDN — Swiper is in `assets/swiper-bundle.min.js` |
| **No external CSS dependencies** | Zero requests to cdnjs, jsdelivr, unpkg, etc. |

## What you can do as a merchant

- **Optimise product images before upload** — Shopify resizes but doesn't recompress. Use TinyPNG or Squoosh to compress to ≤ 200 KB per image before uploading.
- **Limit apps** — every Shopify app you install injects scripts into your storefront. The biggest single performance hit on most stores is the *number* of apps. Audit your app list and remove unused ones.
- **Minimise the homepage** — every section adds requests + JS. A focused homepage scores higher than a maximalist one.
- **Test on a real device** — Lighthouse on a mid-range Android simulates slow CPU. Your iPhone won't.

## Lighthouse targets

| Category | Theme Store min | Almu targets |
| --- | --- | --- |
| Performance | 60 | ≥ 75 |
| Accessibility | 90 | 100 |
| Best Practices | 80 | ≥ 95 |
| SEO | 90 | 100 |

## Debugging a low score

If Lighthouse drops below 60 after you customise:

1. **Look at the "Largest Contentful Paint" element.** If it's an image, confirm `loading="eager"` + `fetchpriority="high"` is set.
2. **Audit installed apps.** Disable each one in turn and re-run Lighthouse to identify the culprit.
3. **Check Custom CSS / Custom Liquid** — bloated custom code can add KB to every page.
4. **Image weights** — Lighthouse's "Properly size images" check tells you which files are oversized.
