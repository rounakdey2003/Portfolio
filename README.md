# Portfolio

A small personal portfolio site built with plain HTML, CSS and JavaScript and bundled using Parcel.

This repo contains the source under `src/` and a few dev scripts to run a local dev server or build a production bundle.

## Quick overview

- Dev server: Parcel serves `src/index.html` and watches for changes.
- Build: Parcel produces a production-ready `dist/` folder.
- Tech: vanilla JS, GSAP, Splitting.js and Lenis for scrolling/animations.

## Requirements

- Node.js (recommended >= 14)
- npm (bundled with Node.js)

If you don't have Node.js installed, download it from https://nodejs.org/.

## Install

Open a terminal (zsh on macOS) in the project root and run:

```bash
npm install
```

This will install Parcel (dev dependency) and runtime dependencies listed in `package.json`.

## Run locally

- Start the dev server (opens browser):

```bash
npm start
```

- Start the dev server and bind to all network interfaces (useful for testing from other devices on your LAN):

```bash
npm run start:network
```

Parcel will serve `src/index.html`. Edit files under `src/` (for example `src/js/`, `src/css/`) and the page will reload.

## Build for production

Create a production build (output goes to `dist/`):

```bash
npm run build
```

This runs `parcel build` (see `package.json`) and prepares assets with a `./` public URL so the build can be served from a static host or opened locally.

## Project structure

```
package.json
src/
  index.html        # entry HTML
  favicon.ico
  assets/           # images and other static assets
  css/
    base.css
  js/
    index.js        # main app logic
    item.js
    utils.js
```

## Scripts (from package.json)

- `npm start` — parcel dev server, opens browser
- `npm run start:network` — parcel dev server bound to 0.0.0.0
- `npm run clean` — remove `dist/*`
- `npm run build` — clean and build for production
- `npm run lint` — run ESLint to report problems in `src/`
- `npm run lint:fix` — run ESLint and apply fixes where possible
- `npm run format` — run Prettier and rewrite files in `src/`
- `npm run format:check` — check formatting without changing files

## Notes & troubleshooting

- If `npm start` fails with a Parcel error, ensure you ran `npm install` and are using a supported Node.js version.
- If you prefer Yarn or pnpm, the same commands will work after converting lockfiles; adjust as needed.
- If you want a specific license, add a `LICENSE` file. Currently no license is included in the repo.

## Contributing

Small changes are welcome: open a branch, commit, and create a PR. For larger changes (new dependencies or major rewrites), open an issue first to discuss.

---

**Made with ❤️ by [Rounak Dey](https://github.com/rounakdey2003)**
