# timjfarrell.com

Personal site. Astro, static, no client-side framework.

## Running it

```bash
npm install
npm run dev      # localhost:4321
npm run build    # -> dist/
```

## Structure

- `src/styles/tokens.css` holds colors and the type scale, light and dark. Nothing hardcodes a hex outside this file.
- `src/styles/global.css` has element styles and layout primitives.
- `src/layouts/` has `Base` for chrome and `Article` for long-form.
- `src/components/` has cards, callouts, and per-article SVG diagrams.
- `src/pages/` is routes.

## Deploying

Built output goes to the `gh-pages` branch and is served by GitHub Pages at
the domain in `public/CNAME`. `public/.nojekyll` is required, otherwise Pages
runs Jekyll and drops the `_astro/` directory.
