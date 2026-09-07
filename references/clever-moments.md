# Clever Moments

A taxonomy of *one* surprise per spread. Load this after a Layout-mode direction is chosen — not while inventing the five directions.

The grid break is the violation (one inventory ID). A clever moment is optional garnish from a **different lane** than that break. If the direction already violates T1 (cropped letters), do not also add typographic cleverness. If it violates G4 (named empty space), do not also add a print-craft void gag.

Clever moments are not a seventh technique and not a second convention ID. They do not replace the Five Conditions.

---

## Operating rules

**One moment per spread.** Two moments compete. The reader does not know which one was the point. If you can see a second moment, delete it.

**Craft first.** The moment sits on a competent grid: measure holds, folios work, type is readable. A joke that needs the layout to fail is not clever.

**Reward, don't require.** The spread still works if the reader misses the moment. No tooltip, no "did you notice?" The people who catch it feel smart; the people who don't still get the story.

**Brand-rooted.** The moment could only belong to this title, this story, this metaphor. A generic wink (a hidden 404 game, a random Konami code) is Uncommon Care spent on the wrong object.

**Timing.** Place the moment where the beat can afford it. Openers can carry a typographic or conceptual moment. Body spreads can carry a craft surprise in a caption or folio. Breath-ers can carry an Easter egg. Do not hide the only joke on the opener in a way that delays identification (unless H4 is the cited violation — and then the moment is *not* also H4).

**Shareable > viral.** A moment worth photographing or quoting is enough. Optimizing for "this will go on TikTok" produces parlor tricks. If the share would need an explainer, it failed the fifth Condition.

---

## The five lanes

### 1. Conceptual / idea wit

The idea is the joke. The layout is straight.

The spread makes an argument you only get once you read the relation between elements — a contents page ordered by the hour the work starts; a profile whose "pull quote" is the subject's radio call sign; a feature about absence whose opener has no subject.

**Fits when:** the brand's weird territory is a *claim*, not a texture.
**Does not fit when:** you are already violating H4 or E10 (the entrance *is* the concept). Pick another lane.

### 2. Typographic cleverness

The letterforms do something the words also mean — or they do something the words refuse.

A sliced wordmark (T-series), a title that shares a stem across two words, a caption set in the same cut as the subject's handwriting, a folio that ticks like a clock. This lane includes letter-crop and scatter when they are the *moment*, not the cited violation.

**Fits when:** the violation was spatial or hierarchical (E1, G4, H1, D1) and type is still available.
**Does not fit when:** the direction already cites D8 or any T-ID. That *is* the typographic act.

### 3. Micro-interactions

A small behavior that rewards attention: a folio that updates with scroll time, a caption that swaps at the third hover, a rule that offset-prints on press-and-hold. Digital only, unless the print edition has a physical analog (a gatefold, a tip-in).

**Fits when:** the spread is already held and the brand has a temporal or tactile claim.
**Does not fit when:** the interaction *is* the product demo. That is marketing, not a moment.

### 4. Easter eggs

Something findable, not announced. A credit hidden in a gutter. A second story in the running head. A coordinate that maps to a real place in the piece. The reader who looks closer is paid; the reader who doesn't is not punished.

**Fits when:** the audience includes people who linger (subscribers, peers, the subject of the piece).
**Does not fit when:** the egg is the only content. Then it is the violation, and you need an ID.

### 5. Print / editorial craft surprises

Craft that print people notice and digital people feel: a named void, a sink that matches the story's pause, a caption that jumps the gutter, a show-through that is planned, a folio that continues a sentence from the previous spread. On a canvas tool, the analog is a visible system used as content (grid labels, coordinates, registration) *if and only if* G1 / E5 / T6 is not already the violation.

**Fits when:** the violation was conceptual or digital (D1, D2, H1) and the spread still looks like every other competent magazine.
**Does not fit when:** the direction already cites G4, E3, E5, or E12. Those *are* the craft surprise.

---

## Lane picker

Ask, in order:

1. **What lane is the violation already in?** Do not reuse it.
2. **What does the brand actually have?** A claim → lane 1. A voice or a wordmark → lane 2. A temporal product → lane 3. A lingering audience → lane 4. A print or craft audience → lane 5.
3. **Where is the beat?** Opener prefers 1 or 2. Body prefers 5 or 4. Breather prefers 4. Closer prefers 5 or 1.
4. **If two lanes still qualify, pick the quieter one.** The violation is the loud thing.

If no lane is free, skip the moment. Skipping is correct more often than forcing.

---

## Prompt stubs

After a direction is picked:

```
Direction {N} is locked. violate: {ID}. Hold every other inventory ID.
Add at most one clever moment. Lane must not be {lane of the grid break}.
Brand root: {metaphor or claim}. Reward, don't require.
```

If you want the skill to propose the moment (instead of inventing one in the executor):

```
Propose three clever-moment options for Direction {N}.
Each from a different remaining lane. One sentence each.
I will pick one or none.
```

Do not generate clever moments for all five directions up front. That is five extra violations dressed as garnish.

---

## Anti-patterns

- **Two moments.** A cropped wordmark *and* a hidden game *and* a witty caption. Pick one.
- **The moment is the layout.** If removing the moment destroys the spread, it was the violation. Cite an ID and drop the garnish.
- **Explainer required.** A footnote that says "this is a joke about…" is a failed fifth Condition.
- **Viral bait.** Confetti, a fake cursor, a personality-quiz nav. Shareable is a photograph of the spread. Viral is a different job.
- **Same-lane stack.** T1 violation + typographic moment. G4 violation + a named-void gag. You spent the budget twice.
- **Borrowed wink.** Konami codes, "lorem" jokes, agent-slop memes. Not brand-rooted.
- **Moment as compensation.** Using a clever trick to rescue a weak violation. Fix the violation.

---

## Tie-back

How this file sits next to the rest of the skill.

| Question | Answer |
|----------|--------|
| Is a clever moment a seventh technique? | No. Techniques still pick the *kind* of weirdness for the direction. The moment is optional garnish. |
| Is it a second convention ID? | No. If it needs an ID, it is a different direction. |
| How does it relate to the Five Conditions? | It must pass them in miniature: familiar enough to catch, purposeful, coherent with the spread, not instantly "oh, an Easter egg page," and it changes how you see the piece — or it is deleted. |
| How does it relate to the grid? | The grid is held. The moment does not redraw columns. See `references/editorial-grids.md`. |
| How does it relate to letter-crop? | Letter-crop is either the *violation* (T-series / D8) or a *lane-2 moment* on a non-type violation. Never both. See `references/letter-crop-scatter.md`. |
| When do I load this file? | After the human picks a direction. Not during the five-direction run. |

---

## One-spread budget (recap)

```
1 grid held
1 inventory ID violated
1 technique named
0 or 1 clever moment, other lane
0 explainers
```
