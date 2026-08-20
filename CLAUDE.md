# comp.thecrimson.com

Jekyll static site for The Harvard Crimson's semesterly comp (recruitment).
11 pages: About Us (`index.html`) + 10 board pages. Live production site for a
student newspaper. Deployed via **classic GitHub Pages from `master`**.

## Commands

```bash
bundle exec jekyll serve --livereload   # dev server -> http://localhost:4000
bundle exec jekyll build                # build into _site/
```

Ruby 3.3.6 via rbenv; Jekyll 3.10.0. Anaconda may prefix the shell with
`(base)` — if Ruby tooling misbehaves, suspect PATH ordering first.
**Editing `_config.yml` requires a server restart** — livereload won't pick it up.

## THE BRANCH RULE — ABSOLUTE

All work happens on **`redesign`**.

- **NEVER** commit to `master`. **NEVER** push to `master`. **NEVER** force-push.
- `master` is live. Pushing to it deploys to students mid-comp.
- There are no preview URLs for non-`master` branches. **Local preview at
  localhost:4000 is the only preview that exists.**
- Merging to `master` is the owner's decision alone. Never initiate it.

## Layout of the repo

| Path | What it is |
|---|---|
| `_config.yml` | Semester data: season/year, nav, stats, signup link, all board directors' names + emails. |
| `_layouts/base.html` | Wrapper for the 10 board pages. |
| `_layouts/index_base.html` | `index.html` only. Duplicates `base.html` + adds splash screen. |
| `_includes/navbar.html` | Nav, built from `site.nav`, re-sorted alphabetically in Liquid. |
| `_includes/comp_director.html` | Renders "Name (mailto link)". |
| `*.html` (root) | The 11 content pages. Prose is currently tangled into markup. |
| `css/`, `js/`, `fonts/`, `images/` | Assets. See "Known cruft". |
| `CNAME` | **Never modify or delete.** Custom domain binding. |
| `_baseline/` | Pre-redesign screenshots, gitignored. Not deployed (Jekyll skips `_`-dirs). |

**Content vs. templates:** structured data (names, emails, dates, stats, links)
belongs in `_config.yml` / `_data/`. Prose belongs in content files. Templates
render; they do not hold copy. Keep these jobs strictly separate — never edit
content during design work, never edit templates during content work.

## Constraints — do not violate

- **Stack:** Jekyll. Do **not** propose Astro/Next/11ty/Hugo. Do **not** add a JS
  framework. Do **not** add a Node build step without explicit owner approval.
- **Dependencies:** a new volunteer student board with mixed skills inherits this
  every year. Every dependency is a tax on them. Justify each one, or omit it.
- **Accessibility:** WCAG 2.2 AA. Non-negotiable — university-affiliated org.
- **Mobile:** mobile-first, genuinely. Most traffic and nearly all signups are
  phones.
- **Security:** repo is public. No secrets, tokens, or keys in the tree, ever.
- **Scope:** ship good over perfect. Say so explicitly when a request does not
  fit the time available.

## Design intent

Modern and distinctive — **not** templated, **not** generic AI-startup aesthetic.
The owner's words: "sleek, sexy, cool." The current site is far too text-heavy;
the redesign must **communicate what matters** rather than paste in every
paragraph. Expect heavy copy cuts. Prefer boring, durable implementation
underneath a distinctive surface.

Editing copy must be trivially easy: open a plain content file, find the
paragraph in readable English, type over it. **No CMS, no admin UI, no
click-to-edit.** Flat over nested, keys in plain English, zero HTML in content
files. If the owner has to think about where a string lives, the design failed.

## Known cruft (audited, not yet fixed)

- **No `<meta name="viewport">` anywhere.** Phones render a 980px desktop layout
  scaled down; the `max-width:480px` CSS never fires on real devices. Biggest
  single mobile defect. Adding it will reflow everything — expect that.
- `_config.yml` holds **Spring 2026** data; a Jan. 31 2026 kickoff date is
  hardcoded in `index.html` prose.
- `blog.html` prose names last semester's directors ("We (Wyatt + Ava)").
- Business `dir2`: name `Arman Lateef` vs. email `hamza.lateef@` — mismatch.
- 16 of 19 font families in `fonts/` are never loaded. `Lato` is referenced in
  CSS but never loaded. `Big Caslon` is macOS-only with no fallback.
- `images/crimson-large.jpg` + `images/harvard.jpg` unreferenced (~1MB).
  `logo.png` is 714KB serving as a favicon.
- Google Analytics uses the deprecated `_gaq`/`ga.js` snippet (sunset by Google);
  duplicated in both layouts. Almost certainly collecting nothing.
- jQuery 3.3.1 from Google CDN powers only the mobile nav toggle and splash.

## Never do this

- Commit or push to `master`. Force-push anything.
- Touch `CNAME`.
- Add a JS framework, a CSS framework, or a Node build step unasked.
- Put prose in templates, or HTML in content files.
- Commit `_site/` or `_baseline/`.
- Guess when uncertain — ask instead.
- Claim something renders correctly without having actually looked at it.
