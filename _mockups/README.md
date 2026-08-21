# Design mockups

Static design references for the redesign. **Not part of the site** — Jekyll
skips underscore-prefixed directories, so nothing here is ever published.

## How to view

These reference `../fonts/` and `../images/`, so they need to be served from the
**repo root** — not opened as `file://` (Chrome blocks webfont loading over
`file://`, so the type would silently fall back to Georgia and the whole point
would be lost).

```bash
cd ~/Projects/comp-site
python3 -m http.server 4002
# then open http://localhost:4002/_mockups/hub.html
```

Don't use `bundle exec jekyll serve` for this — Jekyll won't copy `_mockups/`
into `_site`, so it won't be there.

## Files

### `hub.html`

The comp homepage. One responsive file: mobile as the base, a single media
query at 700px for the two-column layout. Verified with no horizontal overflow
at 320, 390, 768, and 1440px.

**Fonts are the repo's own** — `Crimson` (Caslon-ish serif) for masthead and
headlines, `League Gothic` (condensed) for every label and folio line,
`Vollkorn` for body. No webfont service, no new dependency. This is why the
unused faces in `fonts/` were kept rather than deleted.

**Colours are all measured against WCAG 2.2 AA** on the `#fbfaf6` paper:

| Token | Value | Contrast |
|---|---|---|
| Brand red | `#a82931` | 6.64:1 — AA |
| Body ink | `#15130f` | 17.76:1 — AAA |
| Grey meta | `#615c54` | 6.35:1 — AA |
| Row numbers | `#726c62` | 4.98:1 — AA |
| White on red | — | 6.94:1 — AA |

Do not lighten any grey without re-measuring. An earlier draft used `#c9c3b6`
for the row numbers, which is 1.68:1 and a clear failure.

## Known placeholders

- **Hours per week** shows as an em-dash for all ten boards. Those numbers do
  not exist yet; see `content-questions.md`.
- **The photograph** is `images/crimson.jpg`, the building exterior already in
  the repo. It stands in for a photo of people working, which is what the design
  actually wants.
- **Board copy** is the owner's own one-liners, verbatim. Do not rewrite them.
