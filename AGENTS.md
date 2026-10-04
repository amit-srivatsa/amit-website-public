# AGENTS.md

Rules for AI coding agents (Claude Code, Codex, Cursor and others) working in this repo.

## What this repo is

An archived public snapshot of **v1.0** of amitsrivatsa.com. The live site is **v3.0** and is built from a private repo. Do not try to make this repo match the live site, and do not copy private code, secrets or personal data into it.

## Commit messages (required)

Every commit message starts with a site version: `v{major}.{minor}: what changed`.

- Major goes up only for a complete facelift. Minor goes up for a meaningful change within the same look.
- Fixes, copy, blog posts, dependency bumps and docs keep the current number.
- In this repo that almost always means `v1.0: ...`.
- If a change bumps the version, add an entry to `VERSIONS.md` in the same commit.
- Name branches `v{major}.{minor}/short-description`.

Full rules: `CONTRIBUTING.md`. History: `VERSIONS.md`.

## Writing style

No em dashes or en dashes in any file, commit message or PR text.
