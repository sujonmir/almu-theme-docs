---
title: FAQ
layout: default
nav_order: 9
---

# Frequently Asked Questions

## General

### Is Almu compatible with my Shopify plan?

Yes — Almu works on every Shopify plan (Basic, Shopify, Advanced, Plus). All features use standard Shopify objects and Online Store 2.0 sections, so there's nothing plan-locked in the theme itself.

### Can I use Almu on multiple stores with one purchase?

No. The Shopify Theme Store license is per-store. Each store needs its own purchase. See the [LICENSE.md](https://github.com/) in the theme for full terms.

### Do I get free updates?

Yes — any updates to Almu show up in your store's **Online Store → Themes → Almu → Update available** banner. Click to install. Your customisations are preserved (Shopify keeps `settings_data.json` and template JSONs intact).

### How do I switch back to my old theme?

In **Online Store → Themes**, find your previous theme under "Theme library" and click **Actions → Publish**.

## Customisation

### Can I change [thing] without coding?

99% of the time, yes — every section has 20–80 settings in the theme editor. If something feels missing, [email me](mailto:sujonmhk786@gmail.com?subject=Almu%20%7C%20Customisation%20question) — I'm usually happy to add settings in the next update.

### How do I add my logo?

**Theme settings → Logo** in the theme editor. Upload a PNG, SVG, or 2× retina image.

### How do I change brand colors?

**Theme settings → Colors** for the global palette. Many sections have their own color overrides on top of the global palette.

### Can I edit the cart drawer styling?

Yes — open any page in the theme editor, scroll to the **Cart drawer** section in the left sidebar, and tweak header background, line-item border, padding, shipping note, payment icons, etc.

## Performance

### Why is my Lighthouse score lower than the demo?

Two usual reasons:

1. **Installed apps.** Each app adds JS to your storefront. Audit your app list.
2. **Image sizes.** If product images are 5 MB each, no theme can save you. Compress to ≤ 200 KB per image.

See the [performance guide]({% link performance.md %}) for more.

### Is the theme fast on Cyber Monday traffic?

Almu's storefront performance is independent of traffic volume — Shopify's CDN handles spikes. The only thing under your control is keeping your homepage focused (each extra section adds requests).

## Bugs

### A section won't save my settings

Refresh the theme editor. If it persists, check the browser console for errors — and [email me](mailto:sujonmhk786@gmail.com?subject=Almu%20%7C%20Bug%20report) with the section name and a screenshot of the console.

### Mobile menu is broken

Make sure the **Main menu** setting in the header section points to a valid Shopify navigation menu. If the menu has more than 3 levels of nesting, that's the issue — Almu supports up to 3 levels.

### Cart drawer is empty even after adding to cart

Confirm **Theme settings → Cart → Cart type** is set to **Drawer**, not **Page**. If it's set to Page, the cart adds work but they show up at `/cart` instead of in a drawer.

## Support

### How fast do you respond to support emails?

I aim for 24 hours on weekdays, 48 hours on weekends. For Theme Store buyers, I prioritise urgent storefront-down issues over feature requests.

### Can you customise the theme for me?

I don't offer custom-development services as part of the standard license. For larger custom work, email me with your scope — happy to refer you to a Shopify Expert if needed.
