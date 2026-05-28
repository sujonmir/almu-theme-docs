---
title: Header
layout: default
parent: Sections
nav_order: 1
---

# Header

Used as the header group on every page. Configure once and it applies site-wide.

## What it includes

- **Logo** — uses your theme-level logo by default, or overrides per-header
- **Main navigation menu** — picks from your Shopify navigation menus (Online Store → Navigation)
- **Mega menu** — sub-menus with multi-column dropdowns; supports keyboard arrow navigation
- **Search overlay** — full-screen search that surfaces products and predictive results
- **Account icon** — links to /account
- **Cart icon** — opens the cart drawer (or links to /cart if drawer is disabled)
- **Mobile menu** — slide-in drawer on screens below 990 px

## Settings

| Setting | Description |
| --- | --- |
| **Menu** | The Shopify navigation menu to display |
| **Logo position** | Left, center, or right |
| **Logo width (desktop / mobile)** | In pixels |
| **Show search** | Toggle the search icon + overlay |
| **Sticky header** | Header stays at the top of the viewport on scroll |
| **Show announcement bar** | Render the announcement bar above the header |
| **Background color, text color** | Brand colors for the header itself |
| **Border color, border width** | Bottom border of the header |
| **Padding (desktop / mobile)** | Vertical padding |

## Accessibility

- Skip-to-content link is rendered above the header (visible only on keyboard focus).
- Mega menu sub-items are navigable with arrow keys; `Esc` closes the open sub-menu.
- All toggles use `aria-expanded` / `aria-controls`.

## Common customisations

- **Center-logo header** — set "Logo position" to "Center" and shorten the main menu to even out columns.
- **Transparent header on homepage only** — use Custom CSS in **Theme settings → Custom CSS**, target `.template-index .site-header`.
- **Sticky on scroll only after threshold** — already built in; the header pins after the user scrolls 100 px.
