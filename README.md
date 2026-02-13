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

### 1. Workflow file

This repo includes a GitHub Actions workflow at:

- `.github/workflows/deploy.yml`

It runs on pushes to `main` (or manual dispatch), then:

1. Installs dependencies with `npm ci`
2. Builds with `npm run build`
3. Uploads `dist/`
4. Deploys with `actions/deploy-pages`

### 2. Enable Pages in repository settings

In GitHub for this repository:

1. Open `Settings -> Pages`
2. Under **Build and deployment**, set **Source** to `GitHub Actions`

### 3. Deploy

Push to `main`:

```bash
git add .
git commit -m "$COMMIT"
git push origin main
```

After the workflow completes, your site will be live at:

- `https://dtrupenn.github.io/`

### 4. Manual trigger (optional)

You can also run the workflow from:

- `Actions -> Deploy to GitHub Pages -> Run workflow`
