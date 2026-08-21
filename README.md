# Rhizome documentation

Mintlify documentation for Rhizome, an isolated lending protocol on Rootstock based on the Morpho Blue architecture.

## Local development

Requirements:

- Node.js 20 or newer
- npm or another Node.js package runner

From the repository root, start a local preview without a global install:

```bash
npx mint dev
```

The preview is available at `http://localhost:3000`. To prevent the CLI from opening a browser automatically, run `npx mint dev --no-open`.

Validate the site before opening a pull request:

```bash
npx mint validate
```

## Structure

- `docs.json` configures branding and navigation.
- Root-level `.mdx` files are documentation pages.
- `logo/` and `favicon.svg` contain site assets.

Keep pages concise and technical. Verify Rhizome-specific behavior against the protocol repositories. Use a clear `TODO` when a deployment, parameter, feature, API, SDK, audit, or integration cannot be verified.

## LLM-friendly documentation

Mintlify automatically publishes `/llms.txt` and `/llms-full.txt` for deployed documentation. Page frontmatter includes concise descriptions so the generated index is useful. No hand-maintained `llms.txt` is required.

## Source of truth

Protocol contracts and the canonical Rootstock deployment manifest live in [rhizomeprotocol/rhizome](https://github.com/rhizomeprotocol/rhizome). Indexed data is a historical read model; current safety-critical state must come from Rootstock RPC.
