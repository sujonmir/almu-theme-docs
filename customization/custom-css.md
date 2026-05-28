---
title: Custom CSS & Liquid
layout: default
parent: Customization
nav_order: 5
---

# Custom CSS & Custom Liquid

When the built-in settings don't cover what you need, Almu gives you two escape hatches.

## Custom CSS

Find it under **Theme settings → Custom CSS**.

Anything you put there is appended to the main stylesheet and applies storefront-wide. It runs after the theme's own CSS so your rules override.

Example:

```css
/* Make the header logo bigger only on the homepage */
.template-index .site-header__logo img {
  max-width: 220px;
}
```

The CSS is inlined into `<style>` on every page render — keep it under ~10 KB to avoid bloating the HTML.

## Custom Liquid section

Add a **Custom Liquid** section to any page that supports sections. Drop raw Liquid + HTML + JS in. Useful for:

- One-off promotional banners with custom logic
- Embedding a third-party widget that needs a `<script>` tag
- Quick A/B test markup before promoting it to a dedicated section

## Per-product custom Liquid

The Main Product section has a **Custom Liquid** block in the info column. Add it where you need it (above or below buy buttons, etc.). You have access to:

- `product` — the current product
- `current_variant` — the selected variant
- `customer` — the logged-in customer (if any)
- `cart` — the current cart

Example — show a personalised line based on variant inventory:

```liquid
{% if current_variant.inventory_quantity < 5 %}
  <p class="urgency-note">Only {{ current_variant.inventory_quantity }} left — order soon!</p>
{% endif %}
```
