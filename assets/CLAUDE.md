# assets/ — static assets

Served at `/assets` (see `angular.json`). Subfolders:
- `icon/` — favicons (`favicon.svg`, `favicon.png`) referenced in `index.html`.
- `branding/` — brand marks (`icon.svg`, the app-icon source).
- `images/` — misc images.
- `templates/<category>/` — placeholder folders (birthday, floral, graduation, kids, luxury,
  minimal, party, wedding) for future template preview/hero assets. Currently `.gitkeep` only —
  templates are rendered from config (`core/constants/templates.ts`), not from image files, and
  user photos are stored on the event (data URLs). Add curated preview images here if you later
  want static template thumbnails instead of the live `im-template-thumb` swatches.

Android launcher icons/splash are generated from `resources/logo.svg` via
`npx @capacitor/assets generate` (not from this folder).
