# Targeter API Documentation

This repository contains the documentation for the Targeter API — a campaign management platform for targeted marketing.

## Overview

Targeter provides a REST API for creating, managing, and monitoring targeted marketing campaigns. This documentation site is built with [Mintlify](https://mintlify.com).

## Prerequisites

- **Node.js** [20.17 or newer LTS](https://nodejs.org/) (22 is recommended). Mintlify does **not** support Node 25+ yet — use `nvm`, `fnm`, or `asdf` and the included `.nvmrc` if needed.

## Development

Install dependencies (once):

```bash
npm install
```

Preview the site locally (uses `docs.json` in this directory):

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000). Use `npm run dev -- --port 3333` for another port, or `npm run dev -- --no-open` to skip opening a browser.

Other scripts:

- `npm run validate` — strict build validation (good for CI)
- `npm run broken-links` — internal link check

### Why `bunx mintlify` failed

Older global or cached CLIs looked for `mint.json`. This project uses the current **`docs.json`** layout. Running **`npm run dev`** uses the pinned `mintlify` from `package.json`, which matches Mintlify’s current docs.

## API Endpoints

- **Authentication**: `POST /auth/token` — obtain JWT tokens
- **Campaigns**: `POST /campaign` — create or resolve campaigns

## Publishing Changes

Changes are typically deployed when pushed to the main branch.

## Support

For API support, contact [support@targeter.tech](mailto:support@targeter.tech).

## Resources

- [Targeter Dashboard](https://dashboard.targeter.tech)
- [API Status](https://status.targeter.tech)
