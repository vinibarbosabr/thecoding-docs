# thecoding

> Services portfolio and independent contractor landing website for **Vini B | thecoding**, by **Vini Barbosa** (`@vinibarbosabr`).

**Live site:** [thecoding.dev](https://thecoding.dev)

This repository powers the public documentation and services site for **thecoding**.  
It is built with [Mintlify](https://mintlify.com) using the **Palm** theme and follows a docs-as-code approach.

---

## What is thecoding?

**thecoding** is the independent contractor brand of Vini Barbosa (Vini B) — a technical writer, documentation engineer, developer relations partner, and security researcher focused on blockchain and Web3.

Main service lanes:

- **Sponsored Technical Content** — deep research articles, tutorials, and educational material published on thecoding channels (Substack + X + LinkedIn).
- **Documentation Engineering** — docs audits, focused sprints, full overhauls, and ongoing docs ownership (docs-as-code).
- **DevRel Partner** — workshops, talks, community support, and developer education.

The site also hosts selected portfolio work, open recommendations from clients/partners, and practical entry points to start a project.

---

## Repository structure

```text
.
├── docs.json              # Mintlify configuration (navigation, theme, colors, footer)
├── index.mdx              # About / Welcome
├── quickstart.mdx         # How to start a project
├── pricing.mdx            # Pricing terms and fixed rates table
├── technical-writing.mdx  # Sponsored content lane
├── documentation.mdx      # Docs engineering lane
├── devrel.mdx             # DevRel lane
├── resume.mdx             # Vini B professional resume & portfolio
├── endorsements.mdx       # Public recommendations, testimonies, and endorsements
├── contact.mdx            # Contact links (Signal, Telegram, Email) and form
├── staking.mdx            # Guide on how to stake NEAR with thecoding.pool.near
├── terms.mdx              # Terms of service
├── public/                # Static assets (images, banners)
├── logo/                  # Light & dark logos
└── README.md              # <-- You are here!
```

Navigation is defined in `docs.json`. New pages are added as `.mdx` files and registered in the navigation groups.

## Local development

```Bash
# Install Mintlify CLI
npm i -g mint

# Run local preview (from the repo root)
mint dev
```

Open <http://localhost:3000>.

## How the site is updated & deployed

1. Make changes in this repository (edit .mdx files or docs.json).
2. Push to the main branch.
3. Mintlify automatically rebuilds and deploys the site (GitHub App integration).

There is no manual build step required for production.

## Theme & stack

Platform: [Mintlify](https://mintlify.com/)
Theme: [Palm](https://palm.mintlify.site/)
Content format: [MDX](https://github.com/mdx-js/mdx/)
Primary colors: defined in docs.json (#042F2E, #FFF3CE, #008BBE)

This site itself is an example of the documentation engineering work offered by thecoding.

## Contributing / Leaving a recommendation

This repository is public by design and follows Free (Libre) Open-Source Software practices/ethos.

### Recommendations & Endorsements

Clients, collaborators, and community members can leave public recommendations via a **GitHub issue form** — no fork or pull request needed.

1. Open the issue form:
   `https://github.com/vinibarbosabr/thecoding-docs/issues/new?template=endorsement.yml`
2. Fill in the short form with your name, role, company/project, an optional link, and your recommendation (2–6 sentences).
3. Hit submit.

Approved recommendations are published to the public **Recommendations & Endorsements** page and the issue is then closed.

### Other Contributions

Bug reports, typos, broken links, and small improvements are highly welcome via Issues or PRs.

## Contact

- Email: [thecoding@proton.me](mailto:thecoding@proton.me)
- X: [@vinibarbosabr](https://x.com/vinibarbosabr)
- Signal: [@vinib90](https://signal.me/#eu/xzhT7ZjGlbwTMVtZr8v-NUonD7NuPtFd4UbyMsRNFOJ-Jh4HjKxAG4uIlu5hdFdq)
- Telegram: [@vinibarbosa](https://t.me/vinibarbosa)
- Book a call: [CalCom/vinib](https://cal.com/vinib)

## License

MIT
