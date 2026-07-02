# Home Service Data Mintlify Docs

This is the buyer-visible documentation site for Home Service Data, deployed with Mintlify.

- Production docs: `https://docs.homeservicedata.org`
- Mintlify app URL: `https://homeservicedata.mintlify.app`
- Product app: `https://homeservicedata.org`
- Source app workspace: sibling repo `homeservicedataapp/app`

## Edit Locally

Run from this directory:

```bash
mint dev
```

Install or update the Mintlify CLI if needed:

```bash
npm i -g mint
mint update
```

## Content Rules

- Keep endpoint examples aligned with `https://homeservicedata.org/api/openapi`.
- Use `https://homeservicedata.org` for product, dashboard, and API examples.
- Do not publish secrets, demo credentials, Supabase service keys, or internal dashboard access details.
- Keep dashboard docs focused on customer-visible surfaces: Catalog, Playground, API Keys, Sync Health, and Webhooks.
- When API behavior changes, update the API reference, quickstart, and relevant guide in the same pass.

## Useful Checks

Before publishing, search for stale `.com` API/product domains, old webhook-secret examples, and old Settings-based webhook navigation. Expected result: no matches outside intentional changelog notes.
