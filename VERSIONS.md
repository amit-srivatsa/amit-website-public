# Version history of amitsrivatsa.com

This file numbers every version of the site, from the first Astro build to what is live today.

## How the numbers work

- **Major (v1, v2, v3):** a complete facelift. New design system, new look, new first impression.
- **Minor (v2.1, v2.2):** a meaningful change inside the same look. A new feature, a new page, a visible polish pass.
- Fixes, copy edits, new blog posts and docs keep the current number. They do not bump anything.

## Where the history comes from

This public repo holds a snapshot of **v1.0**. The day-to-day history lives in the private repo that builds the live site. The commit ranges below are short hashes from that private repo, listed so the versions can be traced. Git history before 29 March 2026 was not kept, so v1.0 is the earliest version on record.

## Summary

| Version | Dates | Commits (private repo) | Headline |
|---|---|---|---|
| v1.0 | 29 Mar 2026 | `eff8cf5` to `2949ec3` (16) | First Astro site, "Hi, I'm Amit!" |
| v1.1 | 30 Mar to 8 Apr 2026 | `dcd3612` to `e1b164e` (22) | Content backend: CMS experiments and an admin dashboard |
| v1.2 | 8 Apr 2026 | `38a2f29` to `0d79bbc` (3) | Site-wide dark mode toggle |
| **v2.0** | 22 Apr 2026 | `a29595f` to `9fd39fd` (8) | **Facelift:** career-focused redesign |
| v2.1 | 23 Apr 2026 | `4d2c55c` to `f4b814b` (11) | Recruiter polish, dark header, animated skills diagram |
| v2.2 | 3 Jun to 16 Jul 2026 | `f8ed9bc` to `f8dffa5` (3) | Dark mode switched off, blog fixes |
| v2.3 | 28 Jul to 7 Aug 2026 | `3e58bb6` to `d6970c7` (15) | Ask the agent: recruiter chat on every page |
| v2.4 | 8 to 9 Sep 2026 | `4fd3c49` to `4a7280b` (2) | New portfolio cards |
| **v3.0** | 2 Oct 2026 to now | `b81b7c6` to `d0cd945` (4) | **Facelift:** "The Strategist's Deck". **Live today.** |

## v1: "Hi, I'm Amit!"

White pages, Inter type, a grey Tailwind palette and a green "available" dot. A photo hero opened with "Hi, I'm Amit!", followed by work history and a services overview.

### v1.0 (29 March 2026)

The first version of the site on Astro 5 with React islands. Blog posts came from Notion with ImageKit-hosted covers, and a newsletter form wrote to Notion. **This repo is a snapshot of v1.0.**

### v1.1 (30 March to 8 April 2026)

Same look, new plumbing. The Notion sync got safer, the blog briefly moved to the Keystatic CMS and then back to plain Markdown in git, and a private admin dashboard appeared at `/admin`.

### v1.2 (8 April 2026)

A dark mode toggle across every page, with the choice remembered between visits.

## v2: career-focused redesign

A full rethink aimed at hiring managers. The hero changed to "I help companies build content that compounds" with a "Looking for new roles in the NL/EU" tag. The metrics card became a skill mind map, and work history became logo cards with one-line outcomes.

### v2.0 (22 April 2026)

The new design system shipped, then work items moved into a three-column card grid with descriptions always visible.

### v2.1 (23 April 2026)

Services rewritten for recruiters, the dark mode toggle removed, an MWS logo added, a dark header bar made the default, and the skills diagram redrawn with animated chips. The footer started linking to this public repo.

### v2.2 (3 June to 16 July 2026)

Dark mode switched off site-wide because it looked broken, plus a new blog post and a fix for blog cover images.

### v2.3 (28 July to 7 August 2026)

The career agent arrived: a chat widget on every page and a dedicated `/agent` page, surfaced as "Ask the agent" in the nav. Also an SEO pass, corrected booking links and location, and the downloadable resume PDF removed from the site.

### v2.4 (8 to 9 September 2026)

New portfolio cards for the Ask the agent project and TracXon.

## v3: "The Strategist's Deck"

A playing-card design system drawn from card magic and the Magic Wand brand. Paper, ink, magician's red and chai colours. Fraunces for display type, Inter Tight for body, JetBrains Mono for labels. Custom card suits, a court-card hero deck with a shuffle, and chess, compass and system-stack illustrations. Portfolio and CV now render on the server, and there is a proper 404 page.

### v3.0 (2 October 2026 to now)

**This is the live site at [amitsrivatsa.com](https://amitsrivatsa.com).** Since launch it has also gained a Health Tracker portfolio card, a new blog post and a footer link to the LinkedIn newsletter.

### Next: v3.1 (in progress)

A permanent `/builds` gallery for the Buildtober series, styled as printed playing cards. Not live yet.
