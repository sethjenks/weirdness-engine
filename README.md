# Weirdness Engine

> A Claude skill that pushes web and editorial designs toward productive strangeness — the outlier space where memorable, category-defying work lives.

Most AI design tools converge on the average. They aggregate references and produce work that looks like everything else in the category. "Make it weirder" without structure produces scattered randomness, which reads as broken rather than weird.

The Weirdness Engine works differently. It treats weirdness as a precision instrument: identify one convention with conviction, violate it, hold structure everywhere else. Maximum surprise at a single strategic point. Coherence everywhere else.

## What This Is

A skill that runs in three modes:

- **Critique Mode** — Hand it an existing design (Figma file, screenshot, URL). It inventories the conventions the design is obeying, names the assumptions hiding in plain sight, and produces five directions that each violate a different one.
- **Generate Mode** — Hand it a brand brief at project kickoff. It maps the category's conventions, identifies the brand's authentic territory, and produces five directions rooted in what makes that brand actually different from its competitors.
- **Layout Mode** — Hand it an editorial brief, a spread, or a request for grid / type-geometry originality. It cites convention IDs from the layout inventory and produces five directions that each violate exactly one. An editorial or Paper executor then builds with `violate: {ID}` and holds the rest.

Each run produces exactly five directions, each using a different technique, each targeting a different surface — so you get a real spread, not five variations on the same idea.

## What Makes It Different

Three things distinguish this skill from prompting Claude to "be more creative":

1. **Convention before violation.** Every direction begins by naming what it's breaking and why that convention exists. You can't violate what you haven't named. The skill enforces this discipline on every output.
2. **The Five Conditions.** Every direction must pass five tests: anchored familiarity, purposeful violation, internal coherence, irresolvable tension, and defamiliarizing effect. If a direction fails any one, it's reworked before it ships.
3. **The Six Techniques.** Collision, Alien Perspective, Exaggeration of Truth, Uncommon Care, Constraint Inversion, Outside Reference. Each produces a different *kind* of weirdness. Together they prevent the skill from collapsing into a single voice.

The methodology is grounded in Mark Fisher's ontology of the weird, Viktor Shklovsky's defamiliarization, and the cognitive science of expectancy violation. See `references/theory.md` for the full theoretical foundation.

## Installation

### Claude Code

Drop the `weirdness-engine/` folder into your `.claude/skills/` directory:

```bash
git clone https://github.com/<your-username>/weirdness-engine.git ~/.claude/skills/weirdness-engine
```

The skill registers automatically. Verify with `/skills` in Claude Code.

### Cowork

In Cowork mode, install via the skill picker or drop the packaged `.skill` archive into your skills directory. To package this repo for Cowork:

```bash
cd weirdness-engine
zip -r weirdness-engine.skill SKILL.md references/
```

Then upload the resulting `weirdness-engine.skill` file in Cowork.

### Claude API / Agent SDK

Reference `SKILL.md` as a system prompt or attach it as context. Reference files load on demand — `references/theory.md` for foundational reasoning, `references/techniques.md` for implementation detail, and the layout set (`layout-conventions.md`, `editorial-grids.md`, `clever-moments.md`, `letter-crop-scatter.md`) in Layout mode.

## Usage

### Generate Mode (project kickoff)

> "I'm designing a marketing site for a meditation app called Quiet Studio. The differentiator is that it treats meditation like a recording studio — sessions are tracks, users have a library, teachers are producers. The founders don't want it to look like every other meditation app. Run the weirdness engine."

The skill maps the category's conventions, identifies the brand's authentic territory, and returns five directions. See `examples/example-01-quiet-studio.md` for a full worked output.

### Critique Mode (existing design)

> "Here's the current homepage at <url>. Run the weirdness engine on it."

The skill inventories what the design is obeying, names the assumptions, and returns five directions to push it further.

### Layout Mode (editorial / Paper spreads)

> "We're designing the opener for a print + canvas feature. It should not look like an agent-default marketing page or a three-column magazine template. Run the weirdness engine in Layout mode."

The skill loads the convention inventory, cites IDs, and returns five directions that each violate exactly one. See `examples/example-02-layout-mode.md` for a full worked output.

### Going Deeper

> "Direction 2 is interesting — go deeper."

The skill shifts from provocation to implementation: specific CSS/JS/WebGL approaches, component breakdowns, motion language, accessibility considerations, performance tradeoffs.

## Methodology TL;DR

**The Weirdness Dial**

```
FORGETTABLE ←———————————→ ALIENATING
     |                          |
  safe, expected,          confusing, hostile,
  category average         no anchor point

              SWEET SPOT
            weird enough to
           stand out and stick,
          grounded enough to
              connect
```

Most AI output lands on the left. Genuinely alienating work lands on the right. The sweet spot is between — committed enough to register as intentional, anchored enough to remain navigable. Each run produces a spread across this dial so you can choose how far to push.

**The Core Mechanic**

Every direction follows the same five-step structure: name the convention, name the assumption beneath it, violate with a brand-rooted alternative, specify what stays conventional, explain why this violation could only belong to this brand. This is what separates productive weirdness from random noise.

## Repository Structure

```
weirdness-engine/
├── README.md                       This file.
├── LICENSE                         MIT.
├── SKILL.md                        The skill itself — invoked by Claude.
├── references/
│   ├── theory.md                   Fisher, Shklovsky, cognitive science of weirdness.
│   ├── techniques.md               Implementation-level detail for each technique.
│   ├── layout-conventions.md       Layout-mode inventory (E/D/H/G/P/T IDs).
│   ├── editorial-grids.md          Grid literacy and the hold.
│   ├── clever-moments.md           One surprise per spread; five lanes.
│   └── letter-crop-scatter.md      Type-as-geometry recipe.
├── examples/
│   ├── example-01-quiet-studio.md  A worked Generate Mode output.
│   └── example-02-layout-mode.md   A worked Layout Mode output.
└── .gitignore
```

## Credits

The methodology draws from:

- **Mark Fisher**, *The Weird and the Eerie* (2016) — the ontology of the weird as "the presence of that which does not belong."
- **Viktor Shklovsky**, *Art as Technique* (1917) — defamiliarization as the foundational creative move.
- **David Lynch** — the gold standard for productive weirdness emerging from within the familiar.
- **Liquid Death**, **Old Spice**, and other case studies — proof that this works commercially, not just artistically.
- Cognitive science: the **Von Restorff effect**, **Expectancy Violation Theory** (Burgoon), **Benign Violation Theory** (McGraw & Warren), and the **Meaning Maintenance Model** (Proulx & Heine).

Built by [Seth Jenks](https://github.com/sethjenks) at [Arcana](https://arcana.agency).

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, ship it. Attribution appreciated.

## Contributing

Issues and PRs welcome. The two areas where the skill benefits most from outside input:

- **More worked examples** in `examples/` — different categories, different brands, including Layout-mode editorial briefs. Real briefs that produced directions you actually shipped.
- **New techniques** — if you find a kind of weirdness the six techniques don't cover, document it the way `references/techniques.md` documents the existing six and propose it.

Anything that converges this skill toward the average is the wrong kind of contribution. Anything that sharpens its ability to depart from the average is the right kind.
