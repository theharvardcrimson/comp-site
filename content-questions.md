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

## 1c. PARKED: the financial aid panel prose

Financial aid moved up into the two-column highlights block as bullets, so the
standalone panel that used to sit below the boards is gone -- `_sections/`
is now empty and that slot becomes the comp FAQ.

The full paragraphs are below. They are longer and warmer than the bullets and
say things the bullets do not, so keep them somewhere: they would work as an
FAQ answer, or on a page of their own. Restoring the panel is one file --
recreate `_sections/financial-aid.md` with this body and it reappears.

```markdown
Worried that you won't be able to spend time on The Crimson because you think
you'll need a paying job? We can help. The Crimson's Financial Aid Program offers
limited but substantial compensation to staff members with demonstrated financial
need. It's meant to ensure that students who would otherwise need a term-time job
can be Crimson editors, and it's part of our efforts to make sure that all Harvard
students have the opportunity to enjoy and learn from the experience of working
here, regardless of their socioeconomic background.

Any questions? Want more information? Don't hesitate to contact Crimson President
{{ site.data.semester.contact_name }} ([{{ site.data.semester.contact_email }}](mailto:{{ site.data.semester.contact_email }}))
with any and all questions about the program.
```

## 1e. WAITING ON YOU: the interest form link

You said you would send an updated one. The buttons read **Interest form** in
the hero, the drawer, the footer and the foot of all ten board pages, from
`signup_label` in `_data/semester.yml`; the sticky top bar reads **Sign up**,
from `header_signup_label` in the same file, because the bar is the one place
where the longer wording crowded the corner.

`signup_url` in that same file is still the OLD Google Form:

```
https://docs.google.com/forms/d/e/1FAIpQLScnz4wmdtXud61rA9Zlm6n5JMqopGssM4RDw2PDQoXOsNWyXg/viewform
```

So every button on the site currently says "Interest form" and points at last
cycle's form. That is the single most important thing to fix before launch --
a working button to the wrong form is worse than a broken one, because nobody
notices. Paste the new URL over that line and every button follows.

## 1j. YOUR DRAFT COPY IS IN, and here is what I did not touch

The teaser and three bullets you sent are in `index.md`, verbatim. You said it
still needs an editing pass, so I placed it and changed nothing except curling
the apostrophes. What I noticed while placing it:

1. Bullet 2 reads "completion base/just show up nd do the work" -- "base" for
   "based", "nd" for "and".
2. Bullets 1 and 3 have no closing full stop; bullet 2 does.
3. The slashes in bullets 1 and 2 read as unfinished alternatives rather than a
   deliberate either/or.
4. Bullet 3, "Shape the journalism that shapes Harvard", is a fragment beside two
   full sentences -- and it is the line you said you most want to highlight. It
   may want to BE the teaser rather than the last bullet.

The same list is in the front matter of `index.md` so it is next to the words.

**Teaser shortened at your instruction**, to: "Regardless of your passion — from
journalism, to business, to tech — The Crimson has something for you."

Shortening it dropped the phrase "Harvard's financially and editorially
independent student newspaper", which took a fact off the page rather than just
words. **That is now resolved:** independence came back as the third bullet, as
its own point with a run-in lead, which gives it more weight than it had buried
in an appositive. The teaser stays short.

Still open, from the same reshuffle: "Shape the journalism that shapes Harvard"
was bullet 3 and is now nowhere on the site. You said it was the line you most
wanted to highlight.

## 1k. The fourth stat, and what it cost

`$1M BUSINESS` is in. The wording is a guess from "our 1 million dollar
business" and is yours to set -- `_data/semester.yml` says how to make it read
"MILLION-DOLLAR BUSINESS" instead if you prefer, and what that trades away.

**It broke the stat-over-photograph alignment, deliberately.** Three stats sat
centred over three photographs by sharing a three-column grid with the band --
something you asked for and I measured to 0.0px. Four columns cannot centre over
three, so rather than half-keep it I let it go. The stats grid is now `auto-fit`,
so adding or removing a stat needs no CSS change at all.

Two ways to get the alignment back, if you want it:

- **A fourth photograph.** `printing_presses.jpg` is already in the gallery and
  pairs naturally with a business stat. Needs a credit like the other three.
- **Go back to three stats** and put the business figure somewhere else -- it is
  also already in the Business board's one-liner.

Not doing either without your say. Four stats over three photos does not look
broken; it just no longer looks deliberate.

## 1l. TO DECIDE: the video player and the collapse problem

Autoplay is removed, which fixes the video starting on its own. Opening the
disclosure now shows a paused player and you press play yourself -- one extra
click, and nothing ever starts unprompted.

**What is NOT fixed, and cannot be without JavaScript.** Collapsing the
disclosure hides the player but does not stop it. Verified: after closing, the
iframe is still in the document with its src intact and only `display:none`
applied. A video someone had started would keep playing, unseen. Chrome does not
reliably pause media in a hidden frame.

Why autoplay made this worse, for the record: the parameter lives in the URL
permanently, so it fired whenever the frame loaded rather than when you clicked.
Combined with the collapse behaviour, that gave sound with no visible player --
which is also a WCAG 1.4.2 failure, since audio playing automatically for over
three seconds needs a stop mechanism.

Three ways forward. Your call:

1. **Leave it.** Nothing autoplays now, so this only bites someone who presses
   play and then collapses the panel. The stop mechanism technically exists --
   reopen and pause -- but it is not obvious.
2. **Remove the ability to collapse.** Once opened, the player stays for the rest
   of the page view, so audio always has a visible player and controls. Costs the
   disclosure pattern some correctness -- a <details> that will not close is
   strange for keyboard and screen reader users.
3. **Go back to linking out.** The thumbnail opens YouTube in a new tab. No
   embedded player, so no hidden playback, and no third-party contact at all
   until the click. Costs playback in place, which is what you asked for.

Recommend 1 for now and revisit if it actually bothers anyone: it is a narrow
case, and 2 and 3 both give up something real.

Worth also recording that the no-third-party-until-click property does hold.
Tested across three fresh browser instances: zero requests to
youtube-nocookie.com both before and after scrolling the video into view, and one
after the click. Earlier readings that said otherwise came from a degraded
browser instance that had stopped honouring loading="lazy" -- the same fault that
twice made page images report as never loading.

## 1d. ROADMAP: things the owner has asked for, not yet built

Recorded as they were said, with the one thing each would cost. None of this is
started.

**Events as a calendar, not a list.** Each event should look like a day or entry
on a calendar rather than a row. One more event to add alongside the three.
Also wants the venue -- 14 Plympton Street -- shown and easy to find, possibly
with a small map.

*The map is the only part with a real cost.* A Google Maps embed is an iframe
that loads their JavaScript and sets cookies -- the same problem the comp video
had, and worse, because a map has no natural "click to load" moment. Options,
cheapest first: a static image of the block with a link out to directions;
an OpenStreetMap static tile, same idea but no Google; or an embed, which
breaks the no-third-party position the rest of the page now holds. Recommend
the first.

**Cut the "Before you choose" note** above the board list, replacing it with a
simple line inviting people to learn more about the ten boards. Worth knowing
what gets lost: that note carries the only mention anywhere on the site that
News, Magazine, Sports and Arts comp together for three weeks before splitting,
which is the most reassuring fact available to someone who cannot choose. If it
comes out of there it should land somewhere -- most likely the FAQ.

**Boards as accordions instead of pages.** Keep the ten rows as they are, and
expand each in place with a plus/minus rather than navigating to a page.

*This one is a genuine architecture decision, not styling.* Native <details>
does it with no JavaScript, so the mechanism is easy. The cost is the ten URLs:
/arts/, /news/ and the rest are what boards link to from their own pages and
emails, what search engines have indexed, and what someone pastes into a group
chat. Collapsing them into anchors on one page breaks every one of those links
unless the pages are kept as well and the homepage merely duplicates them.
Worth deciding deliberately, and worth checking with the boards first.

*What goes inside each dropdown*, as specified:

1. **Selected work** -- photos from thecrimson.com linking back to the pieces.
2. **A short description** of the board, cut down from what exists.
3. **Comp requirements and details.**
4. **The comp directors' names and contact details.**
5. **Date, time and location of the first meeting.**

Business will be laid out differently; to be discussed when we get there.

*What already exists versus what has to be gathered,* because the split matters
for how long this takes:

- Already in the repo: requirements (the `requirements` field on each board),
  directors and their emails (`_data/directors.yml`), and a one-line hook per
  board. Item 3 and item 4 are essentially done.
- Needs cutting down, not gathering: item 2. Each board file already carries
  its full prose; a short version is an edit, and it is the boards' own words
  so it is theirs to shorten.
- Needs gathering from scratch: item 1 and item 5. Selected work means, per
  board, a headline, a URL and an image -- with a photographer credit for each
  image, same rule as everywhere else on this site. Ten boards times three or
  four pieces is thirty to forty items, and that is the long pole. First-meeting
  details are ten short entries but depend on the Fall calendar existing, which
  is still open in section 2 below.

*One design note to settle early:* thumbnails that link out to thecrimson.com
mean either hosting copies of those images here, which is the pattern used for
the video thumbnail and keeps the page free of third-party requests, or hotlinking
them, which is lighter to maintain but reaches another server on every page view
and breaks silently when an image is moved. Recommend hosting copies.

**FAQ replaces the financial aid panel.** Done, in the sense that the panel is
gone -- financial aid is now bullets in the two-column block, its prose is
parked in section 1c above, and `_sections/` is empty. The FAQ block already
exists and renders as soon as `_data/faq.yml` has answers, so writing them is
all that is left.

**Drawer should jump to sections, and list more than boards.** Anchor links to
points on the page, plus entries for the FAQ and the About Us material.

*Small note for whoever builds it:* the drawer is a native <details>, and it
will not close itself when an anchor is followed, because closing needs
JavaScript. The panel would sit open over the section just jumped to. Worth
solving before shipping -- probably by having anchors only on a page where the
drawer is not the primary navigation, or by accepting it.

## 1h. Video aligned to the box beneath it — SETTLED

Both sections now read one shared pair of tokens, `--pair-cols` and
`--pair-gap`, so the video's edges and the financial aid box's edges coincide.
Verified to 0.0px at 1440, 1300, 1200, 1100, 1000 and 900.

They had drifted because each section defined its own grid: the intro was
1.1fr/1fr with a 51.8px gap, the highlights 1fr/1fr with 57.6px, which put the
video's left edge 27px inside the box below it. Overriding either token locally
is now the only way to break it again.

Side effect, and it is the good direction: the video went from 600px to 627px at
1440, since equal halves give it more than 1fr of a 1.1:1 split did.

**One thing to keep an eye on.** The text column is narrower now, and the
measure runs 52 characters a line at 1440 down to 42 from 1200 downward. For
continuous prose 42 would be too tight — the comfortable band is 45 to 75. It is
acceptable here only because that column is BULLETS, which are short and
self-contained and tolerate a narrow measure in a way a paragraph does not. If
that column ever goes back to running prose, revisit the ratio: an earlier note
warned against pushing past 1:1 for exactly this reason, and 1:1 is where it now
sits.

## 1i. TO RESOLVE: the board rows -- white space, and active voice

**Less white space — DONE, partly.** The cause was the grid, not the padding, as
suspected. Measured at 1440: the name column was 697px while the widest board
name, Multimedia, is only 445px of actual ink, so the description sat 309px clear
of the longest name and much further from short ones like Tech (178px).

Now `0.72fr 1fr` with a tighter gap, and the row padding down from 34px to 26px.
Dead space at 1440 goes from 309px to 126px. No name overflows its column at any
width; the widest keeps 89px of headroom at 1440 and 44px at 900.

The board name ink widths at 1440, for anyone re-tuning this: Arts 184, Blog 181,
Business 349, Design 259, Editorial 363, Magazine 368, Multimedia 445, News 205,
Sports 273, Tech 178. Multimedia is the constraint. If a board is ever renamed to
something longer, re-measure before narrowing further.

Still available if you want it tighter: the description column is capped at 46ch
and does not use its full width, so the ratio could go further. I stopped at
0.72fr because 900px is where the headroom gets thin.

**Active voice, and this one has a consequence.** You want "write about..."
rather than "writes about...", so it reads as what a comper would be doing.

The edit itself is mechanical -- every one of the ten is a third-person verb
that loses its "s", with Multimedia's "captures & produces" becoming "capture &
produce". I have NOT made the change, because these are the board one-liners
you approved verbatim and it is your call, but it is a find-and-replace rather
than a rewrite if you want it.

*The consequence:* the design currently uses the board name as the sentence's
subject -- the row reads "ARTS writes about the cultural phenomena...". In the
active voice that becomes "ARTS write about...", which is not a sentence. The
run-in construction stops working, so the change means one of:

- Accept the description as a separate phrase rather than a continuation of the
  name. Cleanest, and probably what you already picture.
- Add an implied lead-in, e.g. a small "you'll" or "here you" before each
  description. Costs a word on every row.
- Recast the descriptions as noun phrases instead of verbs.

Flagging it because the sentence-continuation idea is deliberate in the current
markup and comments, and whoever makes the verb change should know they are
retiring it rather than tripping over it.

## 1f. TO RESOLVE: the mobile header looks clumsy

Your words: "kind of dumb and not very sleek." Agreed, and note that renaming
the button made it worse -- "Interest form" is nearly twice the width of "Sign
up", so the crimson slab grew and now dominates a 390px bar next to a bare
hamburger. Two controls, one a heavy filled block and one three thin lines,
with nothing relating them.

Options, cheapest first, all pure CSS:

1. **Quiet both controls.** Drop the button's fill on small screens for the
   ghost outline already used in the hero, cut its padding, and give the
   toggle a small "Menu" text label so the two read as a matched pair of text
   controls rather than icon-plus-slab.

2. **Move the call to action out of the header on phones** into a slim sticky
   bar along the bottom. Thumb-reachable, which the top-right corner is not,
   frees the header to be just wordmark and menu, and the crimson stays a
   full-width band rather than an awkward rectangle. This is the one I would
   pick.

3. **Shorten the label on small screens only** -- "Interest" or "Form". Cheap,
   but it makes the most important control on the site vaguer, so I would not.

4. **Shrink the bar.** 70px is tall for a phone; 56 with smaller controls would
   look tauter on its own.

Recommend 2, with 1 as the fallback if a bottom bar feels like too much.

## 1g. Colour blocks — SETTLED

Four variants were mocked with the real copy and type, every colour pair
measured, and the owner picked **D, the pale wash**: `--wash: #f4e7e5`, ink body
text, crimson headings and markers, grey note. Boxes sit apart, separated by the
section's own gap.

Measured on that tint: body ink 15.38:1, crimson heading 5.75:1, grey note
5.50:1. All AA.

Rejected, with reasons kept so it does not get relitigated:

- *Crimson fill* (6.64:1) — correct and on-brand, but the page already carries a
  full-bleed crimson hero, three crimson stat blocks, a crimson play button and
  a near-black marquee band. Two more saturated slabs competed with all of it.
- *Ink fill* (17.76:1) — punched two dark holes into a light page directly after
  the dark marquee band.
- *One of each* — implied a distinction between alumni and financial aid that
  does not exist.

One thing the measuring caught that looking did not: **crimson markers on ink
are 2.67:1 and fail.** Irrelevant now that D won, but it is the kind of thing to
check rather than eyeball if the fill ever changes.

Two problems solved along the way, both worth knowing if these boxes are edited:

- The height mismatch resolved itself. Grid stretches both boxes to the same
  height, and pushing the contact note to the floor of its box means the spare
  space in the shorter one collects above the note rather than showing as a hole.
- `margin-top:auto` alone was not enough. In the taller box the content fills the
  height, so auto resolved to zero and the note butted against the last bullet.
  It needs a `padding-top` as a minimum separation. Now 28px at 1440.

Body text matches the intro's bullets exactly — clamp(17px,1.9vw,23px) at every
width — so the two bulleted sections read as one voice. Keep them in step.

**Still open:** the two column headings are 42px against the intro's 78px. That
was deliberate, to keep a hierarchy of section title over column label, but the
instruction was to match the text size and it is not certain that meant the body
only. Ask before changing.

## 1m. Bullet separator — SETTLED

The owner picked E, a small crimson middot, from six mocked options. It answers
the crimson bullet a few characters to its left, so the two read as a pair. The
other five are recorded in css/main.css next to the rule, with why each lost --
colon (correct but ordinary), em dash (competes with the teaser's own em dash),
en dash, pipe (reads as a table), and nothing at all.

Lives entirely in CSS (.intro-text strong::after), not in the copy, so this is a
one-line change if it is ever revisited.

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
