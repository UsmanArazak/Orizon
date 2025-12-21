Deployment Notes

- If you deploy to Netlify or Vercel without a build step, simply point the publish/output directory to the repository root.
- If you add a build step (e.g., `npm run build` that outputs to `dist/`), update `deploy-pages.yml` to upload `dist/` instead of `.` and set the deploy path accordingly.
- For CI, store secrets or environment variables securely in your hosting platform.
- After deploying, verify Open Graph metadata with the Facebook/Twitter card validators and test the site on mobile.
