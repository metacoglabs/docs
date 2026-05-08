# Tex Docs

The official documentation for [Tex](https://getmetacognition.com) — the memory layer for AI agents.

Hosted at **docs.getmetacognition.com** (Mintlify).

## Stack

- [Mintlify](https://mintlify.com) — MDX-based docs framework
- Diagrams via [Mermaid](https://mermaid.js.org)

## Run locally

```bash
npm i -g mintlify
mintlify dev
```

Open http://localhost:3000.

## Edit

- Page content lives in `*.mdx` files.
- Navigation is configured in [`mint.json`](./mint.json).
- Add a new page by creating the `.mdx` file and listing it under the right group in `mint.json`.

## Deploy

Push to `main`. The Mintlify GitHub app auto-deploys to docs.getmetacognition.com.

For a manual preview deploy: `mintlify deploy`.

## Style

- Friendly imperative tone — short sentences.
- Code examples wrapped in `<CodeGroup>` for multi-language.
- Use `<Steps>` for ordered procedures.
- Use `<CardGroup>` for navigational hubs.
- Use `<AccordionGroup>` for FAQ-style content.
- Diagrams via Mermaid blocks (` ```mermaid `).

## Structure

```
introduction.mdx        # landing
quickstart.mdx          # 5-min first call
authentication.mdx      # api keys, JWT, refresh

concepts/               # mental model
sdk/                    # Python SDK reference
api-reference/          # REST API
recipes/                # paste-ready integrations
migration/              # migrating from other systems
troubleshooting.mdx
changelog.mdx
```
