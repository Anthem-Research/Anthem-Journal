# Anthem Journal Starter

A minimal Jekyll + Netlify starter for an Obsidian-written public journal.

## Structure

- `_posts/` — public journal essays. File names must follow `YYYY-MM-DD-title.md`.
- `_projects/` — project catalogue pages.
- `_layouts/` — page templates.
- `_includes/` — reusable HTML parts.
- `assets/css/style.css` — site styling.
- `netlify.toml` — Netlify build settings.

## Netlify settings

Build command:

```bash
bundle exec jekyll build
```

Publish directory:

```bash
_site
```

## Local testing

Install Ruby and Bundler, then run:

```bash
bundle
bundle exec jekyll serve
```

Open `http://localhost:4000`.

## Obsidian workflow

Open this repository folder as an Obsidian vault. Write posts and project pages directly in the folders above. Commit and push changes to GitHub. Netlify will rebuild the public site.

Do not place private archive material in this repository unless you are comfortable publishing it later.
