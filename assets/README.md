Assets folder

Instructions & Best Practices

- Place production-optimized assets in this folder (hero.webp, hero.jpg, team photos in .webp and .jpg, favicons).
- Create responsive variants (e.g., 400w / 800w / 1200w) and use `srcset` + `sizes` or `<picture>` with WebP and JPG fallbacks.
- Compress images with tools like Squoosh or `imagemin` to get good quality at smaller sizes.
- Prefer `loading="lazy"` on non-critical images (cards, team photos).
- Replace placeholder Picsum URLs in `index.html` with your optimized files when ready.

Favicons & Social Preview

- Add the following files into `assets/`:
  - `favicon-32x32.png` (32x32)
  - `favicon-16x16.png` (16x16)
  - `apple-touch-icon.png` (180x180)
  - `safari-pinned-tab.svg` (vector, optional) with `#0A2540` mask color
  - `og-image.jpg` / `og-image.webp` (1200x630 recommended) for social previews
- Ensure files are optimized and compressed; prefer WebP for images when possible.
- Update the `<meta property="og:url">` value in `index.html` to your production URL before deploying.
