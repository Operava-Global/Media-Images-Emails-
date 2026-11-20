# OPERAVA Email & Media Assets

Public media library for OPERAVA email signatures and approved service imagery.

## Published paths
- `/Email%20Signatures/` — email signature portraits.
- `/Services%20Images/` — approved public-facing service imagery.
- `/` — responsive media-library preview page.

## Correct image formats
The original `.webp`-named files were inspected and contain JPEG image data. To ensure browsers and email clients receive the correct `image/jpeg` MIME type, canonical `.jpg` copies are now published alongside the original filenames. **Use the .jpg URLs in email templates.** The legacy .webp-named files remain temporarily for compatibility; do not use them for new references.

## GitHub Pages deployment
The GitHub Actions workflow publishes only the `public/` directory. It validates the domain file and canonical image assets before upload. The published root contains `CNAME` for `media.operavaglobal.com`.

For custom-domain activation, set the repository's Pages source to **GitHub Actions**, verify the custom domain in Settings → Pages, and enable HTTPS when GitHub reports the certificate is ready. DNS is managed in Cloudflare.

## Cache and MIME behavior
GitHub Pages derives static content types from file extensions and does not support Cloudflare Workers-style bindings or arbitrary `_headers` configuration. Use accurate extensions (`.jpg`, `.png`, `.svg`, `.webp`) and keep image URLs stable. Cloudflare DNS is currently configured as DNS-only for GitHub Pages.
