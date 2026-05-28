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
| [Header]({{ "/sections/header/" | relative_url }}) | Every page (header group) | Mega menu, search overlay, mobile menu |
| [Footer]({{ "/sections/footer/" | relative_url }}) | Every page (footer group) | Menus, payment icons, newsletter, social |
| [Announcement bar]({{ "/sections/announcement-bar/" | relative_url }}) | Every page (header group, optional) | Sticky banner above the header |
| [Cart drawer]({{ "/sections/cart/" | relative_url }}) | Rendered globally | Cart drawer + cart page |
| [Newsletter popup]({{ "/sections/newsletter-popup/" | relative_url }}) | Rendered globally | Timed popup with email capture |

## Page templates

| Section | Used on |
| --- | --- |
| [Main product]({{ "/sections/main-product/" | relative_url }}) | Product pages (PDP) |
| [Collection]({{ "/sections/collection/" | relative_url }}) | Collection pages |
| [Cart]({{ "/sections/cart/" | relative_url }}) | Cart page |
| [Blog]({{ "/sections/blog/" | relative_url }}) | Blog listing |
| [Article]({{ "/sections/article/" | relative_url }}) | Single blog post |
| [Page]({{ "/sections/page/" | relative_url }}) | Static pages (About, etc.) |
| [Password]({{ "/sections/password/" | relative_url }}) | Password page (when store is locked) |
| [404]({{ "/sections/404/" | relative_url }}) | Not found |
| [Search]({{ "/sections/search/" | relative_url }}) | Search results |
| [Gift card]({{ "/sections/gift-card-display/" | relative_url }}) | Gift card page |

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
