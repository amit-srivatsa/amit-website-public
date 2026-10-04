# Contributing

This repo is an archived snapshot of **v1.0** of amitsrivatsa.com. The live site (v3.0) is built from a private repo, so new features do not land here. Small fixes to this snapshot are welcome.

## Version numbers

The site is numbered `v{major}.{minor}`. The full history is in [VERSIONS.md](VERSIONS.md).

| Change | What happens to the number | Example |
|---|---|---|
| A complete facelift: new design system, new look | Major goes up, minor resets | v2.4 becomes **v3.0** |
| A meaningful change inside the same look: a feature, a page, a visible polish pass | Minor goes up | v3.0 becomes **v3.1** |
| A fix, copy edit, blog post, dependency bump or docs change | Stays the same | stays **v3.0** |

When a version bumps, add an entry to [VERSIONS.md](VERSIONS.md) in the same commit.

## Commit messages

Every commit message starts with the version the site is at **after** the commit, then a colon and a short summary in sentence case:

```
v{major}.{minor}: what changed
```

Good:

```
v1.0: fix broken LinkedIn link in footer
v3.1: add builds gallery page
v4.0: launch new site design
```

Not good:

```
fix footer                 (no version)
V1.0 - fix footer          (wrong case and separator)
v1: fix footer             (minor number missing)
```

Branch names follow the same idea: `v{major}.{minor}/short-description`, for example `v1.0/fix-footer-link`.

## Setting it up locally

Both steps are optional. The first fills in the format for you, the second stops a commit that forgets it.

```bash
git config commit.template .gitmessage
git config core.hooksPath .githooks
```

Merge and revert commits that git writes for you are allowed through the hook.
