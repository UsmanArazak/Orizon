# Deployment Options — Orizon Landing

This document shows simple deployment options for the static Orizon landing page.

## 1) Netlify (recommended for static sites)
- Connect your Git repository in Netlify (drag & drop also works for a quick test).
- _Build command_: (none required) — leave blank if you're serving static files from root.
- _Publish directory_: `/` or the repository root (if you use a build step, set this to `dist` or `public`).
- For continuous deploys, add Netlify environment variables for production if needed.

Quick steps (Netlify UI):
1. Click "New site from Git" → connect your repo.
2. Set branch (e.g., `main`), no build command, publish dir `/`.
3. Deploy and update site settings (custom domain, HTTPS, redirects).

## 2) Vercel
- Great for static sites and frontends. Connect your Git repo and configure the project.
- _Framework preset_: None / Static Site.
- _Build command_: (none) — leave blank if you are not using a build step.
- _Output directory_: `/` or `public` if you use a build step.

## 3) GitHub Pages
- Option A — GitHub Pages via `gh-pages` branch or `gh-pages` action.
- Option B — Use GitHub Pages with `Actions` (recommended). Example workflow is provided in `.github/workflows/deploy-pages.yml`.

## 4) Sample GitHub Actions (deploy to Pages)
- See `.github/workflows/deploy-pages.yml` in the repository for a ready-to-go CI workflow that deploys the `main` branch to GitHub Pages.

## 5) Tips & Production Notes
- Update `index.html` Open Graph `og:url` to your production URL before deploying.
- Add optimized image files to `assets/` and replace placeholder Picsum URLs.
- Ensure `assets/og-image.jpg` is present for social previews (1200x630 recommended).
- Consider a minimal build step to compress/minify CSS and bundle assets.
