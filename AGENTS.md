# Agent Notes

## Project

ECMFS Shipbuilding — multi-page marketing site for Eco-Construct Marine Flotation
Systems (ECMFS) Nig. Ltd.

## Commands

- `npm run dev` — dev server on http://localhost:8080
- `npm run build` — production build into `.output/`
- `npm run lint` — ESLint
- `npm run test` — Vitest

## Conventions

- Site copy belongs in `src/components/site/content.ts`, not inline in components.
- Images live in `public/img/`; downloadable documents in `public/downloads/`.
  Replace a file at the same path rather than renaming it, to avoid touching code.
- All global CSS is in `src/styles.css`. Utilities live in `src/components/ui/`.
- The homepage is the one place that keeps its own typography. Any change to
  `--font-sans` / `--font-display` must stay scoped away from `.site-main--home`.
- Do not rewrite published git history — no force pushes, no rebasing or amending
  commits that are already pushed. Keep the branch in a working state.
