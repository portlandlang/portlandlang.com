# The portlandlang.com website

The website for [Portland](https://github.com/portlandlang/portland), a joyous programming language for Apple silicon.

⚠️ Under construction: for now it says what the site will be, and it will grow a roadmap and a progress dashboard for the language spec.

## Development

Built with [Jekyll](https://jekyllrb.com) and deployed to GitHub Pages by the workflow in `.github/workflows/jekyll.yml` on every push to `main`.

### Running it

|                    |                                                      |
| ------------------ | ---------------------------------------------------- |
| `script/bootstrap` | install dependencies                                 |
| `script/server`    | serve at http://localhost:4000, rebuilding on change |
| `script/test`      | build the site the way the Pages workflow does       |
| `script/cibuild`   | bootstrap, then test                                 |

### Styles

Plain CSS in `assets/css/main.css`, on top of [Bootstrap](https://getbootstrap.com) vendored into `assets/vendor/stylesheets/` and `assets/vendor/javascript/` by [bootstrap-vendor](https://github.com/xoengineering/bootstrap-vendor). No preprocessor, no npm. The pinned version lives in `assets/.bootstrap-version`, so each task takes the `assets` path:

|                                                 |                                            |
| ----------------------------------------------- | ------------------------------------------ |
| `bundle exec rake 'bootstrap:status[, assets]'` | compare the vendored version to upstream's |
| `bundle exec rake 'bootstrap:update[, assets]'` | re-download at the pinned version          |
