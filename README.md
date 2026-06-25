# agarwalknayam.github.io

Personal website of Mayank Agarwal — a minimal Jekyll site served via
GitHub Pages at **[agarwalknayam.com](https://agarwalknayam.com)**.

## Editing the content

Everything is plain text. No build step is required to publish — just
commit and push, and GitHub Pages rebuilds the site.

| What you want to change | Edit this |
| --- | --- |
| Name, tagline, nav, social links | `_config.yml` |
| Home page intro | `index.html` |
| About page | `about.md` |
| Projects list | `_data/projects.yml` |
| A blog post | add a file in `_posts/` (see the sample) |
| Look & feel | `assets/css/style.css` |

Look for `TODO` markers — those are the placeholders to replace.

### Writing a post

Add `_posts/YYYY-MM-DD-slug.md` with front matter:

```yaml
---
title: "Post title"
subtitle: "Optional."
date: 2026-07-01
tags: [ideas]
---
Your Markdown body here.
```

## Running locally (optional)

GitHub builds the site for you, but to preview locally:

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```

(Requires Ruby + Bundler. The `github-pages` gem pins versions to
match production.)

## Deployment

1. Push to `main`.
2. In the repo on GitHub: **Settings → Pages → Source = `main` branch**.
3. The `CNAME` file points the site at `agarwalknayam.com`. Add the DNS
   records below at your domain registrar, then enable **Enforce HTTPS**.

### DNS for the custom domain

| Type | Host | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | iitjmayank.github.io. |
