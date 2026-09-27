# Changelog

## Unreleased

- **LICENSE.md stays in the repo, off the site** — added to Jekyll's exclude list, so it is no longer published as a page.
- **Bootstrap moved under assets/** — the vendored files and `.bootstrap-version` now live in `assets/`, published with the rest of the assets, and the root `vendor/` is excluded whole as bundler's. The bootstrap-vendor tasks take the `assets` path. This deploy also rebuilds the site for the custom domain: the live page was built while the site still sat at the github.io subpath, so its asset URLs carried a `/portlandlang.com` prefix that portlandlang.com does not have, and it rendered unstyled.
- **MIT license** — added MIT license file.
- **Plain CSS and vendored Bootstrap** — removed Jekyll generated Sass files. Vendored Boostrap CSS/JS.
- **Init website** — generated a Jekyll 4.4 site with `jekyll new --blank`, one under-construction page in the language repo's own words, a `CNAME` for portlandlang.com, and a GitHub Pages workflow, with the actions pinned to their current majors (`checkout@v7`, `configure-pages@v6`, `upload-pages-artifact@v5`, `deploy-pages@v5`). Scripts to Rule Them All for bootstrap, server, test, and cibuild.
