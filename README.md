# Orizon — Tech Innovation Hub (Bootstrap Edition)

Phase 1 is implemented in this workspace: initial scaffold, Bootstrap, fonts, icon script, and base CSS utilities.

## Local preview options

- Recommended (VS Code): Install the *Live Server* extension and click "Go Live" from the status bar.

- Using npx (no global installs):
  - `npx http-server -p 5500`  (simple static server)
  - or `npx live-server --port=5500 --open=./index.html`

- Global install (optional):
  - `npm i -g live-server`
  - `live-server --port=5500 --open=./index.html`

## Next steps
- Verify assets load and fonts/icons appear correctly in the browser.
- Then proceed to Phase 1.2 (CSS variable theming verification) and Phase 1.3 (add utilities & test hover states).

## Deployment
See `DEPLOYMENT.md` for instructions to deploy the site to Netlify, Vercel, or GitHub Pages. A GitHub Actions workflow is included at `.github/workflows/deploy-pages.yml` for automatic Pages deployments.