> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is the Rainfrog product documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Audience: people using [app.rainfrog.ai](https://app.rainfrog.ai) who want to learn the product
- Prefer editing existing Guide pages over adding many new ones

## Terminology

| Prefer | Avoid / notes |
| --- | --- |
| **Character** | Do not use “Model” in user docs (internal code name) |
| **Image Generator** | Not a generic “Generator” that also produces video |
| **Video Generator** | Separate node from Image Generator |
| **Full Body Generator** / **Outfit Sheet Generator** | Specialized generators; name them explicitly |
| **Workflows** | Dashboard gallery of cloneable workflows |
| **Templates** | Fashion Shooting, Product Still Life, UGC — added from the **studio** canvas dock |
| **Assets** | Sidebar group for **Products**, **Characters**, and **Environments** |
| **Style** | Chosen on the Style node in studio (no separate Styles dashboard page) |
| **Manage Plan** | Its own nav item — not nested under Settings |
| **Credits** | Shown in the studio header; cost preview appears on the generator before you run |

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Describe what users see and do in the product — not how the system works internally
- Prefer “credit cost is shown on the generator before you run” over publishing fragile exact formulas

## Content boundaries

### Document

- User-facing studio, dashboard, libraries, generation, video, plans, and account flows
- UI labels that appear in the live product
- Public pricing and plan limits from marketing / in-app pricing

### Do not document

- AppSumo or lifetime deal programs
- Backend or architecture (billing sync, webhooks, databases, rate limits, abuse systems, storage paths, API routes, env vars, provider APIs)
- Admin CMS, internal analytics, or enterprise/org-only flags
- Secrets, API keys, service roles, or credentials of any kind
- Troubleshooting that tells users to open the browser console, DevTools, or inspect network requests
- Features that are not visible in the product UI

### Verification

Before stating prices, limits, or UI labels, check the live product or public marketing pricing — not code comments or fallbacks alone.
