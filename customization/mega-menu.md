---
title: Mega Menu
layout: default
parent: Customization
nav_order: 4
---

# Building a Mega Menu

The header supports multi-column dropdowns whenever a nav item has nested children.

## Build it in Shopify

1. **Online Store → Navigation** → open your **Main menu**.
2. Add a top-level item like "Shop".
3. Under "Shop", add sub-items: "Men", "Women", "Accessories" — these become the dropdown's first level.
4. Under each sub-item, nest a third level — "T-shirts", "Hoodies", etc. — and they render as columns of links inside the mega menu.

The menu auto-detects the nesting and switches to mega-menu layout when there are 2+ levels of children.

## Featured image / promo card

Almu's mega menu supports an optional image card in the dropdown. To enable it, name a sub-item exactly `Featured` and point it to a collection or product. The theme renders that target as a featured card next to the link columns.

## Mobile

On mobile the same menu collapses into a sliding drawer with accordion expand/collapse. The structure is identical — Shopify uses the same nav data; only the rendering changes.

## Keyboard navigation

- `Tab` enters and exits the menu
- `Arrow keys` move between sub-items
- `Enter` follows the link
- `Esc` closes the open submenu and returns focus to the parent
