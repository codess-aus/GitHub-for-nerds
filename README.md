# GitHub for Microsoft Nerds Workshop Site

This repository contains an MkDocs-powered workshop website generated from the slides in `docs/assets`.

## Local development

1. Install dependencies:

	`python -m pip install -r requirements.txt`

2. Serve locally:

	`mkdocs serve`

3. Build a production site:

	`mkdocs build --strict`

## GitHub Pages deployment

Deployment is configured with GitHub Actions in `.github/workflows/deploy.yml`.

On each push to `main`, the workflow:

1. builds the MkDocs site
2. uploads the generated `site` artifact
3. deploys to GitHub Pages

## Content structure

- `docs/index.md` - workshop landing page
- `docs/chapters/` - one chapter per slide asset
- `docs/resources.md` - consolidated links and follow-up exercises
- `docs/stylesheets/extra.css` - responsive, accessible workshop styling and dark/light theme overrides

## Verified latest versions snapshot

Checked on 2026-06-05:

- MkDocs: `1.6.1`
- MkDocs Material: `9.7.6`
- GitHub Copilot CLI npm package: `1.0.59`