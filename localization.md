---
title: Localization
layout: default
nav_order: 6
---

# Localization

Almu ships translations for 11 languages out of the box.

## Languages included

| Code | Language |
| --- | --- |
| en | English (default) |
| ar | Arabic |
| bn | Bengali |
| de | German |
| es | Spanish |
| fr | French |
| hi | Hindi |
| it | Italian |
| ja | Japanese |
| pt-BR | Portuguese (Brazil) |
| zh-CN | Chinese (Simplified) |

Each language has both a **storefront** locale file (`<lang>.json`) covering customer-facing text and a **schema** locale file (`<lang>.schema.json`) covering theme-editor labels.

## Enabling a language for shoppers

1. Shopify admin → **Settings → Languages**.
2. Click **Add language**, pick the language, and click **Add**.
3. The new language appears as **Unpublished**. Click it, then **Publish**.

Once published, the language appears in the locale selector in Almu's footer (if you've enabled the "Show locale selector" option in the footer settings).

## Translating into a new language

If you need a language not in the list above:

1. Shopify admin → **Settings → Languages → Add language**.
2. Once added, Shopify shows the language with empty translations.
3. Use Shopify's translation editor or a third-party app to fill in the customer-facing strings.

Or — copy `locales/en.default.json` to `locales/<your-lang>.json` and `locales/en.default.schema.json` to `locales/<your-lang>.schema.json`, translate each value, and push.

## RTL languages

Arabic and Hebrew flow right-to-left. Almu's CSS uses logical properties (`margin-inline-start`, `padding-inline-end`, etc.) where possible, so RTL works automatically for most components. Two manual checks if you publish Arabic:

- Verify the cart drawer slides in from the **left** instead of right (it should).
- Verify the mega menu chevrons flip direction.
