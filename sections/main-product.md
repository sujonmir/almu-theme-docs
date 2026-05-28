---
title: Main Product
layout: default
parent: Sections
nav_order: 2
---

# Main Product (Product Page)

The PDP section. Splits into a **media column** (image gallery + video) and an **info column** (title, price, variant picker, buy buttons, blocks).

## Layout

| Setting | Description |
| --- | --- |
| **Section width** | Default (theme width) or Custom (define your own max width + percentage) |
| **Media width (%)** | Percentage of the section width given to the media column. Set 100 to stack media above info. |
| **Media position** | Left or right of the info column on desktop |
| **Gap between media & info** | Horizontal spacing (desktop) / vertical (mobile) |

## Media gallery

| Setting | Description |
| --- | --- |
| **Enable featured media** | If off, gallery shows full width above the info column |
| **Gallery position** | Top, bottom, left, or right of the featured media |
| **Gallery layout** | Slider (Swiper-powered) or grid |
| **Gallery items per row** | Desktop (1–6) and mobile (1–4) |
| **Enable fullscreen** | Click featured image to open fullscreen viewer with zoom + thumbnail strip |

## Blocks (info column)

The info column is built from blocks you add in the theme editor. Drag-and-drop to reorder. Available block types:

| Block | Purpose |
| --- | --- |
| **Vendor** | Product vendor / brand name |
| **Title** | Product title |
| **Price** | Regular + compare-at price, sale badge |
| **Variant picker** | Color swatches / pills / dropdowns + size pickers, with optional size-chart link |
| **Stock level** | "Only X left" indicator |
| **Buy buttons** | Add to cart, dynamic checkout, buy now |
| **Description** | Product description from Shopify admin |
| **Custom Liquid** | Drop raw Liquid into the info column |
| **Icon with text** | Trust badge / feature bullet with built-in SVG icon or custom image |
| **Collapsible content** | Accordion (e.g., shipping, returns, sizing) |
| **Payment icons** | Inline payment method icons |
| **Pro text block** | Heading + paragraph with typography controls |
| **Image** | Block-level image (with fullscreen viewer support) |
| **Limited stock countdown** | Countdown timer for limited-stock urgency |
| **Customer activity** | "X people viewing now" / "Y purchased recently" social proof |

Each block has its own settings panel — typography (desktop + mobile font sizes, weights), color, spacing, alignment.

### Variant picker — size chart icon

When a product has a "Size" option, the variant picker can show a "Size Chart" link with an icon. Icon options (all rendered as inline SVG):

- None
- Ruler
- Info
- Tag
- Box
- Shopping bag
- Checkmark

Pair with a **Size chart page** setting that points to a page with the actual size chart.

### Variant picker — picker style

| Style | When to use |
| --- | --- |
| **Button** | Default — pill buttons with the option value |
| **Swatch** | Color options with image swatches (uses each variant's featured image) |
| **Color pill** | Color options without images (uses option value as the CSS color) |

If "Swatch" is selected but a variant has no `featured_image`, the picker automatically falls back to "Color pill" for that variant.

## Accessibility

- Variant pickers use semantic `<fieldset>` + `<legend>` + radio inputs.
- Add-to-cart button shows a loading state announced via ARIA live region.
- Fullscreen viewer traps focus and closes on `Esc`.
