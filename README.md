# Module 2 SET Builder

A drag-and-drop sandbox for the SOS 110 Module 2 Review: map the **ecosystem
services of Grand Canyon National Park** and export the result as a PDF.

**Live:** https://ryanpcornell.github.io/sos110-module-2-set-builder/

This is the same tool that appears as slide 4 of the
[Module 2 Review deck](https://ryanpcornell.github.io/sos110-module-2-review/),
published on its own so students can bookmark just the tool.

## What it does, task by task
- **Task 1 — Native biodiversity.** Drag in plant communities and native animals
  from the palette, and record the `nps.gov` / `usgs.gov` pages you took them
  from in the band above the diagram. The checklist wants three or more of each.
- **Task 2 — Ecosystem services.** Four palette groups, one per category:
  Provisioning, Regulating, Supporting, Cultural. Each service you place needs a
  **➜ provides** arrow into a named sustainability outcome — that is the arrow
  the assignment asks for, and the checklist will not tick until every service
  has one.
- **Task 3 — Impact analysis.** Drop in a human pressure and draw a **− harms**
  arrow to the service it damages, then open **Task 3 write-up** for the four
  elements: the challenge, the link, the human factor and the solution. The
  "link" field is a dropdown of the services actually on your diagram.
- **Save as PDF** — opens the browser's own print dialog. The sheet carries your
  diagram, your sources, the assignment's own three-column services table, and
  the four elements composed into a single paragraph.

**Find your own examples.** The assignment says past teams used freshwater
springs and soil stabilisation, and that yours must be new — so every palette
group ends in a blank **Custom** piece, and double-clicking any piece renames it.

Two worked examples load from the toolbar. They are deliberately the two the
assignment names as already used: they show the shape of a complete answer
without being something you could hand in.

## Under the hood
One HTML file, no build step, no dependencies, no backend — nothing is uploaded
and nothing is stored. The only external requests are Google Fonts.

Built from `_deck-builder/module2_set_builder.py` (shared with slide 4 of the
deck, so the two cannot drift) via
`_deck-builder/module2_set_builder_standalone.py`:

    python3 module2_set_builder_standalone.py
