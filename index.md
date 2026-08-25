---
layout: home
title: About Us

# The huge headline. Put the whole phrase in poster_line_1 and leave
# poster_line_2 blank: it sets on one line on a wide screen and the browser
# wraps it to two on a phone, breaking in the same place you would by hand.
poster_line_1: Comp the
poster_line_2: Crimson

# The line under the headline, split across two lines so the break point is
# yours rather than the browser's. Leave lede_line_2 blank to let it wrap on its
# own. Apostrophes are typographic (curly) rather than straight.
#
# No comma before "and", and no full stop at the end. The comma was the genuine
# error: two coordinated noun phrases do not take one, and there is no third item
# to make it a serial comma. The full stop went because this is a fragment used
# as a standfirst rather than a sentence -- display lines conventionally do
# without, and it reads cleaner over the photograph.
lede_line_1: The nation’s oldest continuously published daily college newspaper
lede_line_2: and Harvard College’s premier student organization

# Heading over the intro bullets. Leave "" and no heading renders.
intro_title: The comp

# The teaser line that sets up the bullets. Positioned "above", it is styled as
# a lead -- ink rather than grey, and the same size as the bullets -- because it
# is doing the framing rather than qualifying afterwards. Positioned "below" it
# reverts to the smaller grey qualifier.
#
# THIS IS YOUR DRAFT, placed verbatim. See the note at the bottom of this file
# for the specific things you said still need editing.
#
# Positioned "above" again: this wording sets the bullets up rather than summing
# them up, so it belongs before them.
#
# No full stop, matching the hero line and every bullet. Worth knowing this one
# IS a real sentence -- subject and verb -- so the stop was not an error the way
# the hero's comma was; it comes off for consistency, because no display line on
# this page carries one now. Put one back and it needs putting back everywhere.
intro_note: From journalism to business or tech — regardless of your passion, The Crimson has a comp for you
intro_note_position: above

# Its own line under the bullets, not a bullet itself -- it points somewhere
# rather than stating a fact, so it does not belong in a list of facts. Spaced to
# match the gap between bullets. Leave "" and it does not render.
# The target is the boards heading, id="boards".
intro_link_text: Learn more about our 10 comps

# The bullets below the --- are YOUR DRAFT, placed verbatim -- not tidied, not
# rewritten. You said it still needs an editing pass, so here is what I noticed
# while placing it, for you to fix or wave off:
#
#   1. No bullet has a closing full stop. Consistent, so fine.
#   2. The separator AND the space around it are not typed here. Both come from
#      CSS -- .intro-text strong::after -- so changing either is one line there,
#      applied to every bullet at once. That is also why there is deliberately
#      NO space between ** and the text that follows it on these lines: the CSS
#      margin supplies the gap on both sides equally. Typing a space here as
#      well would add it to only the right side, since the left side already
#      gets its gap from the pseudo-element's own margin -- which is exactly the
#      bug that shipped and was caught by measuring, not by looking.
#   2. There is a NON-BREAKING SPACE between "The" and "Crimson" in the teaser
#      above -- it looks like an ordinary space but the two words can never be
#      split across a line break. That, not the font size, is what stops "The"
#      being orphaned at the end of a line. If you retype that phrase you will
#      lose it; copy the line rather than retyping it.
#
# Lead phrases are both sentence case now, so the source agrees with itself. It
# makes no visible difference -- the run-in style uppercases them either way --
# but it means the next person editing this does not have two patterns to copy.
#   4. Still nowhere on the site: "Shape the journalism that shapes Harvard",
#      which you called the line you most wanted to highlight, and the
#      independence fact, which now survives only on the Business board's page.
#
# The **bold** at the start of a bullet is a run-in lead: it sets in the display
# face, uppercase, so it reads as a tag introducing the sentence. Wrap any
# opening phrase in ** and it behaves the same way.
#
# Apostrophes were curled to match the rest of the site. Nothing else changed.
# Keep the leading "- " on each line and it stays a bullet.
#
# The real copy that used to be here is parked in content-questions.md,
# section 1b, links intact, ready to paste back if you want any of it.
---

- **Real work from day one**Learn from current editors and see your work published before comp ends
- **No experience needed**Most Crimson editors had never worked for a newspaper before their comp
