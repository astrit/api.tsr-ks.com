# api.tsr-ks.com — constitution

This repo is the **single source of truth** for all tsr-ks.com content and media. It is served as static files (GitHub Pages); anything pushed goes live immediately.

- `data/{sq,en,de}.json` — all site content. The website (`../tsr-ks.com`) always fetches it from here; it has no local copy.
- Albanian (`sq`) is the base language: write it first, then translate to `en` and `de`. Every change covers all three files.
- All three files must keep the identical key structure. Structure changes also need the types in `../tsr-ks.com/settings/content.ts` updated.
- Keep changes backwards compatible: add new keys first, remove old ones only after the website that no longer uses them is deployed.
- `svg/` and `media/` hold the sign SVGs and videos used by the site.
