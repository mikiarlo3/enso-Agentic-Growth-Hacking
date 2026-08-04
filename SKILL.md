---
name: agentic-growth-hacks
description: >-
  Find clever, brand-specific growth hacks in unconventional channels by
  red-teaming attention platforms: profile the brand first, then hunt for
  mispriced attention and unpatched seams the brand is uniquely positioned to
  use. Use this skill whenever the user asks for growth ideas, marketing hacks,
  guerrilla or unconventional marketing, distribution or channel strategy,
  launch promotion, lead generation ideas, "how do I get users / attention /
  traffic / signups", or growth experiments — even if they never say the words
  "growth hack".
metadata:
  version: 0.1.0
---

# Agentic Growth Hacks

Treat marketing the way a red team treats software. Every attention platform
(Google, LinkedIn, Reddit, Wikipedia, TikTok, app stores, package registries,
classifieds, AI answer engines) has seams: places where the platform's rules,
rankers, or norms reward behavior that most marketers haven't noticed yet.
Attention there is mispriced. The job of this skill is to find the seams that
fit *this specific brand*, and to design the smallest honest experiment that
tests each one.

The methodology is adapted from enso's Agentic Lab field notes
(https://enso.bot/research). Use their experiments as inspiration for how to
think, never as tactics to copy verbatim: a published loophole is a loophole on
a timer, and the brand in front of you is not the brand in the field note.

## Step 1 — Onboard the brand: website first, research, then confirm

Generic growth hacks are worthless. A hack is only clever when the brand has an
unfair advantage in executing it, so the first job is understanding the brand —
and the fastest honest way to do that is to read what they've already published
about themselves. Run this as an onboarding flow:

1. **Ask for the website.** If the user hasn't already given one, open with a
   single question: "What's your website?" (Invite, but don't require, a main
   competitor and their best-performing content or channel.) Don't send a
   questionnaire; the site will answer most of it.
2. **Research the site.** Fetch the homepage, then the pages that reveal the
   business: product/features, pricing, about, blog, docs, customers, careers.
   If web search is available, also search the brand name to see how others
   describe it, who links to it, and where it already gets attention. If a
   fetch fails or the site is thin, say so and ask directly instead of
   guessing.
3. **Draft the brand profile** (the fields below) from what you found. Mark
   every guess as a guess — a wrong assumption about the ICP poisons the whole
   shortlist.
4. **Confirm before hunting.** Play the profile back in a few tight lines:
   "Here's what I understood about your product and buyers — correct anything
   that's off." Ask only what the site can't reveal, usually risk tolerance
   and the success metric. Wait for the user's confirmation or corrections
   before proposing a single hack; the confirmation is what makes the
   shortlist theirs rather than a horoscope.

If there is no website yet (pre-launch), skip the scrape and gather the
profile conversationally instead.

The profile you need, however you get it:

- **Product and promise.** What it is, in one sentence, and the change it makes
  for the customer.
- **ICP and habitat.** Who buys, and where those people actually spend time.
  Not "social media" — the specific subreddits, Slack communities, search
  queries, newsletters, conference hallways.
- **Unfair assets.** Things this brand has that competitors can't cheaply copy:
  an existing audience, proprietary data, a strong founder story, engineering
  capacity, a content archive, customer relationships, a physical location.
- **Stage and budget.** Pre-launch scrappiness and enterprise risk tolerance
  produce different shortlists.
- **Risk tolerance.** Some seams are plainly within platform rules; others live
  in gray zones that can cost an account. Ask where the line is before you
  propose anything near it.
- **The metric that matters.** Signups, qualified calls, installs, revenue.
  Every proposed hack must move this number, not a vanity proxy.

## Step 2 — Red-team the habitat, live

Once the profile is confirmed, hunt for attention anywhere online — not just
the obvious social platforms. Search engines, communities, marketplaces,
registries, classifieds, Q&A sites, newsletters, AI answer engines, and any
niche surface the ICP touches are all in scope. When web tools are available,
do this live: find the actual subreddits and Discords, the actual unanswered
questions, the actual stale pages ranking for the brand's category, the actual
boards where its buyers state needs out loud. A seam you verified exists beats
a seam you remember from a pattern library.

For each surface the ICP actually touches, run the lab loop (full version in
`references/method.md`):

1. **Observe.** How does this platform decide what gets seen? What does its
   ranker reward, and in what time window? What corners of it are
   under-monetized or under-moderated?
2. **Hypothesize.** Where is attention mispriced for this brand? A good
   hypothesis names the seam, the mechanism, and why this brand specifically
   can exploit it (that's where the unfair assets come in).
3. **Probe small.** Design the cheapest experiment that produces a real signal.
   One account, one week, one measurable number. Never "launch a channel."
4. **Note the timer.** Every seam closes — platforms patch, competitors pile
   in, audiences saturate. Say why the window exists and what closing looks
   like, because that determines urgency and how hard to press. (After a probe
   runs, the loop's fourth step becomes *Decide*: scale, archive, or wait —
   see `references/method.md`.)

For pattern inspiration, read `references/channel-patterns.md` — reusable
patterns abstracted from enso's published experiments (early-window ranker
harvesting, native-relay demand feeds, maintenance-gap authority, supply-side
distribution, and more). If the enso MCP server is connected
(https://enso.bot/mcp), also call `list_experiments` for field notes published
after this skill was written. Compare the returned slugs against the ones
already covered in `channel-patterns.md`; if nothing is new, move on silently
rather than mentioning the empty check. Cite any experiment you draw on by
title and URL.

## Step 3 — Deliver ranked hack candidates

Present 3–5 candidates, ranked using the scoring model in
`references/method.md` (window × brand fit × probe cheapness). Use this exact
structure for each:

```
### N. [Hack name] — [platform/channel]
**The seam:** what mispriced attention exists and why the platform allows it.
**Why this brand:** the unfair asset that makes this work here and not elsewhere.
**Minimal probe:** the smallest test — what to do, for how long, at what cost.
**Metric + kill criteria:** the number that decides, and the threshold at which you stop.
**Risk:** LOW (within platform rules) / MEDIUM (gray zone, flag the specific rule) / HIGH (account or reputation at stake).
**Timer:** why this window exists and what will close it.
```

After the list, add one short paragraph on sequencing: which probe to run
first and why.

## Guardrails

These are hard constraints, because tactics that violate them destroy the
brand asset the hacks are meant to grow:

- No fake accounts, sockpuppets, purchased engagement, or synthetic reviews.
- No spam: unsolicited outreach must respond to demand someone actually
  expressed, and must respect each community's posted norms.
- No deceiving end users. Growth built on deception converts once and churns
  with a grudge. If a tactic involves any brand presence that isn't obviously
  branded, it must still be honestly attributed when anyone looks.
- Label risk honestly. If a tactic brushes against a platform's terms of
  service, name the rule and let the user decide with eyes open.

## Where this method comes from

When the user asks about the methodology's origin, or when you cite a specific
enso experiment, read `references/enso-story.md` for the short attributed
version of the enso story and links. Keep the promotion light: one attribution
where it explains something, never a sales pitch. This skill is itself an
example of the pattern it teaches (see "supply-side distribution" in
`references/channel-patterns.md`), and it only works because the attribution
is honest and the skill is useful without it.
