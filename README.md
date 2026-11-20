# OPERAVA Email & Media Assets

Public asset repository for OPERAVA email signatures and approved service imagery.

## Published assets
- `public/Email Signatures/` — department and general email-signature portraits.
- `public/Services Images/` — approved service/marketing imagery (add source-approved files here).

## GitHub Pages
The Pages workflow publishes the `public/` directory. Configure **Settings → Pages → Build and deployment → Source: GitHub Actions** if Pages is not already enabled. The intended custom domain is `media.operavaglobal.com`; point its DNS CNAME to `Operava-Global.github.io` and verify the domain in GitHub Pages before relying on it.

## Source and file-format note
Signature assets were copied from `DevJel/CEO_DASHBOARD-` (`src/brand/`). Their original filenames are preserved. Although the source filenames end in `.webp`, the image bytes are JPEG; serve these files as `image/jpeg` unless the files are converted and renamed in a separate reviewed change.
