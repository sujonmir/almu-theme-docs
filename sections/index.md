---
title: Sections
layout: default
nav_order: 4
has_children: true
permalink: /sections/
---

# Sections Reference

Almu ships with 50 sections. Each section is independently configurable through the Shopify theme editor.

## Core layout (always present)

| Section | Use on | Notes |
| --- | --- | --- |
| [Header]({% link sections/header.md %}) | Every page (header group) | Mega menu, search overlay, mobile menu |
| [Footer]({% link sections/footer.md %}) | Every page (footer group) | Menus, payment icons, newsletter, social |
| [Announcement bar]({% link sections/announcement-bar.md %}) | Every page (header group, optional) | Sticky banner above the header |
| [Cart drawer]({% link sections/cart.md %}) | Rendered globally | Cart drawer + cart page |
| [Newsletter popup]({% link sections/newsletter-popup.md %}) | Rendered globally | Timed popup with email capture |

## Page templates

| Section | Used on |
| --- | --- |
| [Main product]({% link sections/main-product.md %}) | Product pages (PDP) |
| [Collection]({% link sections/collection.md %}) | Collection pages |
| [Cart]({% link sections/cart.md %}) | Cart page |
| [Blog]({% link sections/blog.md %}) | Blog listing |
| [Article]({% link sections/article.md %}) | Single blog post |
| [Page]({% link sections/page.md %}) | Static pages (About, etc.) |
| [Password]({% link sections/password.md %}) | Password page (when store is locked) |
| [404]({% link sections/404.md %}) | Not found |
| [Search]({% link sections/search.md %}) | Search results |
| [Gift card]({% link sections/gift-card-display.md %}) | Gift card page |

## Marketing / homepage

| Section | Description |
| --- | --- |
| Hero banner with video | Full-bleed hero with image or video background |
| Featured products | Curated product grid |
| New arrival products | Sorted by created_at |
| Collection list | Showcase multiple collections |
| Collections grid | Compact collection grid |
| Image with text | Two-column image + copy |
| Image slider | Carousel with text overlay |
| Video section | Embedded YouTube/Vimeo/Shopify video |
| Testimonial slider | Customer reviews with author images |
| Happy clients | Logo carousel (Swiper-powered) |
| Smart multi-column set | Flexible 1–4 column blocks with collapsible items |
| Comparison table | Side-by-side product comparison |
| Before/after slider | Interactive image comparison |
| Countdown timer with banner | Countdown + CTA |
| FAQ special | Accordion FAQ |
| Instagram feed | Display recent Instagram posts |
| Map | Embedded location map |
| Contact form | Contact form section |
| Text marquee | Scrolling text |

## Customer account

| Section | Used on |
| --- | --- |
| Login | `/account/login` |
| Register | `/account/register` |
| Account | `/account` |
| Order details | `/account/orders/<id>` |
| Addresses | `/account/addresses` |
| Activate account | `/account/activate` |
| Reset password | `/account/reset_password` |

## Utility

| Section | Description |
| --- | --- |
| Custom liquid | Drop raw Liquid into the page |
| Divider | Horizontal rule with styling |
| Spacer | Vertical whitespace |

---

> Section docs are being filled in. If a section you need isn't documented yet, every setting in the Shopify theme editor has inline help text — and you can always email [support](mailto:sujonmhk786@gmail.com?subject=Almu%20%7C%20) for a walkthrough.
