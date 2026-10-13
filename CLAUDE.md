# Project: jillmetcalfe.com (landing page)

## About the user
- Jill is not a coder. Explain terminal commands, git and technical ideas in plain language.
- ADHD mode: lead with the action, number steps, give time estimates, end with one next step.

## What this is
The landing page for Jill's **AI staff training** business (workshops for teams, not executive coaching).
- `index.html`: the whole page. `static/style.css`: all styling. `404.html`: page-not-found.
- **No framework, no build step, no CSS framework.** Same rule as the blog. Don't add one.
- Hosted on GitHub Pages from `main` (repo `jillmetcalfe/jillmetcalfe-com`), custom domain in `CNAME`.
- Cloudflare proxies the domain. A redirect rule sends the blog's old paths (`/blog/`, `/bookshelf/`,
  `/now/`, `/projects/`, `/assets/`, `/feed.xml`, `/sitemap.xml`) to blog.jillmetcalfe.com.
  **Never put landing-page files under those paths.** Our files live in `static/`.
- Claude has no Cloudflare access. Jill makes dashboard changes; give her exact values.

## Words on the page
- Claude drafted the starting copy at Jill's request; Jill rewrites it over time.
- Every Claude-drafted block is wrapped in `<!-- DRAFT: Claude wrote this, Jill to rewrite -->` …
  `<!-- /DRAFT -->`. When Jill rewrites a block she removes the markers. Never re-add markers to
  text she's written, and never "improve" her wording unasked.
- English only, permanently. No translations.

## Design
Placeholder look, inspired by Every.to with a teal accent. Final branding is still to be decided,
so every colour, font and spacing value is a CSS variable at the top of `static/style.css`.

## Privacy
This repo is public. Working notes (`HANDOFF.md`, `NOTES.md`, `docs/`) are gitignored on purpose.
Don't commit them.

## Tracking work in Notion
Same conventions as the blog repo's `CLAUDE.md` → "Tracking work in Notion".
Project page: jillmetcalfe.com (`a59d166b60be4e409521263e36a9a484`).

## Conventions
- Update `CHANGELOG.md` in plain language when something visible changes.
