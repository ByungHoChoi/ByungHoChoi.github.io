# Personal Blog

This is a Jekyll blog using the Minimal Mistakes theme.

Come here!

https://byunghochoi.github.io/

## How Jekyll Works

1. You write content in Markdown files.
2. Each Markdown file starts with front matter between `---` lines.
3. Jekyll reads `_config.yml`, layouts, includes, posts, and assets.
4. Jekyll generates plain HTML/CSS files into `_site`.
5. A static host, such as GitHub Pages, serves those generated files.

There is no backend server in this first version. The "build" step happens
before deployment.

## Important Files

- `_config.yml`: site settings.
- `_posts`: dated Markdown posts.
- `_data/navigation.yml`: top navigation links.
- `Gemfile`: Ruby/Jekyll dependencies.
- `index.md`: home page content.
- `examples/tiny-jekyll-theme`: the first handmade learning version.

## Running Locally

Install Ruby and Bundler first. Then run:

```sh
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll, usually:

```text
http://127.0.0.1:4000
```

## Writing a Post

Create a file in `_posts` using this filename format:

```text
YYYY-MM-DD-title-here.md
```

Example:

```md
---
title: "My New Note"
categories: learning
---

Write the post here.
```

Use one of these categories:

- `papers`
- `life`
- `learning`

## Theme

This site uses `minimal-mistakes-jekyll`.

The important theme settings are in `_config.yml`:

```yml
theme: minimal-mistakes-jekyll
minimal_mistakes_skin: "air"
plugins:
  - jekyll-include-cache
```

Pages and posts use Minimal Mistakes layouts such as:

- `home`
- `archive`
- `single`
