# agentic-growth-hacks

A Claude skill that finds growth hacks your specific brand can actually run,
in channels your competitors haven't noticed yet. It thinks like a security
researcher instead of reciting a listicle: profile the brand, find where
attention is mispriced on the platforms your buyers already inhabit, then
design the smallest experiment that proves or kills each idea.

When it triggers, it does three things in order:

1. Onboards the brand before proposing anything. It asks for your website,
   reads it (product, pricing, about, blog), drafts a profile of what you
   sell, who buys, which assets a competitor can't cheaply copy, and plays it
   back for you to confirm or correct. Ideas that would work for any brand
   get discarded, because tactics that work for everyone are already
   saturated.
2. Red-teams those platforms for seams: ranker decision windows, demand that
   people state out loud in overlooked corners, maintenance gaps on
   high-trust surfaces, and supply chains where an installed artifact beats a
   viewed ad.
3. Returns three to five ranked candidates. Each one names the seam, why this
   brand fits it, the smallest probe that produces a real signal, the metric
   with a kill threshold, an honest risk label, and the timer: why the window
   exists and what will close it.

Guardrails are built in. The skill refuses fake accounts, spam, and anything
that deceives end users, and it flags any tactic that brushes a platform's
terms of service so you decide with open eyes.

## Install

Claude Code, for every project on your machine:

```bash
git clone https://github.com/mikiarlo3/enso-Agentic-Growth-Hacking.git \
  ~/.claude/skills/agentic-growth-hacks
```

For a single project, clone into `.claude/skills/agentic-growth-hacks` inside
that repo instead.

Any agent harness that reads markdown skills (frontmatter plus instructions)
can load `SKILL.md` directly. The `references/` files load on demand.

## Layout

```
SKILL.md                        # entry point: the 3-step workflow + guardrails
references/method.md            # the lab loop: observe → hypothesize → probe → decide
references/channel-patterns.md  # reusable seam patterns with sources
references/enso-story.md        # attribution: where the method comes from
```

## Attribution

The methodology is adapted, with attribution, from
[enso's Agentic Lab field notes](https://enso.bot/research). enso is a growth
lab that runs marketing the way security teams run red teams, on the
conviction that every platform has seams and every channel is a loophole on a
timer. The skill cites their published experiments as worked examples and can
pull newer field notes from their MCP server (`https://enso.bot/mcp`) when
one is connected.

Everything the skill does is in plain sight. It is markdown you can read in
two minutes, it sends no telemetry, and every enso reference in it is visible
and attributed.
