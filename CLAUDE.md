# comp.thecrimson.com

Jekyll static site for The Harvard Crimson's semesterly comp (recruitment).
**One page.** The ten boards used to each have their own URL; the owner cut
those standalone pages entirely, so every board now lives only as a popup
card off the homepage board list (`_includes/board-panel.html`, opened from
`_includes/board-list.html`). Live production site for a student newspaper.
Deployed via **classic GitHub Pages from `master`**.

## Commands

```bash
bundle exec jekyll serve --livereload   # dev server -> http://localhost:4000
bundle exec jekyll build                # build into _site/
```

Ruby 3.3.6 via rbenv (see `.ruby-version`); Jekyll 3.10.0. **rbenv shims must
be ahead of system Ruby (2.6) on PATH** — Anaconda's `(base)` prefix can shadow
them, and you'll get a bundler error that looks like a missing gem.
**Editing `_config.yml` or `_data/` requires a server restart** — livereload
won't pick those up.

## THE BRANCH RULE — ABSOLUTE

All work happens on **`redesign`**.

- **NEVER** commit to `master`. **NEVER** push to `master`. **NEVER** force-push.
- `master` is live. Pushing to it deploys to students mid-comp.
- There are no preview URLs for non-`master` branches. **Local preview at
  localhost:4000 is the only preview that exists.**
- Merging to `master` is the owner's decision alone. Never initiate it.

## Where things live

Content is separated from templates on purpose. Never put prose in a template,
never put HTML or Liquid in a content file.

| Path | What it is |
|---|---|
| `index.md` | Homepage. Front matter for the headline; body is the intro prose. |
| `_boards/*.md` | **One file per board**, `output: false` -- data only, no page of its own. Front matter (`hook`, `photo`, `requirements`, `showcase`) + prose body. |
| `_sections/*.md` | Homepage prose blocks, ordered by `order`. `output: false`, so no URLs. |
| `_data/semester.yml` | Season, year, signup link, contact, newsletter/Instagram/X links, stats, tagline, events, hero photo, logo. Edited every cycle. |
| `_data/directors.yml` | All 19 directors, a plain list per board. Edited every cycle. |
| `_data/faq.yml` | Q&A pairs. **Only entries with a non-empty answer render.** |
| `_layouts/site.html` | The one shell: head, header, closing "Comp The Crimson" line, footer. |
| `_layouts/home.html` | The only page layout there is now -- everything renders on the homepage. |
| `_includes/board-list.html` | The ten typographic bands on the homepage; each is a `<details>` popup. |
| `_includes/board-panel.html` | One board's full content, rendered inside that popup -- description, requirements, Featured content, contacts. This is what used to be the standalone board page. |
| `_includes/drawer.html` | The nav panel (hamburger menu). Links jump to `/#slug` on the homepage, not to separate pages. |
| `css/main.css` | Everything. Design tokens at the top. |
| `_config.yml` | **Configuration only, no content.** Collections, kramdown, exclude list. |
| `CNAME` | **Never modify or delete.** Custom domain binding. |
| `_mockups/`, `_baseline/` | Design references from early in the redesign. Underscore-prefixed, so never published. |

Blank means hidden, never "empty slot": no `photo` renders no figure, no
`hero_photo` leaves the hero flat crimson, an empty `faq.yml` removes the whole
FAQ section. Optional fields are omitted rather than left as stubs.

## Constraints — do not violate

- **Stack:** Jekyll. Do **not** propose Astro/Next/11ty/Hugo. Do **not** add a
  JS framework or a Node build step.
- **The site ships ZERO JavaScript.** jQuery is gone and nothing replaced it.
  The nav drawer is a native `<details>`; motion is CSS scroll-driven
  animation. Keep it that way unless there is no alternative.
- **No new dependencies.** kramdown uses its own parser, not GFM, specifically
  to avoid the `kramdown-parser-gfm` gem — and because GFM turns a single
  newline into a `<br>`, which would inject line breaks when someone
  hard-wraps a paragraph. Image work uses `sips`, which ships with macOS.
- **Accessibility:** WCAG 2.2 AA. Non-negotiable — university-affiliated org.
- **Mobile:** mobile-first, genuinely. Most traffic and nearly all signups are
  phones.
- **Security:** repo is public. No secrets, tokens, or keys, ever.

## THE COPY RULE

**The owner and the boards write all prose. You do not.**

This is a student newspaper; the copy is the boards' own voice. Do not draft,
rewrite, tighten, or "improve" prose unless asked for that specific passage.

Permitted, because it moves text rather than authoring it: migrating copy
between files verbatim, converting HTML entities to real characters, and
reporting word counts or flagging stale facts. When a new field has no existing
copy, leave it empty and say so — never fill it with invented text. If you
catch yourself having written a headline, move it into a data field and flag it.

## Design tokens (owner-confirmed)

- **Crimson `#a82931`.** 6.64:1 on the `#fbfaf6` paper — AA.
- **Body ink `#15130f`** (17.76:1), **grey `#615c54`** (6.35:1).
- Muted text on colour uses solid tokens, **never `opacity`** — opacity
  multiplies against the background so the real ratio can't be verified.
- **The hero scrim is 88% and that number is derived.** Over a pure-white
  photo it resolves to 5.30:1 for paper text; at 80% it fails at 4.49:1.
- Fonts are the repo's own: League Gothic (display), Crimson (wordmark),
  Vollkorn (body), behind CSS custom properties so they swap in one line.

**Measure every colour before shipping it.** Three greys failed AA during this
redesign and each one looked fine by eye.

## Never do this

- Commit or push to `master`. Force-push anything.
- Touch `CNAME`.
- Add a JS framework, a CSS framework, a Node build step, or any gem, unasked.
- Put prose in templates, or HTML in content files.
- Run `git add -A` without checking what's new. That committed a 1.4MB `.ai`
  file, which is now stuck in history.
- Assume `.gitignore` keeps a file out of the build. **It does not** — Jekyll
  copies anything not in `_config.yml`'s `exclude`. An 18MB JPEG was being
  published until that was caught.
- Ship an `opacity: 0` starting frame on a scroll animation. Content that never
  enters its animation range stays invisible; animate transform only.
- Guess when uncertain — ask instead.
- Claim something renders correctly without having actually looked at it.
- Trust that a later, "more specific-looking" single-class override rule
  actually wins. `main.css` has one long cascade; two single-class selectors
  targeting the same property are equally specific regardless of which name
  sounds more targeted, so the one that's LOWER IN THE FILE silently wins —
  this has shipped real bugs twice. When overriding a shared class's
  property, write a compound selector (`.prose.board-card-prose`, not
  `.board-card-prose` alone) so the win doesn't depend on file order.
