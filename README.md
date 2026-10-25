# PixelWin Labs website

Three static pages for the company site: no build step, no scripts, no cookies. Upload the folder as it is to
GitHub Pages, Cloudflare Pages, Netlify or Firebase Hosting.

| File | What it is |
|---|---|
| `index.html` | Home page: Pocket Puzzles: Offline Games and its fourteen games |
| `privacy.html` | Privacy policy (linked from the Play Store listing and from the app's Settings) |
| `terms.html` | Terms of service (the same text as the company site's `pixelwin-labs-site/terms.html`; change both together) |
| `support.html` | Support address and common questions |
| `style.css` | The one stylesheet |
| `images/` | Logo, app icon and the ten game pictures |

## To fill in before it goes live
- **Company name** — "PixelWin Labs" everywhere (header, footer, privacy policy section 1).
- **Support email** — `pixelwinlabs@gmail.com` (Aftab, 2026-10-24) on every page (search for it). It must be a mailbox that is read.
- **Country** — "India" in `privacy.html` section 1.
- **Audience** — 18+ (Aftab, 2026-10-24): `privacy.html` "Children" and `terms.html` section 2 say so. The Play Console target audience must be 18+ too.
- **Store button** — in `index.html` the button reads "Coming soon to Google Play"; the comment above it holds the
  line to use once the app is published.
- **Screenshots** — `index.html` has a screenshots section inside a comment; add `images/shot-1.png` … `shot-5.png`
  and remove the comment markers.
- **`app-ads.txt`** — add the one line AdMob gives you as a file named `app-ads.txt` in this folder.
- **Dates** — "Last updated" in `privacy.html`.

The ten game pictures are the hub's own card pictures; to redraw them:
`cd game_hub && SITE_ASSETS_DIR=../website/images flutter test test/site_assets_test.dart`

## Domain
`CNAME` holds `pocketpuzzles.pixelwinlabs.com` (Aftab's domain is pixelwinlabs.com). GitHub Pages reads it as the custom domain; the DNS records are set at the registrar.
