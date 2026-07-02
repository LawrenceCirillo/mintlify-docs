# Home Service Data — Mintlify docs

## About this project

- Documentation for [Home Service Data](https://homeservicedata.org), deployed at `https://homeservicedata.mintlify.app`
- Source repo: `https://github.com/LawrenceCirillo/mintlify-docs`
- App codebase lives in the sibling `homeservicedataapp` workspace (`app/`)
- Pages are MDX with YAML frontmatter; site config is `docs.json`
- Preview locally: `mint dev` from this directory (requires [Mintlify CLI](https://www.npmjs.com/package/mint))

## How to edit

1. **Direct edits (preferred in Cursor):** change MDX files here, commit, and push to `main`. Mintlify deploys from GitHub.
2. **Search/read live content:** MCP server `https://homeservicedata.mintlify.app/mcp`
3. **Admin MCP (PR workflow):** `https://mcp.mintlify.com` — requires OAuth login in Cursor MCP settings

When app behavior changes, update the matching docs page and keep API examples aligned with `app/app/api/v1/`.

## Terminology

- **Home Service Data** / **HSD** — the product and API platform
- **Quote-safe** — records approved for customer-facing quotes (`quote_safe: true`)
- **Context-only** — background data; must not drive live quote math (`quote_safe: false`)
- **Data packet** — a typed dataset slice (finance, equipment, incentives, etc.)
- **Access level** — `sample`, `sandbox`, or `production` scope on an API key
- **Quote context** — composite `/quote-context` response bundling finance, equipment, incentives, and local context
- **Sync** — snapshot + delta endpoints for keeping a local database current

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and API fields
- Prefer real endpoint paths and JSON shapes that match production responses

## Content boundaries

- Document the public REST API, dashboard workflows, and integration guides
- Do not document internal admin ingestion pipelines or unreleased endpoints
- Do not expose secrets, API keys, or internal Supabase details
- Link to `https://homeservicedata.org/dashboard` and `https://homeservicedata.org/contact` for product actions
