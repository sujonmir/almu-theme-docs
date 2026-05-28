---
title: Accessibility
layout: default
nav_order: 8
---

# Accessibility

Almu targets **WCAG 2.1 AA** and Shopify Theme Store accessibility requirements.

## What's built in

| Feature | Where |
| --- | --- |
| **Skip-to-content link** | `layout/theme.liquid` — visible only on keyboard focus |
| **`:focus-visible` styles** | `assets/base.css.liquid` — focus ring on every interactive element when keyboard-focused |
| **ARIA live regions** | Cart drawer announces line-item changes; toasts use `role="status"` |
| **Keyboard trap** | Cart drawer, newsletter popup, fullscreen viewer all trap focus while open |
| **Mega menu arrow nav** | Arrow keys move between sub-items, Esc closes |
| **`aria-expanded` / `aria-controls`** | Every toggle (mega menu, mobile menu, search overlay, accordions) |
| **Semantic landmarks** | `<header>`, `<main id="main-content">`, `<nav>`, `<footer>` |
| **Image alt text** | Every theme-rendered image has `alt`; product images use the Shopify alt field; fallback uses the section heading or product title |
| **Form labels** | Every input has a `<label>` (visually hidden where appropriate, but always present for screen readers) |
| **Color contrast** | All default color combinations meet WCAG AA (4.5:1 for body text, 3:1 for large text) |
| **`<html lang>`** | Dynamic based on `request.locale.iso_code` — screen readers pronounce content correctly |

## What you should test before going live

- **Tab through the whole homepage.** Focus should be visible at every step. Order should make sense.
- **Open the cart drawer with the keyboard.** Tab cycles inside, Esc closes, focus returns to the trigger.
- **Use a screen reader on one product page.** VoiceOver (Mac) or NVDA (Windows). Confirm: heading order, link purpose, form labels, alt text.
- **Verify color contrast** of any custom colors you set. Use [WebAIM contrast checker](https://webaim.org/resources/contrastchecker/).

## Common pitfalls when customising

- **Color contrast** — picking a soft pastel for body text on a white background drops contrast below 4.5:1.
- **Removing focus styles** — don't override `:focus-visible` in Custom CSS without providing a replacement.
- **Hiding elements with `display: none` instead of `aria-hidden`** — screen readers will still see `aria-hidden`-only elements visually but skip them aurally. Almu does this for decorative icons.
- **Auto-playing video with sound** — WCAG fails. Keep video muted by default.

## Reporting an accessibility bug

Email [sujonmhk786@gmail.com](mailto:sujonmhk786@gmail.com?subject=Almu%20%7C%20Accessibility%20bug) with:

1. URL where the issue occurs
2. Browser + assistive technology + version
3. Steps to reproduce
4. Expected vs actual behavior
