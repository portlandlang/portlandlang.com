# portlandlang.com

The website for [Portland](https://github.com/portlandlang/portland), a joyous programming language for Apple silicon. Under construction: for now it says what the site will be, and it will grow a roadmap and a progress dashboard for the language spec.

Built with [Jekyll](https://jekyllrb.com) and deployed to GitHub Pages by the workflow in `.github/workflows/jekyll.yml` on every push to `main`.

## Running it

|                    |                                                        |
| ------------------ | ------------------------------------------------------ |
| `script/bootstrap` | install dependencies                                   |
| `script/server`    | serve at http://localhost:4000, rebuilding on change   |
| `script/test`      | build the site the way the Pages workflow does         |
| `script/cibuild`   | bootstrap, then test                                   |
