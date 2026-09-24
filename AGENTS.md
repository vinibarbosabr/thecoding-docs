# Documentation project instructions

## About this project

- **thecoding.dev** — services portfolio and contractor landing site for **Vini B | thecoding** (Vini Barbosa, `@vinibarbosabr`)
- Built on [Mintlify](https://mintlify.com) (Palm theme). Pages are MDX files with YAML frontmatter in the repo root; configuration lives in `docs.json`
- Deploy: push to `main` → Mintlify GitHub App rebuilds automatically. QA on local preview (`mint dev`) or branch previews before anything reaches `main`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP; use `https://www.mintlify.com/docs/mcp` for Mintlify product knowledge

## Active work: 2026-09 buyer-path docs overhaul

This overhaul doubles as a public docs-as-code case study for thecoding.dev.
Brief and progress log: `internal/OVERHAUL.md` (gitignored, kept out of the public repo). Public tracking: [milestone 1 — Overhaul: buyer path (2026-09)](https://github.com/vinibarbosabr/thecoding-docs/milestone/1) · starter issue #4 · per-phase follow-on issues.

Roadmap checklist — a phase starts only when the previous phase's exit criteria are met:

- [x] Phase 0 — Setup: branch, brief (`internal/OVERHAUL.md`), success test, scope freeze, repo audit
- [x] Phase 1 — Briefing: audience, job-to-be-done, primary CTA, cut list, non-goals
- [x] Phase 2 — Inventory & audit: page-by-page buyer-job table + proof inventory (no copy rewrites) *(issue #6)*
- [x] Phase 3 — Source of truth: freeze positioning, lane names, SKUs, forbidden phrases, CTA model
- [x] Phase 4 — Information architecture: `docs.json` nav only, navbar CTA swap *(issue #8)*
- [ ] Phase 5 — Proof: new `/work` page (≥3 honest cards) + endorsements cleanup
- [ ] Phase 6 — Conversion path: pricing → quickstart → contact → service pages (`developer-education.mdx`) → home (last) → demote the rest
- [ ] Phase 7 — Chrome & consistency: shared CTAs, metadata, links, create `llms.txt`, verify redirects, mobile nav QA, full QA click-through
- [ ] Phase 8 — Revision & ship: revision pass against the brief, release to `main`, handoff note

## How we work

- One concern per PR; feature PRs target the overhaul branch, not `main` (the site deploys from `main`)
- Conventional commit prefixes: `docs:`, `feat:`, `fix:`, `chore:`
- No unpublished claims: only state what the proof inventory allows
- Inventory before adjectives; structure before sentences; pricing and quickstart before the homepage
- Every old URL must keep working; this run changes titles, not slugs, with one sanctioned exception: the Developer Education merge (`/devrel` + `/technical-writing` → `/developer-education`, with redirects)
- Keep a clean paper trail: the PR history is part of the public case study

## Public vs internal

- Everything tracked in git is public (`AGENTS.md`, all MDX) — write accordingly
- Sensitive, security-related, or internal-only notes belong in `internal/` (gitignored)
- Never commit secrets, keys, private client data, or NDA-restricted details (anonymize or omit)

## Terminology

- Lane and SKU names are frozen in Phase 3 (`internal/source-of-truth.md` once it exists); until then, do not rename lanes or SKUs in copy
- Decided 2026-09-23: target shape is **two commercial lanes** — Documentation Engineering and **Developer Education** (merge of technical-writing + devrel). `Technical Education` stays a product name, never a lane. Details in `internal/OVERHAUL.md` decision log
- Primary action is a **briefing** (send a brief / book 20 minutes), not a "call" or "chat"

## Style preferences

- Active voice, second person ("you"); one idea per sentence
- Sentence case for headings; bold for UI elements (Click **Settings**); code formatting for file names, commands, paths
- Frontmatter `title` is the page header — do not add a duplicate manual H1 (convention normalized in Phase 6–7)
- Lead with the job and the work, not biography or audience-size claims
- No em dashes (`—`) in copy: use commas, colons, periods, or restructure the sentence
- Simple, clear language; short sentences; no heavy jargon, copy-heavy tone, or ad-like urgency
- No reach or engagement numbers (followers, subscribers, likes, views, attendees) in sales or proof copy; deliverable counts (words, issues, PRs) are fine
- Conversion comes from clarity and proof, never pressure; the reader is technical

## Content boundaries

- This is a contractor sales site, not a blog or CV: nav matches the offer
- The staking page serves existing delegators; it stays out of the sales path and sales copy
- Security-research framing is limited to writing and postmortems; not selling audits
