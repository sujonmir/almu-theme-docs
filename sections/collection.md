---
title: Collection
layout: default
parent: Sections
nav_order: 9
---

# Collection (Product Listing)

The collection page template. Renders a filterable, sortable product grid with pagination.

## Layout

- Products per page (configurable)
- Columns: desktop (1–4) and mobile (1–2)
- Image aspect ratio: adapt, 1:1, 4:3, 16:9

## Filtering

Almu uses Shopify's storefront filters (configured in **Settings → Search & discovery → Filters**). The theme renders:

- **Sidebar filters** on desktop (left or right)
- **Drawer filters** on mobile (sticky "Filter" button at the top)
- **Apply / Clear / Clear all** controls
- **Filter chips** showing active filters above the grid

Filtering uses AJAX — the grid replaces in place, the toolbar/filters stay, and the URL updates so filtered views are shareable.

## Sort

Standard Shopify sort options (Featured, Best selling, Price low-high, etc.). Customer's selection persists across pagination.

## Pagination

Numbered pagination with prev/next. The "current" page is styled with the accent color.
