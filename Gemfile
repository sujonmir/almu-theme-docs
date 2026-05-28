source "https://rubygems.org"

# GitHub Pages builds the site automatically — this Gemfile is only used
# for local preview via `bundle exec jekyll serve`.

gem "github-pages", group: :jekyll_plugins

# just-the-docs theme is loaded via remote_theme in _config.yml,
# so we don't need it as a gem dependency for GitHub Pages builds.

group :jekyll_plugins do
  gem "jekyll-remote-theme"
  gem "jekyll-seo-tag"
end

# Windows + JRuby support (safe to leave in cross-platform)
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
