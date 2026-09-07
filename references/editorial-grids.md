# Editorial Grids

Grid literacy for Layout mode. Load this when the job is a spread, a magazine opener, a Paper canvas treated as print, or any brief that says "editorial."

The grid is not the weirdness. The grid is the structure you hold so one convention can break. A layout that invents a new grid on every spread reads as noise. A layout that holds a grid and violates one inventory ID reads as craft.

Companion files: `references/layout-conventions.md` (what to violate), `references/letter-crop-scatter.md` (type-as-geometry on the grid), `references/clever-moments.md` (one surprise after the grid is held).

---

## Anatomy

Name these before you place anything. If you cannot point to each one, you do not have a grid yet — you have a pile of frames.

**Format.** The page, spread, or artboard. A3, tabloid, 1440×900, a Paper page at a stated size. Format is a decision. "Whatever the canvas is" is not a format.

**Margins.** The field between the trim and the text area. Head, foot, fore-edge, spine. Margins are not leftover padding. They are the first proportion.

**Columns.** Vertical tracks inside the text area. Column width is a function of type size, not of "how many we usually use."

**Gutters.** The gaps between columns. One gutter value, used everywhere, unless a violation ID says otherwise (E1, G5).

**Modules.** The cells made when columns are crossed by horizontal divisions. The smallest picture is one module. Larger pictures are spans.

**Flow lines.** The horizontal rules that create those modules — and that give headlines, images, and sinks a place to sit. Without flow lines you have a column grid, not a modular one.

**Baseline.** The invisible horizontal rhythm type sits on. Body, captions, and folios share it. Display type may break it; body does not.

**Markers.** Crop marks, registers, folios, grid labels, coordinates. Usually hidden (G1). Showing them is a violation, not a default.

---

## Types of grid

**Manuscript.** One column, wide margins. Books, long essays, letters. Freedom is in the measure and the sink, not in spanning.

**Column.** Two to six vertical tracks, few or no flow lines. The classic magazine. Variety comes from spanning, not from redrawing.

**Modular.** Columns × flow lines = a field of cells. Newspapers, catalogs, Swiss posters. The most powerful editorial system — and the one agents underuse.

**Hierarchical.** Zones of different size from the start (a wide feature well, a narrow rail). Not the same as E1 (unequal columns inside one system) — this is a page made of unlike regions.

**Baseline.** A vertical rhythm in points or pixels that everything snaps to. Can sit under any of the above. Without it, mixed type sizes look like they were dropped.

Pick one primary type per project. You may add a baseline under a column or modular grid. You may not run two primary types on the same spread unless that *is* the violation (and then you cite it).

---

## Column cheat sheet

| Columns | Where it belongs | What body does |
|---------|------------------|----------------|
| 1 | Manuscript, essay, letter | The measure *is* the page. Watch line length. |
| 2 | Classic magazine, interview | Text + image, or two text fields. The default competent spread. |
| 3 | Feature flexibility | Body in two, rail in one — or body in one, images spanning two. |
| 4–6 | News, catalog, index | Narrow measures. Body rarely sits in a single 4–6 column; it spans. |
| 12 | Digital *mental* grid | Not twelve visible text columns. Body spans 4–6 of the 12. |

A 12-column digital grid that sets body in twelve skinny tracks is a failed translation of print. The 12 is for spanning. The reader should see two or three text columns.

---

## Measure

Comfortable body measure is **45–75 characters** (roughly 7–12 words). Below 45, the rag or justify chatters. Above 75, the eye loses the start of the next line.

Column width is a consequence of measure and type size, not the other way around. If the measure is wrong, change the span or the size — do not "live with it."

Display type has no measure in this sense. Display type has *geometry*. See the T-series and `references/letter-crop-scatter.md`.

---

## Spanning as craft

Once the grid is set, the work is spanning: an image across two columns, a standfirst across three, a sidebar in one. Variety comes from moves *within* a fixed structure.

Rules of thumb:

- Span odd or even, but be consistent about which edges you honor.
- A span that stops in a gutter is a mistake unless E1 or T2 is the cited violation.
- The smallest illustration is one module. Do not invent a size between modules.
- Empty modules are allowed. Unnamed leftover slivers are not. See G4.

---

## Drop cap

Default: a **three-line** drop cap, set after the body is placed, not before.

- Cut it into the opening graph so three lines of body run beside it.
- The cap sits on the same baseline grid as the body.
- Do not drop a cap into a headline or a dek.
- A two-line or five-line cap is a decision; call it. A random size is decoration.
- If the opener has no body — only display type — skip the drop cap. It has nothing to drop into.

The drop cap is craft, not weirdness. Do not spend the violation budget on it unless the brief is specifically about initials (then cite a T-ID or H-ID, not "make the cap weird").

---

## Pacing

A feature is a sequence, not a single hero. Name the four beats before you design any of them:

**Opener.** The first spread. Identification + one image or one typographic act. This is where a violation usually lives.

**Body.** The reading spreads. Grid held. Measure held. Spanning does the variety.

**Breather.** A spread that lets go — a full-bleed picture, a named void, a short lyric. Without a breather, a long feature feels like a feed.

**Closer.** The last spread. Credits, folio, a final image, an afterword. Not a stacked footer of links.

Digital translation: these are views or pages, not one scrolling column of identical sections (that is D9). You can scroll and still pace.

---

## Paper / CSS translation

The same anatomy, two executions. Keep the names so the handoff is not a new invention.

| Print name | Paper / canvas | CSS |
|------------|----------------|-----|
| Format | Page / artboard at a stated size | Viewport or a spread frame (`width` / `height` or `@page`) |
| Margins | Padding on the spread frame, not on every child | `padding` on the spread; not `margin` on cards |
| Columns | Column guides or a grid of frames | `grid-template-columns` |
| Gutters | Gap between frames | `gap` |
| Modules | Cells; images sized to N cells | `grid-template-areas` or line-based spans |
| Flow lines | Horizontal guides | `grid-template-rows` / named lines |
| Baseline | A repeating vertical guide | `line-height` locked to a step (e.g. 8 or 12px) |
| Markers | Coordinates, labels, crop ticks | Utility layers; hide unless G1 / T6 / E5 is the violation |

Do not rebuild the grid as a stack of cards (D1) and call it a translation.

---

## Skill defaults

Use these when the brief does not specify a system. They are defaults, not laws. Changing them without citing an ID is slop.

- **Mental grid:** 12 columns.
- **Visible body columns:** 2 or 3.
- **Margins:** at least 64px (or 12mm on print). More on an opener.
- **Gap / gutter:** 24–32px (or 4–6mm). One value.
- **Measure:** 45–75ch in every body column.
- **Baseline:** 8 or 12px step; body and caption share it.
- **Drop cap:** 3-line, after body exists.
- **Pacing:** opener / body / breather / closer, named in the coherence plan.

---

## Violation budget

This file holds the grid. `references/layout-conventions.md` spends the budget.

- **One convention ID per direction.** If you break E1, you do not also break G4 in that direction.
- **One clever moment per spread**, from a different lane than the grid break.
- **Hold the rest.** Equal gutters, readable measure, working folios, intact hierarchy — unless the cited ID is one of those.
- **Do not "break the grid" as a vibe.** "Break the grid" is not an ID. Cite E1, G3, G5, or T5.

---

## Checklist

Before you call a spread done:

- [ ] Format is named (size, not "the canvas").
- [ ] Margins, columns, gutters, modules, flow lines, baseline, and markers can each be pointed at.
- [ ] Grid type is named (manuscript / column / modular / hierarchical / baseline).
- [ ] Body measure is 45–75ch.
- [ ] Visible body columns are 2–3, even if the mental grid is 12.
- [ ] Spans land on module edges.
- [ ] Empty space is either a module or a named void — not a sliver.
- [ ] Drop cap, if present, is three lines and post-dates the body.
- [ ] The sequence has an opener, and a closer if the piece is longer than one spread.
- [ ] Exactly one inventory ID is violated. Everything else is held.
- [ ] At most one clever moment, and it is not doing the job of the violation.
