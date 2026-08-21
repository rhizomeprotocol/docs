# Rhizome documentation guidelines

This repository contains the Mintlify documentation for Rhizome.

## Technical sources

- Treat the Rhizome protocol contracts and canonical deployment manifests as the source of truth.
- Use Morpho documentation only as a conceptual reference. Verify Rhizome behavior against the pinned code.
- Distinguish unmodified upstream Morpho components from Rhizome-specific Rootstock configuration and code.
- Do not invent addresses, parameters, audits, APIs, SDKs, integrations, or deployment status. Add a clear `TODO` when a fact cannot be verified.
- Treat Rootstock RPC as authoritative for current protocol state. Indexed data is for discovery and history.

## Writing

- Write for readers who understand basic crypto concepts.
- Keep pages short, precise, and neutral.
- Avoid promotional language.
- Do not copy upstream documentation verbatim.
- Use sentence case for headings and concise page descriptions.

## Mintlify

- Pages are MDX files with YAML frontmatter.
- Configuration and navigation live in `docs.json`.
- Run `npx mint validate` after structural changes.
- Mintlify generates `/llms.txt` and `/llms-full.txt` automatically from navigable pages and their descriptions.
