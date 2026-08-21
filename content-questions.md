# Content questions — Fall 2026 comp

Temporary working file. Fill in the blanks; the answers get moved into
`_data/` during the redesign, and then this file gets deleted.

Excluded from the built site, so nothing here is published while you work on it.

Leave anything blank that you don't know or don't want on the site — blank
means "hide it," never "show an empty space."

---

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
