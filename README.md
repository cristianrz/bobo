# bobo
KISS static site generator in ~120 lines of POSIX shell and awk.

## Prerequisites

* [`smu`](https://github.com/Gottox/smu) — Markdown to HTML (or any converter; change `CMD` in `bobo-build-page`)
* `busybox` — local development server

## Getting started

```sh
git clone https://github.com/cristianrz/bobo.git
cd mysite
./bobo-init
```

Edit files inside `articles/`, `pages/`, and `resources/`, then:

```sh
./bobo-run
# open http://localhost:8080
```

## Project layout

```
mysite/
├── articles/        # Blog posts (Markdown)
├── pages/           # Static pages (Markdown)
├── resources/       # CSS, images, fonts — copied verbatim to html/
├── template.html    # Page template — use $article$ as content placeholder
└── html/            # Generated output (do not edit)
```

## Writing content

The first `h1` is used as the page title and the first `h6` as the date
in the blog index:

```markdown
# My article title
###### 12 Apr 2026

Body text here.
```

## Authors

- **Cristian Ariza** — [cristianrz](https://github.com/cristianrz)

See also the list of [contributors](https://github.com/cristianrz/bobo/contributors).

## License

See the [LICENSE](LICENSE) file for details.
