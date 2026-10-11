# apophisgathering.com

Splash page for the Apophis Gathering (13 April 2029). Static site, no build step.

## Deploy (GitHub Pages)
1. Upload everything in this folder to the repo root (including the hidden `.nojekyll`).
2. Settings > Pages > deploy from the `main` branch, root folder.
3. `CNAME` already points to apophisgathering.com. At the DNS host, add GitHub Pages A records for the apex and a CNAME for `www`.
4. Turn on "Enforce HTTPS" once the certificate is issued.

## Signups
The form sends signups to the Customer.io "Apophis" workspace via the JavaScript snippet (public Site ID in `index.html`, `CIO_SITE_ID`). Each signup creates a person (id and email = address, `signup_source`, `created_at`) and a `signed_up` event.

## Files
- `index.html` page (all CSS/JS inline)
- `img/` photos, hero loop video (`hero-pass.mp4`) and its poster
- `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `site.webmanifest` icons
- `og-image.jpg` 1200x630 share image
- `404.html`, `robots.txt`, `sitemap.xml`
