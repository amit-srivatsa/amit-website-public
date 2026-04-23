# amitsrivatsa.com — public source reference

This is a cleaned-up, public snapshot of the source code behind [amitsrivatsa.com](https://amitsrivatsa.com). It's updated roughly once a quarter. The live site runs on a private repo with additional integrations not included here.

## Stack

- **[Astro 5](https://astro.build/)** — static site generator with component islands
- **[React 19](https://react.dev/)** — interactive UI components via Astro islands
- **[Tailwind CSS 3](https://tailwindcss.com/)** — utility-first styling
- **[TypeScript](https://www.typescriptlang.org/)** — throughout

## Structure

```
src/
├── components/       # Reusable UI components (Astro + React)
│   └── islands/      # Client-side interactive React islands
├── content/
│   └── blog/         # Blog posts as Markdown files
├── layouts/          # Base page layout
├── pages/            # File-based routing (Astro pages)
├── styles/           # Global CSS
├── types/            # Shared TypeScript types
└── lib/              # Utility functions
public/               # Static assets (images, logos, PDFs)
```

## Pages

| Route | Description |
|-------|-------------|
| `/` | Home — hero, work history, services overview |
| `/cv` | Full curriculum vitae |
| `/portfolio` | Selected work |
| `/services` | Service offerings |
| `/blog` | Writing index |
| `/blog/[category]/[slug]` | Individual blog posts |
| `/resources` | Resource library |
| `/contact` | Contact |
| `/book` | Book a consultation |

## Running locally

```bash
npm install
npm run dev
```

No environment variables are required to run the site locally — the newsletter subscription form won't submit without a backend, but everything else renders fine.

## What's not in this repo

The live site has server-side features not included here:

- Newsletter subscription backend (Notion API integration)
- Subscriber management admin dashboard
- Analytics dashboard
- Image optimization pipeline (ImageKit)

## About

I'm Amit Srivatsa — AI-first content strategist based in the Netherlands. 10+ years across Adobe, NetApp, and Solid Optics. I help companies build content systems that compound over time.

→ [amitsrivatsa.com](https://amitsrivatsa.com)  
→ [LinkedIn](https://www.linkedin.com/in/amit-srivatsa/)
