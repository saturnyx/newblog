# My New Blog

This is the source code for my personal blog. It is intentionally small: Zola
builds the site, Sass handles the styling, and Markdown is all I need to write
new posts.

The site is still a work in progress, so the design and content will continue
to change.

## Built with

- [Zola](https://www.getzola.org/) for generating the site
- [Tera](https://keats.github.io/tera/) templates for the page structure
- Sass for the stylesheets
- Markdown for blog posts

## Run it locally

Install Zola, then start the development server from the project directory:

```sh
zola serve
```

Open <http://127.0.0.1:1111> in your browser. Zola will rebuild the site as
files change.

To create a production build:

```sh
zola build
```

The generated site is written to `public/`.

## Writing a post

Create a Markdown file in `content/`. A post needs front matter at the top,
for example:

```md
+++
title = "A Small First Post"
date = 2026-01-01
+++

Write the post here.
```

The section configuration in `content/_index.md` sorts posts by date.

## Project layout

```text
content/     Blog posts and section configuration
sass/        Sass source files
templates/   Zola page and section templates
static/      Static assets copied to the built site
zola.toml   Site and Markdown configuration
```

## Deployment

Every push to `main` builds the site with Zola and deploys it to GitHub Pages
using the workflow in `.github/workflows/zola.yml`.

## License

See [LICENSE](LICENSE).
