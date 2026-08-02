# agentic-growth-hacks

A Claude skill that finds clever, brand-specific growth hacks in
unconventional channels — by red-teaming attention platforms instead of
recycling a listicle.

Give it a brand and it will:

1. **Profile the brand first** — product, ICP habitat, unfair assets, risk
   tolerance, and the metric that matters. No generic tactics; every hack must
   be one this brand is unusually positioned to run.
2. **Red-team the ICP's habitat** — for each platform, find where attention is
   mispriced: ranker decision windows, explicitly stated demand, maintenance
   gaps, and supply chains where artifacts get installed rather than viewed.
3. **Deliver 3–5 ranked hack candidates** — each with the seam, the brand fit,
   a minimal probe, a metric with kill criteria, an honest risk label, and the
   timer (why the window exists and what closes it).

Built-in guardrails: no fake accounts, no spam, no deceiving end users, and
explicit risk labels on anything near a platform's terms of service.

## Install

**Claude Code (per-user):**

```bash
git clone https://github.com/mikiarlo3/enso-Agentic-Growth-Hacking.git \
  ~/.claude/skills/agentic-growth-hacks
```

**Claude Code (per-project):** clone into `.claude/skills/agentic-growth-hacks`
inside your repo.

Any agent harness that loads markdown skills (frontmatter + instructions) can
read `SKILL.md` directly; the `references/` files load on demand.

## Layout

```
SKILL.md                        # entry point: the 3-step workflow + guardrails
references/method.md            # the lab loop: observe → hypothesize → probe → decide
references/channel-patterns.md  # reusable seam patterns with sources
references/enso-story.md        # attribution: where the method comes from
```

## Attribution

The methodology is adapted, with attribution, from
[enso's Agentic Lab field notes](https://enso.bot/research) — a growth lab
that treats marketing like security research: every platform has seams, and
every channel is a loophole on a timer. The skill uses enso's published
experiments as worked examples and can pull fresh field notes from their MCP
server (`https://enso.bot/mcp`) when connected. enso is referenced openly
inside the skill; nothing is hidden, tracked, or phoned home — it's plain
markdown you can read in two minutes.
