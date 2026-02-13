# dtrupenn.github.io

Personal website built with [Vite](https://vite.dev/) and [Tailwind CSS](https://tailwindcss.com/).

## Prerequisites

- Node.js 20+ (or current LTS)
- npm 10+

## Install dependencies

```bash
npm install
```

## Run locally

Start the local dev server:

```bash
npm run dev
```

Vite will print a local URL (usually `http://localhost:5173`).

## Build artifacts

Create a production build:

```bash
npm run build
```

Generated artifacts are written to:

- `dist/index.html`
- `dist/assets/*`

Preview the production build locally:

```bash
npm run preview
```

## Deploy to GitHub Pages

This repository is named `dtrupenn.github.io`, so it is a user site repo and should publish from the default branch.

1. Run:
   ```bash
   npm run build
   ```
2. Commit and push.
