# Changelog

## Unreleased

- **Plain CSS and vendored Bootstrap** — the generator's Sass files are gone; the site's styles are one plain `assets/css/main.css`, served as written. Bootstrap 5.3.8 (upstream's latest) is vendored into `vendor/stylesheets/` and `vendor/javascript/` by the bootstrap-vendor gem through a `Rakefile`, pinned in `.bootstrap-version`, and linked from the layout. Jekyll's exclude list now names only the bundler paths under `vendor/`, so the vendored files publish. Jekyll 4 still installs its Sass converter as a dependency; nothing in the site uses it.
- **The site exists** — a Jekyll 4.4 site generated with `jekyll new --blank`, one under-construction page in the language repo's own words, a `CNAME` for portlandlang.com, and a GitHub Pages workflow in the shape of eliduke/thisamericanlife.co's, with the actions pinned to their current majors (`checkout@v7`, `configure-pages@v6`, `upload-pages-artifact@v5`, `deploy-pages@v5`). Scripts to Rule Them All for bootstrap, server, test, and cibuild.
