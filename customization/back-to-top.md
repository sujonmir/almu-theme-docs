---
title: Back to Top
layout: default
parent: Customization
nav_order: 2
---

# Back-to-Top Button

A floating button that scrolls the user to the top of the page after they've scrolled past a threshold.

## Settings

Find these under **Theme settings → Back to top**:

| Setting | Default | Notes |
| --- | --- | --- |
| **Enable** | On | Master toggle |
| **Position** | Bottom-right | Or bottom-left / bottom-center |
| **Shape** | Circle | Or square / rounded |
| **Border radius** (when shape = rounded) | 10 px | |
| **Icon** | Chevron up | Or arrow up / double chevron |
| **Show label** | Off | Adds text next to the icon |
| **Label text** | "Back to top" | Only when "Show label" is on |
| **Size (desktop / mobile)** | 44 / 40 px | Width/height of the button |
| **Icon size (desktop / mobile)** | 20 / 18 px | |
| **Scroll threshold** | 400 px | How far the user scrolls before the button appears |
| **Smooth scroll** | On | Animated vs instant scroll back |
| **Side offset (desktop / mobile)** | 24 / 16 px | Distance from the side of the viewport |
| **Bottom offset (desktop / mobile)** | 24 / 16 px | Distance from the bottom |
| **Background / icon color** | Dark / white | |
| **Hover background / icon color** | Lighter dark / white | |
| **Shadow strength** | 18 (0–100) | Box-shadow opacity |
| **Hide on mobile** | Off | Enable if a chat widget is in the same corner |

The button is rendered globally from `layout/theme.liquid`, so it appears on every page that uses the main layout.
