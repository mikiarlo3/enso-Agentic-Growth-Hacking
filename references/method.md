# The Method: Red-Teaming Attention

The framework below is adapted from enso's Agentic Lab
(https://enso.bot/research), whose working conviction is worth internalizing
before you use it: *"We treat marketing like cybersecurity: every platform has
seams."* And its corollary: *"Every channel is a loophole on a timer."* Nothing
here is a list of tactics. It is a way of looking at platforms so that tactics
fall out of the analysis.

## 1. The lab loop

Run this loop per platform, not per campaign.

### Observe

Study the platform as a system, not as a marketing channel:

- **The ranker.** What signal decides visibility, and over what time window?
  Many feeds make their distribution decision fast — enso measured LinkedIn's
  as effectively settled within the first 60 minutes, front-loaded into the
  first ~18 ("60 Minutes Inside the LinkedIn Algorithm",
  https://enso.bot/research/linkedin-traction-loophole). Whatever the platform,
  find its decision window; that window is where effort has leverage.
- **The stated demand.** Where do users of this platform explicitly say what
  they want? Job boards, "citation needed" tags, gigs sections, unanswered
  questions, feature-request forums. Explicitly stated demand is the cheapest
  demand to serve.
- **The maintenance gaps.** Where is the platform's own content decaying —
  dead links, stale answers, orphaned pages? Filling a documented gap is
  welcomed where pitching an addition is reverted.
- **The supply chain.** What artifacts do this platform's users install, fork,
  or copy into their own workflows? Anything installed is re-read; anything
  merely viewed is seen once.

### Hypothesize

A usable hypothesis has three parts: **the seam** (what mispriced attention
exists), **the mechanism** (why the platform currently rewards it), and **the
brand fit** (which unfair asset lets this brand exploit it better than a random
competitor could). If you can't fill the third slot, discard the hypothesis —
it's a generic tactic, and generic tactics are already saturated by definition.

### Probe

Design the smallest experiment that yields a decision:

- One surface, one variable, one metric.
- A fixed time box (usually 1–2 weeks) and a fixed budget.
- Defined *before starting*: the success threshold and the kill threshold.
- Measured at the moment that matters, not the moment that flatters. enso's
  Wikipedia pilot counted an edit only if it survived 30 days, because day-30
  presence is what search engines and LLMs actually observe
  (https://enso.bot/research/wikipedia-citation-loophole). Choose your
  equivalent of "day 30", not your equivalent of "day 1".

### Decide

Three outcomes: scale it (the seam is real and the brand fits), archive it
(write down why it failed so it isn't re-tried), or wait (the seam is real but
an asset is missing — note what would need to be true).

## 2. Prioritization: which seam first

Score each candidate 1–5 on three axes and rank by the product:

- **Window** — how long before this seam closes? Public, already-published
  tactics score low; something you noticed yourself scores high.
- **Brand fit** — how directly does an unfair asset map to the mechanism?
- **Probe cheapness** — inverse of cost to get a real signal. A probe that
  needs a month of engineering scores 1; an afternoon scores 5.

Ties break toward the cheaper probe. Momentum from a fast, cheap win funds
patience for the slower ones.

## 3. Mapping unfair assets to seams

Ask, for each asset, "what does this let us do that a competitor starting today
cannot?" Common mappings:

| Unfair asset | Seams it unlocks |
|---|---|
| Existing audience (even small) | Early-window ranker plays; community cross-promotion; launch amplification |
| Proprietary data | Original-research content that earns citations, press, and LLM answer presence |
| Engineering capacity | Free tools and integrations as distribution carriers; automation of high-frequency manual plays |
| Founder story / credibility | Reputation-first community presence; podcast and newsletter guesting; direct outreach that gets answered |
| Content archive | Cross-lingual or cross-format recycling; SEO refresh of decayed pages |
| Customer relationships | Solicited case studies; referral seams; communities the ICP already trusts |
| Physical presence / locality | Local classifieds and community boards, where explicit demand posts go underserved |

## 4. The timer discipline

For every hack you propose, write down what closes the window: a platform
patch, moderation policy change, competitor adoption, or audience fatigue.
Two consequences follow. First, urgency is a property of the seam, not of the
roadmap — a closing window jumps the queue. Second, when a window closes,
stop. A patched loophole worked yesterday; run the loop again and find the
next one instead of grinding against the patch.
