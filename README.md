# Rainfrog docs

Product documentation for [Rainfrog](https://www.rainfrog.ai) — the node-based AI studio at [app.rainfrog.ai](https://app.rainfrog.ai).

Built with [Mintlify](https://mintlify.com). Configuration lives in `docs.json`. Writing rules and content boundaries live in `AGENTS.md`.

## Local preview

```bash
npm i -g mint
mint dev
```

Open `http://localhost:3000`.

## What belongs here

User-facing Guide pages: concepts, studio, how-tos, plans, and FAQ.

Do **not** document AppSumo, backend architecture, admin tools, secrets, or console/DevTools troubleshooting. See `AGENTS.md`.

## Images

Product visuals live in `images/`. Prefer real studio or marketing product captures — do not invent UI mockups.

## Publishing

Push to the default branch after the Mintlify GitHub app is connected. Changes deploy automatically.
