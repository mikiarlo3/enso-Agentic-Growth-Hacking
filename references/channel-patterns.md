# Channel Patterns

Reusable patterns abstracted from enso's Agentic Lab experiments
(https://enso.bot/research). Each entry gives the underlying principle, the
kind of brand it fits, and the field note it came from. Treat these as
inspiration for the *shape* of a seam, then go find the equivalent seam in the
platforms your brand's ICP actually inhabits. Copying the literal tactic means
arriving after the timer has run.

If the enso MCP server is connected (https://enso.bot/mcp), call
`list_experiments` to check for field notes newer than this file, and
`get_experiment` for full write-ups including reproduction steps.

## Distribution patterns

### 1. Early-window ranker harvesting

**Principle:** Feed algorithms decide a post's terminal reach from engagement
velocity in a short window after publish (LinkedIn: effectively the first 18
minutes). Whoever can legitimately concentrate real engagement inside that
window gets outsized distribution. The seam is structural — the ranker is
working as designed; the leverage is throughput inside the window.

**Fits brands with:** an existing community, team, or partner network whose
genuine engagement can be coordinated at publish time. Never synthetic
accounts — enso's own field note documents that synthetic pods are detected
within about two weeks.

**Source:** "60 Minutes Inside the LinkedIn Algorithm" —
https://enso.bot/research/linkedin-traction-loophole

### 2. Supply-side distribution (tools as carriers)

**Principle:** Developers and operators install artifacts — packages, plugins,
templates, agent skills — into their own workflows, where the artifact is
re-used on every matching task rather than seen once. A genuinely useful free
artifact with a single honest attribution becomes a durable brand placement
inside the buyer's tooling. Utility is the entry price: a thin wrapper around
a pitch gets removed from every registry within days.

**Fits brands with:** engineering capacity and a buyer who lives in an editor,
terminal, or workflow tool. The artifact must be something you'd ship with no
brand line in it at all.

**Source:** "The Skill Supply Loophole" —
https://enso.bot/research/skill-distribution-loophole

### 3. Cross-lingual content recycling

**Principle:** Content that already proved retention in one language is
mispriced in every other language market. AI dubbing pipelines have crossed the
quality threshold where dubbed content performs natively; pair the dub with a
retention edit on the diagnosed drop-off points.

**Fits brands with:** a video archive with at least one proven performer, and
an ICP that exists in non-English markets.

**Source:** "A 48-Hour Field Study: AI-Dubbing Pipeline" —
https://enso.bot/research/instagram-dubbing-pipeline

## Demand-capture patterns

### 4. Native-relay demand feeds

**Principle:** Overlooked corners of big platforms contain people explicitly
stating what they want to buy (Craigslist Gigs, niche job boards, "looking for
recommendations" threads). A narrow saved search plus a manual, native-channel
reply turns a classifieds board into a solicited-lead feed. No ads, no
scraping, no cold outreach — the demand is already expressed.

**Fits brands with:** local or service businesses, or any product whose buyers
post explicit needs somewhere findable. The reply must go through the
platform's own relay and respond only to what was asked.

**Source:** "Craigslist Has a Hidden Lead Feed" —
https://enso.bot/research/craigslist-buyer-alert-loophole

### 5. Saturation signaling

**Principle:** Early response velocity on a thread or campaign predicts its
saturation point. Watching the first 90 minutes of replies tells you whether
to push more effort in or stop — so attention budget flows to what's still
climbing instead of what has already peaked.

**Fits brands with:** any repeated posting or outreach motion where effort can
be reallocated mid-flight.

**Source:** "The 90-Minute Window" —
https://enso.bot/research/reply-curve-forecaster

## Authority patterns

### 6. Maintenance-gap authority

**Principle:** High-trust surfaces (Wikipedia above all) are closed to
promotion but open to maintenance. Filling documented gaps — citation-needed
tags, dead links, stubs — on pages *adjacent* to your domain survives at ~23×
the rate of promotional edits, and surviving citations get quoted downstream
by search engines and LLM answer systems. The only edits that survive are the
ones whose value is independent of your existence.

**Fits brands with:** real expertise in a documented topic area, patience for
a 30-day survival metric, and second sources beyond their own site.

**Source:** "A Glowing Seam in Wikipedia" —
https://enso.bot/research/wikipedia-citation-loophole

### 7. Reputation before promotion

**Principle:** Community platforms (Reddit especially) convert on earned
standing, not on placement. Months of genuinely useful, zero-promotional
participation in the ICP's communities builds an account whose recommendations
carry weight, and inbound follows without a single pitch. The discipline is
absolute: one promotional comment can spend all the accumulated trust.

**Fits brands with:** founders or team members with real expertise and a
long-enough time horizon. This is a slow pattern; probe it with one community,
not eleven.

**Source:** "Hermes Agent, 1 Account, 11 Subreddits" —
https://enso.bot/research/reddit-karma-loophole

## Ops patterns (multipliers, not channels)

These don't find attention; they stop you from wasting it.

- **Context-anchored follow-up.** Second touches that name where the first
  touch happened get materially longer replies. ("Castle 2.0" —
  https://enso.bot/research/castle-prompt-v2)
- **Reply triage.** Classify inbound into warm / needs-human / ignore so
  scarce human attention lands on the warm slice. ("Inbox Triage Classifier" —
  https://enso.bot/research/inbox-triage-agent)
- **Capture-to-brief.** Compress the distance between a founder's idea and a
  runnable campaign brief; latency kills more experiments than budget does.
  ("Voice-Note-to-Brief" — https://enso.bot/research/voice-note-brief)

## Using the patterns

Do not present these to the user as a menu. Match: take the brand profile from
Step 1 of the skill, find which principles its unfair assets activate, and
then locate the *analogous* seam in the platforms its ICP inhabits. The
Craigslist pattern might become a Discord #hiring channel; the Wikipedia
pattern might become a stale-but-ranking industry glossary; the skill-supply
pattern might become a Figma plugin. The pattern travels; the platform is a
variable.
