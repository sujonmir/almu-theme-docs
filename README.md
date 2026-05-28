# Almu Theme Documentation

This repository contains the public documentation for the **Almu Shopify theme**, published at:

**https://sujonmir.github.io/almu-theme-docs/**

The site is built with [Jekyll](https://jekyllrb.com/) + the [just-the-docs](https://just-the-docs.github.io/just-the-docs/) theme and served by GitHub Pages.

---

## Publishing this repo to GitHub Pages

1. Create a new GitHub repo named **`almu-theme-docs`** under your `sujonmir` account.
2. From this folder, push the contents:
   ```bash
   git init
   git add .
   git commit -m "Initial docs"
   git branch -M main
   git remote add origin https://github.com/sujonmir/almu-theme-docs.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: **main** / **(root)**
   - Save.
4. Wait 1–2 minutes. The site builds automatically and goes live at
   `https://sujonmir.github.io/almu-theme-docs/`.

That URL is already wired into the theme's `theme_documentation_url` in `config/settings_schema.json`. If you use a different repo name or username, update that field.

## Local preview (optional)

If you want to preview docs locally before pushing:

```bash
cd documentation
bundle install
bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000/almu-theme-docs/>.

You need Ruby installed (`ruby --version` should print 2.7+).

## File layout

```
documentation/
├── _config.yml           # Jekyll config (theme, search, nav)
├── index.md              # Home page
├── installation.md       # How merchants install the theme
├── theme-settings.md     # Global settings reference
├── localization.md       # 11 supported languages
├── performance.md        # Lighthouse, lazy load, LCP
├── accessibility.md      # WCAG 2.1 AA features
├── faq.md
├── changelog.md
├── support.md
├── 404.md
├── sections/             # one md per section
│   ├── index.md
│   ├── header.md
│   ├── footer.md
│   ├── main-product.md
│   └── ...
├── customization/        # how-to guides
│   ├── index.md
│   ├── cart-drawer.md
│   └── ...
├── Gemfile               # only used for local preview
└── .gitignore
```

## Editing the site

Every page is a markdown file with a YAML front-matter block. The front-matter controls the page's place in the sidebar:

```yaml
---
title: My Page
layout: default
parent: Sections    # optional — for nested pages
nav_order: 5         # controls sidebar ordering
---
```

Save, commit, push — GitHub Pages rebuilds within a minute.

## License

The docs themselves are © 2026 Sujon Mir. The Almu Shopify theme is licensed separately via the Shopify Theme Store — see the theme repo's `LICENSE.md`.
