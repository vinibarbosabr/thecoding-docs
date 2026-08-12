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
├── technical-writing.mdx  # Sponsored content lane (to be expanded)
├── documentation.mdx      # Docs engineering lane (to be expanded)
├── devrel.mdx             # DevRel lane (to be expanded)
├── public/                # Static assets (images, banners)
├── logo/                  # Light & dark logos
└── README.md
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

Clients and partners can leave public recommendations by opening a Pull Request.

1. Fork the repository (or create a branch if you have write access).
2. Add a new file under a `recommendations/` folder (or follow the template on the site).
3. Include:

- Your name / project
- Role / relationship
- Short testimonial (2-6 sentences)
- Optional: link to the related work or project
1. Open a PR with a clear title, e.g. `recommendation: [Project Name]`.

Recommendations are reviewed and merged. Once merged, they appear on the public **Recommendations & Endorsements** page.
A simpler form-based flow may be added later. For now, the pure Github PR approach keeps everything transparent and version-controlled.

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
