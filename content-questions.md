# Content questions — Fall 2026 comp

Temporary working file. Fill in the blanks; the answers get moved into
`_data/` during the redesign, and then this file gets deleted.

Excluded from the built site, so nothing here is published while you work on it.

Leave anything blank that you don't know or don't want on the site — blank
means "hide it," never "show an empty space."

---

## Supplied by Matteo, Aug 20 — with one blocker

He sent a full set of board one-liners and a shopping-week schedule. The
one-liners are **timeless and usable verbatim**. The dates are **Spring 2026 and
cannot ship** — the sessions below ran 2/1–2/6, six months ago. Fall equivalents
are needed for every one of the ten.

### The ten one-liners — usable as-is

Verbatim, his wording and punctuation. These become the `hook` field on each
board. Note the design intent: the board name stays as the opening word of the
sentence, set bold as a newspaper run-in head, so his text is preserved intact
rather than trimmed.

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

Two display names to carry through the site: Blog is **Flyby**, Magazine is
**FM**. Neither is currently shown as such in the nav.

### Shopping week — structure good, dates dead

Spring's schedule, kept only as a shape to fill in. **Every date, time, and room
below needs a Fall replacement.** Note that venues varied — three sessions were
off-site, so location is per-session, not a site-wide constant.

| Board | Spring slot (STALE) | Venue |
|---|---|---|
| Business | Sun 2/1, 2:00 pm | 14 Plympton St |
| News | Mon 2/2, 5:00 p.m. | Fong Auditorium, Boylston Hall |
| Magazine | Mon 2/2, 7:00 p.m. | Emerson Hall, Room 305 |
| Multimedia | Mon 2/2, 7:30 p.m. | Emerson Hall, Room 305 |
| Sports | Tue 2/3, 7:30 p.m. | 14 Plympton St |
| Tech | Wed 2/4, 7:00 pm | 14 Plympton St |
| Design | Wed 2/4, 7:30 pm | 14 Plympton St |
| Arts | Thu 2/5, 6:30 p.m. | 14 Plympton St |
| Editorial | Thu 2/5, 7:00 p.m. | 14 Plympton St |
| Blog | Fri 2/6, 5:00 p.m. | 14 Plympton St |

"Comp shopping week" is the right frame and it is currently absent from the
site. It also reconciles with the single "Comp Kickoff" event: Spring ran a
Saturday kickoff (1/31) and then per-board sessions the following week.

### Still missing after this batch

- **Hours per week, all ten boards.** The one-liners describe what each board
  does but not what it costs you. Still the highest-value gap.
- **Fall kickoff date**, plus the ten Fall session slots above.

### Decision needed: the phone number

His sign-off included a personal mobile:

> Questions? Contact Crimson President E. Matteo Diaz
> president@thecrimson.com | (415) 686-4169

**Not publishing that without explicit confirmation.** This repo and the site
are public and indexed, so a personal mobile on the page will be scraped. The
email is institutional and safe. Options: email only, publish the number
anyway, or route through a Google Voice number.

## 0. Board groupings and the shared reporting comp

The hub groups the ten boards by type rather than listing them A–Z. Working
structure, from Matteo:

| Group | Boards | Notes |
|---|---|---|
| Reporting | News, Magazine, Sports, Arts | **Shared comp: all four meet together for the first three weeks, then split off.** |
| Opinion / Blog | Editorial, Blog | Written but not reporting. Group name still undecided. |
| Visual + technical | Multimedia, Tech, Design | "Functional" boards — they make the paper rather than write it. |
| Business | Business | Its own category; revenue side, not editorial. |

**The shared three-week reporting comp is the most important undocumented fact
on the site.** It means someone interested in reporting does not have to choose
between four boards up front — which is exactly the fear that stops people from
starting. It currently appears on zero pages.

Questions on it:

- **How does it actually work?** Three weeks of shared sessions, then you pick a
  board? Or do you declare a board first and just train together?
- **Can you switch after the split?** If someone starts toward News and lands on
  Sports, is that fine?
- **Do the four boards' requirements overlap during those three weeks**, or does
  each still expect its own pieces from week one?
- **Same meeting time and place for all four?**
- **Do any of the other groups share a process** the way reporting does? Do
  Multimedia / Tech / Design overlap at all, or are they fully separate comps?

**Group names are yours to set.** "Reporting", "Visual + technical", and
"Business" are placeholders that read fine. The Editorial + Blog pair is the
awkward one — they are genuinely different from each other, and "Opinion / Blog"
is descriptive but limp. Options: name it plainly, or drop the group and let
those two stand alone between the others.

## 1. Per board

`hours_per_week` is the single highest-value missing fact on the whole site.
It's what every prospective comper actually wants to know, it appears nowhere
today, and it's the number that makes the ten-board comparison view work.
A range is fine ("4–6"). An honest-but-scary number beats no number, because
people fill silence with their worst guess.

| Board | Hours/week | Meeting day + time | Pieces or projects required |
|---|---|---|---|
| Arts | | Mondays, 6 p.m. (seminars) | 5 pieces |
| Blog | | | 6 posts |
| Business | | | |
| Design | | | |
| Editorial | | | 2 op-eds + 1 staff-ed |
| Magazine | | Mondays (writers' mtg) | 4 articles |
| Multimedia | | | |
| News | | | up to 6 articles |
| Sports | | Mondays, 8 p.m. (board mtg) | |
| Tech | | | |

Pre-filled cells are what I could read off the current pages — correct them if
they're wrong or stale. Empty cells aren't stated anywhere on the site today.

## 2. Comp logistics

These apply site-wide and currently appear nowhere.

- **Fall kickoff date:**
- **Kickoff time:** (currently reads "4–6 p.m." — still right?)
- **Kickoff location:** (currently "14 Plympton St")
- **Comp start date:**
- **Comp end date:**

The About Us page currently says "Date and time TBA" because the old line said
`Saturday, Jan. 31, 2026` — the Spring date. I removed it rather than let a
false date ship, so this one is worth filling first.

## 3. The anxiety questions

These are the things a nervous first-year wants to know and cannot find
anywhere on the site. My read is that the silence is doing real damage — an
unanswered "will I get in?" gets answered pessimistically by default.

- **Is comp competitive? Is finishing enough to be elected?**

- **Can you comp two boards at once?** (Arts hints at reduced requirements for
  multi-board compers; no other page mentions it.)

- **What if you start late, or miss meetings?** (Arts says the work still
  counts. Is that true board-wide, or Arts-specific?)

- **What happens after comp?** What being an editor actually means — time,
  commitment, what you get.

- **No experience required** — true for all ten boards, or are there
  exceptions? Several pages say it; worth stating once, authoritatively.

## 4. Corrections needed

**Business, second director.** `_config.yml` has a mismatch — which is right?
```
name:  Arman Lateef
email: hamza.lateef@thecrimson.com
```

**Editorial, second director.** `Salma O. Siddiqui ` has a trailing space in
`_config.yml`. Harmless today, but it would break an exact-match lookup later.
I'll strip it unless it's meaningful.

**`tech` vs `technology`.** The file is `tech.html`, the nav says "Tech", the
config key is `technology`. Standardizing on `tech` unless you object.

## 5. Needs your rewrite (I won't touch prose)

**`blog.html`** names last semester's directors in the body copy:

> "We (Wyatt + Ava) are super stoked to be working with our compers..."

`_config.yml` now lists Cristian D. Dominguez and Grace E. St Laurent. The
sentence is first-person and warm, so swapping two names mechanically would
put words in the new directors' mouths. Your call, or theirs.

While you're in there — is anything else on the ten board pages out of date?
Named people, specific events, "this year we're doing X" claims. That kind of
staleness is invisible to me; I can't tell a current fact from a 2024 one.

## 6. Photography

The redesign leans on real Crimson photography, which means we need a set to
work from. Multimedia publishes 1,000+ photos a year and the site currently
uses exactly one image: a static shot of the building.

- Can you get ~10–15 images cleared for site use from Multimedia?
- Ideally: the newsroom at work, a few boards mid-activity, the building, and
  two or three dramatic news/sports/arts shots.
- Any credit or usage line they need alongside them?

Worth flagging early: this is the one dependency in the redesign that runs
through another board's time, during their busiest week.
