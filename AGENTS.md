> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

{/* Add product-specific terms and preferred usage */}
{/* Example: Use "workspace" not "project", "member" not "user" */}

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

{/* Define what should and shouldn't be documented */}
{/* Example: Don't document internal admin features */}

## Cursor Cloud specific instructions

- This repo is a Mintlify docs site (MDX pages + `docs.json`). There is no `package.json`, no automated test suite, and no local build step — Mintlify builds and deploys via its GitHub app on push to the default branch.
- The only tool dependency is the global `mint` CLI, installed by the environment update script. Global npm installs are not user-writable here, so the update script installs with `sudo` while preserving `PATH` (nvm's npm). `mint` ends up at `/usr/bin/mint`.
- Run the dev server from the repo root (where `docs.json` lives): `mint dev` serves the preview at `http://localhost:3000`. Start it in a long-lived session (e.g. tmux); it is a foreground process.
- Validate content/links with `mint broken-links` (used here as the lint/check step).
- `mint dev` prints "Run mint login in the cli to activate search" — search requires auth, but login is NOT needed for local preview/rendering, so it is safe to ignore for local development.
- If the dev server misbehaves after a CLI change, run `mint update` to refresh the CLI.
