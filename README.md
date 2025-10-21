
# Revolant EPK — GitHub Pages Project Site

This folder is a ready-to-publish **project site** for GitHub Pages.
It will be served at `https://<your-username>.github.io/epk/` and, once the user/organization site is mapped to a custom domain, also at `https://revolantband.com/epk`.

## Publish Steps (project repo)
1. Create a new GitHub repository named **epk** (public).
2. Upload *all* files from this folder to the root of that repo (including `.nojekyll`).
3. In the repo: **Settings → Pages**  
   - Source: **Deploy from a branch**  
   - Branch: **main** (or `master`) / folder: **/** (root)
4. Wait for Pages to finish building; your site appears at `https://<your-username>.github.io/epk/`.

## Map custom domain `revolantband.com/epk`
To use the `revolantband.com/epk` URL:
- Set up a **user/organization site** in a separate repo named `<your-username>.github.io` (or your org’s).  
- In that repo’s **Settings → Pages**, set **Custom domain** to `revolantband.com` and save.
- Update DNS at your domain registrar:
  - **Apex** (`revolantband.com`) → A records to GitHub Pages IPs:
    - 185.199.108.153
    - 185.199.109.153
    - 185.199.110.153
    - 185.199.111.153
  - **WWW** (`www.revolantband.com`) → CNAME to `<your-username>.github.io`
- Once the apex custom domain is configured for your user/organization site, this **project site** will be accessible at `https://revolantband.com/epk` automatically.

## Files
- `index.html` — the scrolling EPK
- `logo.png`, `band.jpg`, `gallery1..3.jpg` — images (replace gallery images when you have live shots)
- `Revolant_EPK_OneSheet.pdf` — downloadable one‑sheet
- `.nojekyll` — disables Jekyll processing
- `404.html` — not found page
