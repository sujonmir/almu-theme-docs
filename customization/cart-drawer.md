---
title: Cart Drawer
layout: default
parent: Customization
nav_order: 1
---

# Customising the Cart Drawer

1. **Enable the drawer** — **Theme settings → Cart → Cart type → Drawer**.
2. **Shipping note** — under **Cart drawer** section, set "Shipping note" to something like:
   ```
   Spend {{amount}} more for free shipping
   ```
   The `{{amount}}` placeholder is replaced with the remaining amount until the threshold you set in "Shipping note threshold".
3. **Order note field** — toggle "Show order note field" if you accept custom requests from customers.
4. **Payment icons** — choose which icons display via **Theme settings → Payment icons**.
5. **Empty state** — upload an "empty cart image" and configure the heading + body + CTA text under the cart drawer section.

## Visual tweaks

- **Line item border** — set color + width under the cart drawer section. Width 0 removes the border entirely.
- **Quantity controls** — choose +/- buttons or a numeric input under "Quantity controls".
- **Header / body background colors** — split into two so you can give the drawer header a brand accent.

## Accessibility notes

The drawer is keyboard-accessible by default. Don't add `tabindex="-1"` to anything inside the drawer or you'll break the focus trap.
