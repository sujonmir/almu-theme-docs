---
title: Newsletter Popup
layout: default
parent: Sections
nav_order: 14
---

# Newsletter Popup

A timed popup with email capture. Rendered globally so it can appear on any page.

## Triggers

- **Delay** — show after N seconds on the site
- **Scroll depth** — show after N% scroll
- **Exit intent** (desktop only) — show when the mouse leaves the viewport top
- **Show once per session** — never re-pop after dismissal in the same session

## Settings

| Setting | Description |
| --- | --- |
| **Enable** | Master toggle |
| **Trigger type** | Delay, scroll, or exit |
| **Trigger value** | Seconds (for delay), percent (for scroll) |
| **Show on mobile** | Hide on narrow screens if intrusive |
| **Heading, body, button text** | Copy |
| **Background image** | Optional image (left side) |
| **Colors** | Background, text, accent |
| **Discount code** | Optional code to display after successful sign-up |
| **Success message** | Shown after sign-up completes |

## Accessibility

- Opens with focus trapped inside the modal
- `Esc` closes
- Backdrop click closes
- Dismissal is remembered in localStorage so the same visitor doesn't get re-spammed
