# Plan: GitHub profile README alignment + LinkedIn audit (2026-09)

## Goal

Create internal artifacts for:

1. A rewritten GitHub profile README for `@vinibarbosabr/README.md`, aligned with current positioning from `resume.mdx`, `work.mdx`, `source-of-truth.md`, and `2026-09_career-assets-review.md`.
2. A LinkedIn audit and suggested changes for `in/viniciussb90`, since LinkedIn cannot be fetched anonymously.

User selected: **Portfolio-first** GitHub README tone, not heavily salesy.

## Source findings

Current README issues from career-assets review and user-provided text:

- Title is too broad: `Technical Writer & Docs Engineer | DevRel | Blockchain & Security`.
- Portfolio badge links to old `thecoding.framer.website`, not `https://thecoding.dev`.
- Uses forbidden `6+ years` claim; should use `since 2020`.
- Includes validator/delegation amounts and “top community delegate”, which conflict with no-amount/no-stake-sales rules.
- Contains typo `Docusauros`; Docusaurus is not strongly evidenced.
- Contains likely dead/private P2P.me PR link; should not be presented as verifiable link unless public.
- Missing current 0xramp docs + SDK lead work, which is now the strongest recent proof.
- Missing canonical links to `thecoding.dev/work`, `/resume`, `/contact`.
- Uses em dashes; current style avoids them.
- “Security Researcher” framing should be avoided; use security writing/postmortems only.

LinkedIn cannot be audited directly due to HTTP 999. The deliverable should be a manual checklist and recommended copy.

## Deliverables in `internal/`

Recommended structure:

- `internal/career-assets/github-profile-readme.md`
  - Final polished GitHub README draft, ready to paste into `@vinibarbosabr/README.md`.
- `internal/career-assets/linkedin-audit-2026-09.md`
  - LinkedIn checklist, headline options, About draft, experience alignment, featured links, skills, recommendations, cleanup.
- Optional: keep plan file at `.opencode/plans/github-readme-linkedin-alignment.md` for session plan.

## GitHub README structure

Portfolio-first, concise, proof-linked:

1. Header: name + role line.
   - Recommended role line: `Documentation Engineer & Technical Writer · Developer Education · Blockchain & Security Writing`.
2. Badges/links: thecoding.dev, LinkedIn, Substack, X. No old Framer link.
3. One-paragraph positioning:
   - Since 2020.
   - Documentation engineering + developer education.
   - Read code, test flows, ship docs/content.
4. Current work:
   - 0xramp labs: docs site + partner SDK lead.
   - thecoding.dev: public docs-as-code portfolio.
5. Selected work:
   - Dash GroveDB, Dash Orchard, MultiversX Andromeda, HackenProof, Storage Cost Attacks on NEAR, Quai Starter Pack.
   - MultiversX Brazil developer education.
   - Nano Foundation education articles.
6. Open-source / community table:
   - `0xramp-docs`, `0xramp-sdk`, `erc4337-driver`, `near/docs`, `multiversx/mx-docs`, `near-daos/sputnik-dao-contract`.
   - Exclude P2P.me link unless public; can mention without link or remove.
7. Skills:
   - Documentation and writing.
   - Engineering.
   - Ecosystems.
   - Education.
8. Contact:
   - Portfolio, work, contact page, email.
   - No pressure language.
9. Footer line:
   - “Building documentation that scales with engineering teams.”

Constraints:

- No em dashes.
- No audience counts, delegation amounts, or stake dollar values.
- No `6+ years`.
- No `Security Researcher` identity.
- No `call/chat`; use `brief` or `briefing` if mentioning work.
- Avoid overclaiming 0xramp role; use “docs site and partner SDK lead” or “co-builder, documentation and SDK lead” consistent with resume.

## LinkedIn audit recommendations

Since actual profile cannot be fetched, create manual audit sheet:

1. Headline:
   - Recommended: `Documentation Engineer & Technical Writer · Developer Education · web3 docs-as-code`
   - Avoid: KOL, influencer, “Security Researcher”, too many titles.
2. About:
   - 3 paragraphs: positioning, proof, CTA.
   - Include canonical links.
3. Experience:
   - Add/update 0xramp labs as current role.
   - Add/update thecoding founder/contractor role.
   - Mirror resume dates and wording.
4. Featured:
   - Pin `thecoding.dev`, `/work`, `docs.0xramp.app`, best Substack article.
5. Skills:
   - Put documentation skills first: Technical Writing, Documentation, Docs-as-code, Developer Education, API/SDK Documentation, Information Architecture, Mintlify, Markdown/MDX, Git.
6. Recommendations:
   - Request from 0xramp lead developer and Dash contact if appropriate.
7. Cleanup:
   - Remove follower counts, delegation amounts, top delegate claims, old portfolio links.
   - Ensure all links go to canonical properties.

## Additional improvement recommendations

- Make `resume.mdx` the master source. Any future change should cascade to GitHub README and LinkedIn.
- Pin `thecoding-docs` and `erc4337-driver` on GitHub profile if possible.
- If the 0xramp SDK can be published to npm, do it; it strengthens engineering credibility.
- Add a short “Now” line to GitHub README only if it can be maintained.
- Verify all public links quarterly.
- Consider adding GitHub profile README to the Phase 7 consistency sweep.

## Execution steps after approval

1. Create `internal/career-assets/` directory.
2. Write `github-profile-readme.md` with final README.
3. Write `linkedin-audit-2026-09.md` with audit and copy suggestions.
4. Optionally update `internal/2026-09_career-assets-review.md` with note that GitHub README draft and LinkedIn checklist now exist, if user wants.
5. Do not edit the actual GitHub profile README repository from here unless user provides that repo or asks to push.

## User decisions

- P2P.me: keep as text only, no broken link.
- Email: keep `vinibarbosabr@proton.me` public in GitHub README.
- Artifacts: save under `internal/career-assets/`.
- 0xramp role: use “co-builder, docs and partner SDK lead” to match resume/work.

## Updated GitHub README draft

```markdown
<div align="center">

# Vini Barbosa

**Documentation Engineer & Technical Writer** · **Developer Education** · **Blockchain & Security Writing**

[![Portfolio](https://img.shields.io/badge/thecoding.dev-Portfolio-111827?style=for-the-badge&logo=googlechrome&logoColor=white)](https://thecoding.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/viniciussb90/)
[![Substack](https://img.shields.io/badge/Substack-FF6719?style=for-the-badge&logo=substack&logoColor=white)](https://thecoding.substack.com)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/vinibarbosabr)

Brazil · Remote · Open to documentation and developer-education work

</div>

I write about web3 protocols, developer tools, and security since 2020. My work sits at the intersection of documentation engineering and developer education: I read code, test flows, organize information, and ship documentation or technical content that developers can actually use.

## What I do

- **Documentation engineering**: docs-as-code, information architecture, docs health checks, section rebuilds, API and SDK documentation
- **Developer education**: tutorials, research articles, guides, workshops, onboarding paths, education-shaped DevRel
- **Security writing**: technical explainers, research summaries, and postmortem-style writing, not audits

## Current work

- **0xramp labs**: co-builder, docs site and partner SDK lead for a non-custodial fiat-to-crypto ramp  
  [docs.0xramp.app](https://docs.0xramp.app) · [0xramp-docs](https://github.com/0xramp-labs/0xramp-docs) · [0xramp-sdk](https://github.com/0xramp-labs/0xramp-sdk)
- **thecoding.dev**: my portfolio and services site, built and overhauled docs-as-code in the open  
  [thecoding.dev](https://thecoding.dev) · [thecoding-docs repo](https://github.com/vinibarbosabr/thecoding-docs)

## Selected work

- [Dash: GroveDB deep dive](https://thecoding.substack.com/p/a-look-at-grovedb-making-blockchains), sponsored research article
- [Dash Orchard explainer](https://thecoding.substack.com/p/dash-orchard-zcash-privacy-rebuilt), sponsored research article
- [MultiversX Andromeda blog post](https://multiversx.com/blog/andromeda-supernova-highspeed-highways), engineering update
- [HackenProof: How to Become a Bug Bounty Hunter](https://hackenproof.com/blog/how-to-become-a-bug-bounty-hunter), guest article
- [Storage Cost Attacks on NEAR](https://thecoding.substack.com/p/storage-cost-attacks-on-near-explained), protocol research
- [Quai Starter Pack](https://thecoding.substack.com/p/quai-starter-pack-a-quickstart-guide), sponsored tutorial
- MultiversX developer education in Brazil: meetup, newsletter, Telegram group, and mentorship support
- Nano Foundation education articles during my community lead tenure

More examples with context: [thecoding.dev/work](https://thecoding.dev/work)

## Open source and community

| Project | Contribution |
| --- | --- |
| [0xramp-docs](https://github.com/0xramp-labs/0xramp-docs) | Documentation architecture, Mintlify docs, partner-facing guides |
| [0xramp-sdk](https://github.com/0xramp-labs/0xramp-sdk) | Partner SDK documentation, `SPEC.md`, `DESIGN.md`, partner guide |
| [erc4337-driver](https://github.com/vinibarbosabr/erc4337-driver) | TypeScript library for driving an existing thirdweb ERC-4337 account from any EIP-1193 provider |
| [near/docs](https://github.com/near/docs) | Documentation contributions |
| [multiversx/mx-docs](https://github.com/multiversx/mx-docs) | Documentation reviews and structural proposals |
| [near-daos/sputnik-dao-contract](https://github.com/near-daos/sputnik-dao-contract) | Research and documentation issues |
| P2P.me | Documentation contribution on smart-account and fund-recovery behavior, repo link unavailable |

## Skills

**Documentation and writing**: docs-as-code, Git and GitHub workflows, Markdown/MDX, Mintlify, mdBook, information architecture, API and SDK documentation, style guides  
**Engineering**: TypeScript, Rust, Python, Solidity, Foundry, Linux, Neovim  
**Ecosystems**: NEAR, MultiversX, Zcash, Nano, EVM, validator and governance participation  
**Education**: tutorials, workshops, talks, mentorship, onboarding paths

## Contact

Portfolio and work samples: [thecoding.dev](https://thecoding.dev)  
Work inquiries: [thecoding.dev/contact](https://thecoding.dev/contact)  
Email: [vinibarbosabr@proton.me](mailto:vinibarbosabr@proton.me)

---

<div align="center">

**Building documentation that scales with engineering teams.**

</div>
```

## LinkedIn audit draft outline

File: `internal/career-assets/linkedin-audit-2026-09.md`

- Note that LinkedIn cannot be fetched anonymously; audit is a manual checklist.
- Headline options.
- About section draft.
- Experience entries to mirror `resume.mdx`:
  - 0xramp labs: co-builder, docs and partner SDK lead, 2026 to present.
  - thecoding: founder/independent contractor, March 2026 to present.
  - Independent technical writer/docs contributor/DevRel, 2020 to February 2026.
  - Finbold technical editor/news reporter, August 2023 to March 2025, technical editor from March 2024.
  - Nano Foundation community lead, July 2023 to September 2024, part-time; Brazilian ambassador September 2021 to June 2023.
  - Portal do Bitcoin technical journalist, April 2023 to August 2023.
  - Cointimes research/content, November 2021 to February 2023, research lead from November 2022.
  - Earlier roles summarized.
- Featured links:
  - `https://thecoding.dev`
  - `https://thecoding.dev/work`
  - `https://docs.0xramp.app`
  - Dash GroveDB article or Substack
- Skills reorder and additions.
- Recommendations to request.
- Cleanup checklist: remove old Framer link, 6+ years, delegation amounts, audience counts, “security researcher” identity, KOL language.
