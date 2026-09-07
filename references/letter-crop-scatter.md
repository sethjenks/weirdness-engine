# Letter-Crop Scatter

A type-as-geometry recipe for Layout mode. Load this when a direction cites **D8** or any **T-ID**, or when a clever moment is in the typographic lane and the violation is something else.

The method: letters are not text in a box. They are shapes in clipped frames, oversized and nudged so the visible part is a chosen slice, then placed on a grid that may leave cells empty.

Inspired by the Paper marketing treatment of a sliced "designer" wordmark — a word broken across a visible grid, each letter cropped, coordinates shown. Recreate the *method*, not the ad.

This is not a Paper MCP tutorial. Any canvas or CSS that can clip a frame and set type will do.

---

## When to use

**Use when:**

- The cited ID is D8, T1, T3, T4, or T5.
- The brand has a word worth looking at as geometry (a short title, a masthead, a one-word claim).
- The rest of the spread can stay quiet. Cropped type is loud.

**Do not use when:**

- The job is a long read and you have not placed the body yet. Geometry comes after measure, or not at all.
- You already spent the violation on another typographic or overflow ID (do not stack T1 with D4, D8, T3, T5).
- The word is long. More than ~8–10 letters and scatter becomes a ransom note.
- You need the word to identify at a glance *and* you are not willing to run a three-meter test (below).

If G1 or T6 is the cited ID, you may *show* the grid and coordinates. If it is not, hide the labels — the crop still works.

---

## Steps

### 1. Draw the grid

Name the format. Use the skill defaults unless the brief overrides: 12-column mental grid, 2–3 visible body columns elsewhere on the spread, margins ≥64px, gap 24–32px. See `references/editorial-grids.md`.

For the wordmark field itself, decide a coarser module — often 4×2, 5×2, or 6×3 cells. The word does not need one letter per column of the page grid. It needs a field.

Show the grid if G1 or T6 is in play. Otherwise keep it as construction.

### 2. One clipped frame per letter

Each letter gets its own frame. The frame is a module (or a span of modules). Clip it: `overflow: hidden` in CSS; "clip content" on a canvas.

Do not put the whole word in one frame and mask it. The crop is per letter so each slice can be nudged independently.

Frames sit on the grid. They may span two modules. They may not sit at arbitrary pixel offsets — yet. That is step 4.

### 3. Oversized glyphs, nudged for a slice

Set the letter much larger than its frame. Then nudge X and Y until the visible crop is a *slice you chose*:

- a bowl (the counter of **e**, **o**, **a**)
- a stem (**d**, **l**, **i**)
- a join (**n**, **m**, **r**)
- a terminal or ear (**r**, **g**, **a**)

The test: could you name the part of the letter you are showing? If you only know "it looks cropped," keep nudging.

Weight and optical size matter. A display cut with a thick stem survives crop better than a hairline.

### 4. Scatter with half-cell offsets

Once the slices are right, break the even marching line. Move some frames by **half a cell** — up, down, or sideways. Not a random jitter. Half-cell is still the grid (G5-adjacent, but do not cite G5 unless that is the ID; here it is execution).

Typical pattern: most letters on the row; one or two raised a half-module; one dropped. The word still has a reading line. The scatter is a limp, not a explosion.

### 5. Empty cells get a mantra, a halftone, or a name

The field will have cells with no letter. That is correct.

- A short mantra or log line, set small, one cell.
- A halftone, a dot grid, a rule.
- Nothing — but then *name* the void in the coherence plan (G4 thinking, without citing G4 unless it is the ID).

Do not fill empty cells with more letters, logos, or cards (D1). Empty is a material.

---

## Anti-patterns

- **Ransom note.** Every letter a different size, weight, or offset. Scatter is half-cell, not chaos.
- **Illegible on purpose.** Crop is not encryption. If the word cannot be recovered, you made texture, not type.
- **One frame for the whole word.** Then you have a mask, not a sliced wordmark.
- **Tiny type in a huge clip.** The slice should feel oversized — a fragment of something bigger than the cell.
- **Labels on by default.** Coordinates and cell numbers are a T6 / G1 / E5 decision. They are not decoration for every crop.
- **Cards around letters.** A radiused, padded island per glyph is D1 sneaking back.
- **Hug-content frames.** If the frame sizes to the letter, there is no crop (P2). Fix the frame, overflow the glyph.
- **Long words.** If you need the whole sentence, set the sentence. Crop a title, a masthead, a one-word claim.
- **Crop as the second violation.** If E1 or H1 is the cited ID, letter-crop may only appear as the *clever moment* (typographic lane), and only if you still have budget.

---

## The three-meter test

Readability is a craft hold, not a cowardice.

1. **Three meters (or a thumbnail).** Can you still tell there is a word, and roughly which word? If not, the slices are too abstract or the scatter is too wide. Pull letters back toward the reading line, or show more of each glyph.
2. **One meter (or the actual spread).** Can a patient reader assemble the word without a caption? If they need the caption to know what it says, add a small, complete setting of the same word elsewhere on the spread (a folio, a masthead line). That complete setting is craft, not an explainer.
3. **In the hand (or at 100%).** Does each cell still look like a chosen slice — bowl, stem, join — rather than a bad crop? If a cell looks accidental, nudge it.

Failing the three-meter test is allowed only if illegibility *is* the cited violation (rare; you would cite H4 or T4 and say so). Otherwise, fix the type.

---

## Hand-off

When the direction is T-series or D8:

```
violate: {T1|T3|T4|T5|D8}
Execute letter-crop scatter.
Per-letter clipped frames. Oversized glyphs, nudged to a named slice.
Half-cell scatter only. Empty cells: mantra / halftone / named void.
Pass the three-meter test. Hold every other inventory ID.
```

When letter-crop is the clever moment (other ID already chosen):

```
violate: {ID}
Clever moment, lane 2 only: letter-crop the {word}, not the layout.
One moment. No coordinates unless {ID} is T6/G1/E5.
```

Full inventory: `references/layout-conventions.md`. Grid holds: `references/editorial-grids.md`. Moment budget: `references/clever-moments.md`.
