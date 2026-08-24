# Content questions — Fall 2026 comp

Temporary working file. Fill in the blanks; the answers get moved into
`_data/` during the redesign, and then this file gets deleted.

Excluded from the built site, so nothing here is published while you work on it.

Leave anything blank that you don't know or don't want on the site — blank
means "hide it," never "show an empty space."

---

## Settled

- **Flat list of ten boards.** No grouping by category.
- **No hours-per-week figure.** Dropped at the owner's request; the field is
  removed from all ten board files and from the templates.
- **No shopping week for Fall.** Per-board info sessions are not happening, so
  no session dates, times, or venues anywhere on the site.
- **Board one-liners supplied and approved** (below). Nothing else from that
  batch is being used — not the intro paragraph, not the financial-aid line,
  not the sign-off.
- **Personal mobile number will not be published.** Resolved; `president@thecrimson.com`
  is the contact.
- **Board pages are showpiece-led**, one pattern reused ten times, with a
  text-only fallback so a board with no photograph still looks deliberate.
- **Brand red is `#a82931`** — 6.94:1 on white, AA for text, AAA at display
  sizes. Secondary grey must be `#6b6b6b` or darker.
- **Photos arriving later.** Photo is an optional field from the start, so
  adding them is a one-line change per board, not a rebuild.

## The ten board descriptions — approved, verbatim

His wording and punctuation, unaltered. These are the `hook` field on each
board. The board name stays as the sentence's opening word, set as a newspaper
run-in head, so the sentence is preserved intact rather than trimmed to avoid
repeating the heading.

- **ARTS** writes about the cultural phenomena taking over Harvard, Cambridge, & the world
- **BLOG (FLYBY)** provides witty & hilarious commentary on all things student life
- **BUSINESS** runs the million-dollar business that supports our independent journalism
- **DESIGN** crafts the stunning graphics & print products that showcase our stories
- **EDITORIAL** shapes campus & national discourse with leading opinion coverage on Harvard
- **MAGAZINE (FM)** leads our longform coverage with incisive style & impactful investigations
- **MULTIMEDIA** captures & produces all of The Crimson's photo, video, & podcast content
- **NEWS** breaks high-impact stories, holding power to account & informing millions of readers
- **SPORTS** covers the nation's leading athletic program in varsity teams & Olympic gold medals
- **TECH** builds the website that powers one of the nation's most tech-savvy college newsrooms

Two display names carried through the site: Blog shows as **Flyby**, Magazine
as **FM**.

---

## 1. The third stat — SETTLED

`15M+ VIEWS IN THE LAST YEAR`, from the owner's "15+ million views in the last
year". Note this changed the metric from *readers* to *views*.

Written as 15 / M+ so it renders "15M+", the conventional order. "15+M" is a
one-character change in `_data/semester.yml` if the literal phrasing is wanted.

No TK remains anywhere on the site.

## 1b. PARKED: the old homepage prose

The homepage body is a single lorem ipsum paragraph at your request, until you
know what you want it to say. Nothing here is published -- this file is
excluded from the build -- so this is a safe place to keep the old copy while
you decide. Paste any of it back into `index.md` below the front matter, or
write over the placeholder entirely.

It is also in git, at commit 825ea11 and earlier, if this section ever gets
tidied away.

The markdown link syntax is intact, so pasting a paragraph back gives you the
working links again.

```markdown
Welcome to the {{ site.data.semester.season }} {{ site.data.semester.year }} comp
for The Harvard Crimson! Regardless of your passion, we have ten different boards
and 153 years of experience waiting for you at 14 Plympton St. The Crimson is not
only the nation's oldest continuously published daily newspaper, but it is also
the premier student organization at Harvard College, offering opportunities in
everything from journalism to business to photography.

As Harvard's financially and editorially independent student newspaper, The
Crimson's reporting has had a profound impact on campus life. Our award-winning
reporting has [exposed racism and sexism within the Harvard University Police Department](https://www.thecrimson.com/article/2020/1/31/hupd-investigation/);
brought to light allegations of misconduct [against powerful faculty members](https://www.thecrimson.com/article/2020/5/29/harvard-anthropology-gender-issues/);
and provided minute-by-minute [coverage of campus crises](https://www.thecrimson.com/article/2024/1/3/claudine-gay-resign-harvard/).

Comping The Crimson will give you the opportunity to shape the journalism that
shapes Harvard.

The Crimson is also a training ground for the next generation of journalists,
public servants, and business leaders.

Our prominent alumni include U.S. Presidents Franklin D. Roosevelt '1904 and John
F. Kennedy '40; 30 Pulitzer prize-winners including Nicholas D. Kristof '81, Linda
Greenhouse '68, David Sanger '82, and Susan C. Faludi '81; and titans of business,
media, and technology, such as Microsoft CEO Steve Ballmer '77, fmr. YouTube CEO
Susan D. Wojcicki '90, and Mad Money host Jim Cramer '77 just to name a few.

The Crimson has substantial reach as a newspaper and a company. Its million-dollar
business. Its website, which in 2023 received over 21 million page views. Its
Financial Aid Program, which has given out close to $1 million over the past decade
to hundreds of Crimson staffers. Its lasting friendships and vibrant community.

Come see for yourself! Stop by 14 Plympton Street for a tour of The Crimson's
historic building and to learn more about our 10 comps.
```

## 2. Needed: what the Fall comp actually looks like

Shopping week is gone, which removes the only per-board event structure the
site had. So:

- **Is there still a kickoff event?** `index.html` currently reads "Fall Comp
  Kickoff — Date and time TBA." If there's no kickoff either, that whole block
  should come out rather than sit there empty.
- **How does someone start?** Just the Google Form, or is there a first
  meeting?
- **Comp start and end dates.**
- **Is there any date at all** that belongs on the site for Fall? If the answer
  is genuinely "sign up and we'll email you," that's fine — but the site should
  say so plainly instead of implying a calendar that doesn't exist.

## 3. Open: where the shared reporting comp fact goes

News, Magazine, Sports, and Arts comp together for the first three weeks before
splitting off. This is the most useful undocumented fact on the site — it means
nobody has to pick correctly and cold among four boards.

Grouping is out, so it no longer has a natural home. Options:

- One line above the board list, unattached to any group.
- A small marker on those four rows only.
- In the FAQ.

Still worth surfacing prominently somewhere. Also unresolved: can you switch
boards after the split, and do the four boards' requirements overlap during
those three weeks?

## 4. The anxiety questions

Absent from all eleven current pages. A nervous first-year wants these and an
unanswered "will I get in?" gets answered pessimistically by default.

- **Is comp competitive? Is finishing enough to be elected?**
- **Can you comp two boards at once?** (Arts hints at reduced requirements for
  multi-board compers; no other page mentions it.)
- **What if you start late or miss meetings?** (Arts says the work still counts.
  True board-wide, or Arts-specific?)
- **What happens after comp?** What being an editor actually means.
- **No experience required** — true for all ten, or are there exceptions?
  Several pages say it; worth stating once, authoritatively.

## 5. Corrections needed

**Business, second director.** Still a mismatch in `_data/directors.yml` — which
is right?
```
name:  Arman Lateef
email: hamza.lateef@thecrimson.com
```
This is the only outstanding item in this section. The trailing space in
"Salma O. Siddiqui" is fixed, and `technology` is now `tech` everywhere.

## 6. Needs your rewrite (I won't touch prose)

**`_boards/blog.md`** names last semester's directors in the body copy:

> "We (Wyatt + Ava) are super stoked to be working with our compers..."

`_data/directors.yml` lists Cristian D. Dominguez and Grace E. St Laurent. The
sentence is first-person and warm, so swapping names mechanically would put
words in the new directors' mouths. Your call, or theirs.

While you're in there — anything else out of date across the ten board pages?
Named people, specific events, "this year we're doing X" claims. That staleness
is invisible to me; I can't tell a current fact from a 2024 one.

## 7. Typefaces — SETTLED

Four variants were rendered side by side at real size and the owner picked the
one already in place:

- **League Gothic** — display. Headlines, board names, labels, buttons.
- **Crimson** — the wordmark, and nothing else.
- **Vollkorn** — body copy and standfirsts.

Rejected, with reasons, so this doesn't get relitigated:

- *Crimson for body too* (one serif everywhere) — more unified and one fewer
  font file, but it's a lighter face that reads thin on the crimson field, and
  being narrower it pushed the hero standfirst from two lines to three.
- *Chunk Five instead of League Gothic* — at the same size the headline is far
  wider, so it would have to be set smaller. The scale is the point.
- *Colaborate Light for labels* — too small a change to justify a fourth family.

The two faces from the new thecrimson.com are still welcome if you want them
later; all three are behind CSS custom properties at the top of `css/main.css`,
so a swap is one line each. But nothing is waiting on them.

## 8a. Photography — three in, credits still needed

The homepage three-up band is filled from `images/gallery/front_page_gallery/`:

1. The Dec. 1966 press-room celebration (black and white)
2. The HUA livestream
3. Commencement issues in the newsroom

**Still needed: a photographer credit for each.** The design has a byline slot
that stays hidden until `credit` is filled in `_data/semester.yml`; fill it and
the caption appears by itself. Nothing on the page is broken without them, but
the photographers are currently uncredited.

**Also worth your eye: the alt text.** `label` on each of the three is the alt
text, written from looking at the photographs. The event names were inferred
from filenames, not known — particularly whether the livestream really is an
HUA event. Correct them in `_data/semester.yml`; they are one line each.

The lower marquee band is filled separately from
`images/gallery/crimson_front_pages/` — twenty Vol. CLIII front pages in date
order. Those are aria-hidden decoration, carry `alt=""` by design, and need no
credits. Three cosmetic oddities in that supplied run, none of which affect
anything: there is no no-15 or no-19, and two different issues are both
numbered no-16.

## 8b. Photography — the rest, later

Optional field, so this can land any time.

- ~18–20 images: ten board pages, one hub hero, plus spares.
- Originals, or at least 2000px on the long edge. Don't pre-compress.
- Name them by board (`news-01.jpg`).
- **Per photo: photographer credit** (the design has a red byline slot; a photo
  without a credit can't ship) **and a one-line caption** of what's happening —
  that becomes the visible caption and the basis for correct alt text.
- Prioritize people working over buildings. The current site's one photo is an
  empty building exterior and it's the least persuasive image available.
