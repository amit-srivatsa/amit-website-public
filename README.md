# amitsrivatsa.com, v1.0 (archived)

> **This is an old version of my website.** It does not look like the live site any more.
> The current site is **v3.0, "The Strategist's Deck"**, at [amitsrivatsa.com](https://amitsrivatsa.com).
> Its source lives in a private repo. This repo stays public as a reference for how v1 was built.

This repo is a public snapshot of the code behind **v1.0** of amitsrivatsa.com, the first Astro version of the site (March 2026). It was published on 23 April 2026, but the code inside matches the site as it was on 29 March 2026. It has not been updated since, and it will not be kept in sync with the live site.

## Which version is which

The site is numbered by look. Every complete facelift is a new major number. Smaller changes within the same look are minor numbers.

| Version | Dates | What it looked like | Where the code is |
|---|---|---|---|
| **v1.x** | Mar to Apr 2026 | "Hi, I'm Amit!" White pages, Inter, grey Tailwind palette, green availability dot, photo hero | **This repo (v1.0)** |
| v2.x | Apr to Sep 2026 | Career-focused redesign. "I help companies build content that compounds", skill mind map, logo work cards, dark header bar, later the Ask the agent chat | Private repo |
| **v3.0** | Oct 2026 to now | "The Strategist's Deck". Playing-card design system: paper, ink and magician's red, Fraunces and Inter Tight type, court-card hero deck | Private repo, **live today** |

The full history, with dates and commit ranges, is in [VERSIONS.md](VERSIONS.md).

## What is in this snapshot (v1.0)

- **[Astro 5](https://astro.build/)** with React islands for the interactive parts
- **[Tailwind CSS 3](https://tailwindcss.com/)** for styling
- **TypeScript** throughout
- Blog posts as Markdown in `src/content/blog/`

```
src/
├── components/       # Reusable UI components (Astro + React)
│   └── islands/      # Client-side interactive React islands
├── content/blog/     # Blog posts as Markdown files
├── layouts/          # Base page layout
├── pages/            # File-based routing (Astro pages)
├── styles/           # Global CSS
├── types/            # Shared TypeScript types
└── lib/              # Utility functions
public/               # Static assets
```

| Route | Description |
|-------|-------------|
| `/` | Home: hero, work history, services overview |
| `/cv` | Full CV |
| `/portfolio` | Selected work |
| `/services` | Service offerings |
| `/blog` and `/blog/[category]/[slug]` | Writing |
| `/resources` | Resource library |
| `/contact`, `/book` | Contact and booking |

### Running it locally

```bash
npm install
npm run dev
```

No environment variables are needed. The newsletter form will not submit without a backend, but every page renders.

### What was never in this repo

The live v1 site also had a Notion-backed newsletter, a subscriber admin view, an analytics dashboard and an ImageKit image pipeline. Those stayed private.

## Commit convention

Every commit in this repo starts with the site version it belongs to:

```
v{major}.{minor}: what changed
```

For example `v1.0: fix broken link in footer` or `v3.1: add builds gallery page`. The rules are in [CONTRIBUTING.md](CONTRIBUTING.md). To have git fill in the format for you:

```bash
git config commit.template .gitmessage
git config core.hooksPath .githooks   # optional: rejects commits without a version prefix
```

## About

I'm Amit Srivatsa, an AI-first content strategist based in the Netherlands, with 10+ years across Adobe, NetApp and Solid Optics. I build content systems that compound over time.

[amitsrivatsa.com](https://amitsrivatsa.com) · [LinkedIn](https://www.linkedin.com/in/amit-srivatsa/)
