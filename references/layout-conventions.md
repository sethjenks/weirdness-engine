# Layout Convention Inventory

Use this inventory in **Layout mode**. Every direction cites exactly one ID. The violation is a replacement, not a removal. Everything else holds.

Read `references/editorial-grids.md` when the job is a spread, a grid, or magazine pacing. Read `references/letter-crop-scatter.md` when the ID is in the T-series or D8. Read `references/clever-moments.md` only after a direction is chosen and you are adding at most one surprise.

This file is a catalog of *what to break*. It is not a Paper tutorial.

---

## How to use

1. **Name the corpus.** Editorial feature openers, print spreads, and agent-default digital layouts. Be specific about which average you are departing from.
2. **Pick IDs, not vibes.** Scan the tables. Prefer conventions so taken-for-granted that nobody registered them as choices.
3. **One ID per direction.** Five directions, five IDs, five techniques. Do not stack E1 and G4 in the same direction.
4. **Hand off with the ID.** When a human picks a direction, the editorial / Paper executor builds with `violate: {ID}` and holds the rest of the inventory.
5. **Optional clever moment.** One per spread, from a *different lane* than the grid break. See `references/clever-moments.md`.

### Prompt stub

```
Run Weirdness Engine in Layout mode on {brief or screenshot}.
Corpus: editorial feature openers + agent-default layouts.
Use the layout convention inventory; cite convention IDs.
Produce 5 directions; each violates exactly one ID.
```

### Highest-leverage breaks

Prioritize these when the brief does not already point at a surface. They are the conventions agents and safe designers obey first.

| ID | Short name | Why it pays |
|----|------------|-------------|
| **D1** | Kill the cards | Cards are the default atom of digital and agent layout. Removing the chrome is usually the fastest path to a field. |
| **E1** | Unequal columns | Equal columns are the editorial average. Ratio is a decision; evenness is a habit. |
| **H1** | Size ≠ importance | Bigger-is-louder is the cheapest hierarchy. Inverting it restores seeing. |
| **E3** | Move the pull quote | The quote is treated as a caption for nearby copy. Relocating it makes it architecture. |
| **G4** | Named empty space | Leftover white space is how grids die. A named void is how they live. |
| **D8 / T-series** | Shader or crop in the letterform | Type-as-geometry. See the T-section below and `references/letter-crop-scatter.md`. |

---

## E — Editorial / print conventions

What a competent magazine spread obeys before anyone tries to be interesting.

| ID | Convention | Assumption | Sample violation | Technique fit |
|----|------------|------------|------------------|---------------|
| **E1** | Columns are equal in width | Even columns feel fair, balanced, and "designed." Ratio would look like a mistake. | Set a 5∶3∶2 or 2+1 field. Body in the wide measure; rail and caption in the narrow ones. | Constraint Inversion |
| **E2** | Body starts at the top of the text block | Empty space above type is waste. Fill from the head. | Sink the opening graph several modules. Start the text at the optical center or after a named void. | Alien Perspective |
| **E3** | The pull quote sits beside the paragraph it quotes | A quote is a restatement of nearby copy; adjacency keeps it honest. | Move the quote to a corner, the folio line, the gutter, or the following spread. Or set it as a structural beam. | Collision |
| **E4** | Images live in their own rectangular frames | Pictures and words occupy separate territories. Overlap is sloppy. | Run type through the picture, or let a letterform be the frame. | Collision |
| **E5** | Folios sit at the bottom outer corners | Readers find their place at a predictable edge. | Treat folios as a coordinate system — oversized, inside the grid, or as labels on cells. | Uncommon Care |
| **E6** | Headline, then dek / standfirst, then body | Hierarchy is a vertical stack. Identification precedes reading. | Crop the headline into a field. Put the dek in its own column. Start body somewhere else. | Constraint Inversion |
| **E7** | Body is justified or evenly left-aligned across columns | Even rag or justify = professionalism. Mixed alignment is unfinished. | Justify one column, rag another. Or hang an indent that becomes structure. | Constraint Inversion |
| **E8** | Captions sit under their images, small and quiet | Captions are metadata. They must not compete. | Make the caption a third column, the largest type on the spread, or the only text. | Alien Perspective |
| **E9** | Masthead / title lives at the top of the spread | You identify the publication first. | Put the masthead at the foot, as a stamp, or as a cropped fragment. | Outside Reference |
| **E10** | The opener splits image-half / type-half | Feature openers divide the spread into a picture and a text block. | Full-bleed type *is* the image. Or the picture is a thin strip and the field is type. | Exaggeration of Truth |
| **E11** | Running heads repeat the section name | Orientation requires a constant header. | Turn running heads into a score, a clock, a log line — or let grid labels do the job. | Uncommon Care |
| **E12** | White space is leftover after placing content | Empty areas are what you could not fill. | Design the void first. Content is what remains. (Pair the *idea* with G4; do not cite both in one direction.) | Constraint Inversion |

---

## D — Digital / agent defaults

What marketing sites and agent-built canvases reach for when nobody names a convention.

| ID | Convention | Assumption | Sample violation | Technique fit |
|----|------------|------------|------------------|---------------|
| **D1** | Everything lives in cards | Cards are the atomic unit. Chrome keeps things "clean." | Kill the cards. Type and image share one field. No radius, no shadow, no padded island. | Constraint Inversion |
| **D2** | Hero = headline + subhead + CTA + background | The first viewport must orient and convert. | Treat the first view as a spread, not a hero. No CTA — or the CTA is a folio. | Alien Perspective |
| **D3** | A 12-column grid with equal tracks and even gutters | Digital grids are even and invisible. | Number the tracks. Make them unequal. Let the grid be seen. | Exaggeration of Truth |
| **D4** | Nothing overflows its frame | Cropping is a bug. Safe-area thinking is professionalism. | Overflow on purpose. Clip a letter, a photo, a rule. | Constraint Inversion |
| **D5** | Images sit in rounded rectangles of one radius | Soft corners = friendly and modern. | Hard crops, irregular silhouettes, or type-shaped masks. | Collision |
| **D6** | Sticky top navigation | Users need persistent wayfinding on every scroll. | Nav as a running footer, a column, or absent on the opener. | Alien Perspective |
| **D7** | Features as three equal cards | Three is the sacred number of marketing. | One column of features as a contents page or an index. | Outside Reference |
| **D8** | Type lives fully inside its box | A letterform must be complete to be readable. | Shader, crop, or slice *in* the letterform. See T-series. | Uncommon Care |
| **D9** | Centered, stacked sections | Digital rhythm is one block after another. | Magazine pacing: opener / body / breather / closer as distinct spreads. | Outside Reference |
| **D10** | Agent default: Inter, 16px, 8px spacing, soft shadow, generous padding | "Clean" is the absence of decisions. | Specify a type system and a grid *before* any component exists. | Exaggeration of Truth |

---

## H — Hierarchy / reading order

What we assume about what gets seen first.

| ID | Convention | Assumption | Sample violation | Technique fit |
|----|------------|------------|------------------|---------------|
| **H1** | Bigger = more important | Size is the primary hierarchy signal. | A small title that is the real headline. A large caption that is not. | Constraint Inversion |
| **H2** | Reading order is top-left → bottom-right | The Western page path is the only path. | Enter through a crop, a folio, or a bottom-left caption. | Alien Perspective |
| **H3** | Color and weight carry hierarchy, not position | You paint importance onto type. | One weight throughout. Isolation and position do the work. | Constraint Inversion |
| **H4** | The first thing you see is the title | Identification precedes experience. | Enter through a fragment, a crop, or an empty cell. | Collision |
| **H5** | One focal point per viewport | Competing foci confuse. | Two equal foci that refuse to resolve — or a field of equal cells with no hero. | Exaggeration of Truth |

---

## G — Spatial / grid meta

Conventions about the grid itself, not the content on it.

| ID | Convention | Assumption | Sample violation | Technique fit |
|----|------------|------------|------------------|---------------|
| **G1** | The grid is invisible infrastructure | Showing the grid means the work is unfinished. | Draw the grid. Number the cells. Treat the system as content. | Exaggeration of Truth |
| **G2** | Content fills the grid | Empty modules are unfinished. | Leave modules empty on purpose. | Constraint Inversion |
| **G3** | Modules are equal | Equal units = fairness and system. | Hierarchical modules: some 3×2, some 1×1. | Constraint Inversion |
| **G4** | Empty space is leftover and unnamed | Space without a name is waste. | Name the void — "silence," a coordinate, a pause, a shift. The empty cell is a decision. | Uncommon Care |
| **G5** | The grid is orthogonal and axis-aligned | Grids are right angles. | Rotate, skew, or stagger the field. Half-cell offsets count. | Constraint Inversion |

---

## P — Paper-culture / canvas conventions

Defaults that show up when a canvas tool (Paper or otherwise) and an agent share a file. Violate the *habit*, not the tool. Do not turn the direction into a product demo.

| ID | Convention | Assumption | Sample violation | Technique fit |
|----|------------|------------|------------------|---------------|
| **P1** | The canvas is an infinite artboard of loose frames | Digital design is a pile of rectangles. | Treat the canvas as a printed spread with a format, a bleed, and a folio. | Outside Reference |
| **P2** | Hug-content / auto-layout is the default | Elements should size to what they contain. | Fix the field. Let type overflow it. | Constraint Inversion |
| **P3** | Design-system tokens *are* the aesthetic | Tokens = taste. | Tokens hold craft. Taste lives in one violation. | Alien Perspective |
| **P4** | Screens are stacked pages, not spreads | Digital = a scroll of pages. | Design facing pages. Sequence opener / body / breather / closer. | Outside Reference |
| **P5** | Components first, composition second | Build from cards and buttons up. | Compose the field first. Components are guests. | Exaggeration of Truth |

---

## T — Typographic crop and position

Type as geometry. These IDs are the execution surface for D8. When a direction cites a T-ID, load `references/letter-crop-scatter.md` before expanding.

| ID | Convention | Assumption | Sample violation | Technique fit |
|----|------------|------------|------------------|---------------|
| **T1** | Letterforms sit fully inside their box | A cropped letter is a mistake. | Per-letter `overflow: hidden` frames. Oversized glyphs, nudged until the crop is a slice, not an accident. | Constraint Inversion |
| **T2** | Type aligns to a column edge | Flush left or right is how type meets the grid. | Sit type on coordinates. Let letters straddle gutters. | Uncommon Care |
| **T3** | Wordmarks stay intact | A logo must be complete to be a logo. | Slice the wordmark across a visible, numbered grid. | Collision |
| **T4** | Type size is for reading, not geometry | Display type is just large text. | Letters define the spatial structure. The boundary between type and layout dissolves. | Constraint Inversion |
| **T5** | Letters do not overflow or scatter | Overflow is a bug; scatter is chaos. | Scatter letters with half-cell offsets. Empty cells get texture, not more type. | Uncommon Care |
| **T6** | Type does not carry coordinates or grid labels | Labels are for the designer, not the reader. | Publish the coordinates as part of the spread. | Exaggeration of Truth |

### Letter-crop recipe (summary)

Inspired by the Paper marketing treatment of a sliced "designer" wordmark on a visible grid with coordinates — a word broken into cells, each letter cropped, the system shown rather than hidden.

Do not execute this as a product recreation. Use it as a method:

1. Draw the grid. Show it. Number it if T6 or G1 is in play.
2. One frame per letter. Clip (`overflow: hidden`).
3. Set the glyph much larger than the frame. Nudge X/Y until the visible slice is intentional — a bowl, a stem, a join.
4. Scatter: offset some frames by half a cell. Do not randomize.
5. Empty cells get a mantra, a halftone, or nothing named (G4). They do not get more letters.

Full steps, anti-patterns, and the three-meter test: `references/letter-crop-scatter.md`.

---

## Citation in output

Layout-mode directions keep the standard six fields. The convention line **starts with the ID**:

```
**Convention being violated:** D1 — Everything lives in cards. Digital and agent layouts package every block as a padded, radiused island.
```

The executor prompt is then:

```
violate: D1
Hold every other inventory ID. One clever moment maximum, from a lane other than the grid break.
```
