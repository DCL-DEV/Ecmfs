# ECMFS Shipbuilding

Website for **Eco-Construct Marine Flotation Systems (ECMFS) Nig. Ltd** — a Nigerian
marine construction company building aluminium and steel vessels, concrete flotation
systems, and providing boat maintenance and yacht construction services.

RC No: 1879101

## Stack

- [TanStack Start](https://tanstack.com/start) (SSR + file-based routing)
- [React 19](https://react.dev) / TypeScript
- [Tailwind CSS v4](https://tailwindcss.com) + custom CSS layer
- [Vite 8](https://vite.dev) for bundling
- [Nitro](https://nitro.build) for the server build (Cloudflare Workers target)

## Development

Requires Node.js 20+ and npm.

```sh
git clone <this-repository-url>
cd <repository-name>
npm install
npm run dev
```

The dev server listens on <http://localhost:8080>.

## Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the dev server |
| `npm run build` | Production build (outputs to `.output/`) |
| `npm run build:dev` | Development-mode production build |
| `npm run preview` | Serve the production build locally |
| `npm run lint` | Run ESLint |
| `npm run test` | Run the Vitest suite |
| `npm run format` | Format with Prettier |

## Deployment

The build targets Cloudflare Workers via Nitro. `npm run build` emits:

- `.output/public` — static client assets
- `.output/server` — the SSR worker bundle
- `.output/server/wrangler.json` — generated Wrangler config

## Content

Site copy lives in `src/components/site/content.ts`; images are served from
`public/img/` and downloadable documents from `public/downloads/`. Replacing a file
at the same path updates the site without touching code.
# ECMFS
