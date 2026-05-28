---
title: Theme Settings
layout: default
nav_order: 3
---

# Global Theme Settings
{: .no_toc }

Settings that apply to the whole store. Find these in **Online Store → Themes → Customize → Theme settings** (the gear icon at the bottom of the left sidebar).

1. TOC
{:toc}

---

## Typography

Pick fonts for headings and body text. Almu uses Shopify's font_picker, so you have access to every font in the Shopify font library — both system fonts (no extra HTTP request) and Google Fonts (loaded asynchronously with `font-display: swap`).

| Setting | What it does |
| --- | --- |
| **Primary font** | Used for body text, paragraphs, and most UI |
| **Heading font** | Used for h1–h6 headings (falls back to primary if not set) |

> **Performance tip:** system fonts render fastest. If you choose a Google Font, only the regular and bold weights are preloaded; italic and other weights are lazy-loaded.

## Layout

| Setting | What it does |
| --- | --- |
| **Page width** | Maximum content width on desktop. Sections respect this unless their own setting says "Full width". |
| **Section spacing** | Default vertical padding between sections. Each section can override. |

## Colors

Almu uses a small palette that cascades through every section. Section-level colors override these.

| Setting | Common uses |
| --- | --- |
| **Background** | Page background |
| **Foreground (text)** | Body text |
| **Accent** | Buttons, links, focus rings |
| **Border** | Card borders, dividers |
| **Card background** | Product cards, article cards, comparison cells |

## Cart

| Setting | Description |
| --- | --- |
| **Cart type** | **Drawer** (slides in from the right) or **Page** (`/cart`) |
| **Show shipping note** | Free-text note above the cart total — great for shipping thresholds |
| **Show order note field** | Lets customers add a note at checkout |
| **Show payment icons** | Shows the icons configured under **Payment icons** below |

The cart drawer keyboard-traps focus (WCAG 2.1.2) and announces line-item changes via an ARIA live region.

## Payment Icons

Pick which payment icons display in the cart drawer / footer. The icons available cover all major networks (Visa, Mastercard, Amex, PayPal, Apple Pay, Google Pay, Shop Pay, etc.).

## Back to top

A floating "back to top" button is available globally. Configure under **Theme settings → Back to top**:

| Setting | Description |
| --- | --- |
| **Enable** | Master toggle |
| **Position** | Bottom-right, bottom-left, or bottom-center |
| **Shape** | Circle, square, or rounded |
| **Size** | Button width/height (desktop + mobile) |
| **Icon** | Chevron up, arrow up, or double chevron |
| **Show label** | Adds a text label next to the icon |
| **Scroll threshold** | How far the user scrolls before the button appears |
| **Smooth scroll** | Animated vs instant scroll back |
| **Hide on mobile** | Hide for narrow screens (recommended if a chat widget is in the same corner) |

## Social Media

URLs for your social accounts. These power the share buttons in the page and article templates, and the footer social links.

## Favicon

Upload a square PNG/SVG/ICO. Recommended 32×32 px for crisp display in browser tabs.

## Checkout

Almu inherits Shopify's checkout. To brand the checkout, go to **Settings → Checkout → Customize**.

---

## Section-specific settings

Every section has its own settings panel — see the [sections reference]({{ "/sections/" | relative_url }}) for per-section documentation.
