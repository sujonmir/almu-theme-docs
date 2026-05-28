---
title: Cart
layout: default
parent: Sections
nav_order: 3
---

# Cart Drawer & Cart Page

Almu ships a feature-rich cart drawer (slide-in panel) and a full cart page. Switch between them via **Theme settings → Cart → Cart type**.

## Cart drawer (recommended)

The drawer is rendered globally — clicking any "Add to cart" button opens it. Features:

- Quantity adjustment with +/- buttons
- "Saved amount" badge per line item when a sale price exists
- Inline product property display (gift message, customizations, etc.)
- Shipping note above the total (configurable text — supports a `{{amount}}` placeholder for "Free shipping after $X")
- Order note field
- Payment icons row
- Continue shopping / Checkout CTAs
- Empty state with a configurable image + heading + button

### Cart drawer settings

| Setting | Description |
| --- | --- |
| **Header background, text color** | Drawer header styling |
| **Body background** | Drawer body |
| **Line item border, alignment** | Border color/width between line items |
| **Quantity controls** | Show as +/- buttons or text input |
| **Shipping note text** | Free-text note with optional `{{amount}}` placeholder |
| **Shipping note threshold** | Dollar amount above which the note shows celebration text |
| **Show order note field** | Customer can add a note before checkout |
| **Show payment icons** | Inline payment method icons |
| **Subtotal label** | Customize the "Subtotal" label |
| **Checkout button text** | Customize the CTA |
| **Empty-state image, heading, body, CTA** | All configurable |

### Accessibility

The cart drawer is fully keyboard-accessible:

- Opens on click of any "Add to cart" or cart icon
- Focus is trapped inside the drawer while it's open
- `Esc` closes it and returns focus to the trigger
- Line-item updates are announced via an ARIA live region
- Backdrop click also closes

## Cart page

If you prefer `/cart` as a full page (some merchants do for B2B), set **Cart type** to **Page**. The drawer becomes a redirect to `/cart`.

The cart page uses the same line-item template and supports the same settings (shipping note, order note, payment icons).
