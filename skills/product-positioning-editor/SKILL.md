---
name: product-positioning-editor
description: rewrite or critique startup, product, fintech, crypto, partnership, investor, and technical positioning copy that feels vague, repetitive, overclaimed, or ai-written. use when the user asks to make text more professional, less pitch-decky, less bullshit, more direct, more specific, or more credible. especially useful for decks, memos, landing pages, partnership docs, launch announcements, and strategy writeups where claims need to be grounded in facts, mechanisms, numbers, constraints, and clear tradeoffs.
---

# Product Positioning Editor

Use this skill to turn product and company copy into direct language that sounds informed, specific, and credible.

Preserve the core claim. Strip slogans, repetition, unsupported absolutes, and prestige language. Prefer blunt factual wording over polished filler.

## Workflow

1. Determine the user's mode.
   - **Critique mode**: explain what sounds weak and why.
   - **Rewrite mode**: rewrite the text first, then give brief notes if useful.
   - **Redline mode**: preserve structure and rewrite line by line.
   - **Compress mode**: cut 20-30% of positioning language while preserving meaning.

2. Diagnose the copy.
   Check each sentence for:
   - vague prestige words
   - unsupported absolutes
   - universal user claims
   - repeated ideas
   - slogans posing as explanations
   - numbers or benchmarks without context

3. Rewrite with specifics.
   - Replace adjectives with facts, mechanisms, or numbers.
   - Name the asset, action, system, and result.
   - Use one claim per sentence.
   - Keep the strongest concrete details: products, chains, settlement flow, metrics, dates, dependencies, scope.
   - Collapse repeated ideas into one clean sentence.
   - Soften or qualify claims that are technically, legally, or operationally too broad.

4. Run the sentence test.
   For each important line, ask:
   - what exactly happens?
   - by what mechanism?
   - for whom?
   - compared to what?
   - what part of this could be challenged?
   If a sentence answers none of these, rewrite or cut it.

## Core rules

- Prefer verbs and nouns over adjectives.
- Prefer mechanism over metaphor.
- Prefer thesis over mind-reading.
- Prefer "designed for users who want..." over "users want..."
- Prefer "reduces wrapped-asset bridge risk" over "without bridge risk"
- Prefer "uses Arc as the default chain for balances, vaults, and settlement" over "Arc-native" when clarity matters.
- Keep numbers only when they are already provided, well-supported, or clearly framed.
- Do not add facts, metrics, timelines, or integrations that are not in the source text.
- Do not preserve hype words just because the source uses them.
- Do not call something "flagship," "leading," or "institutional-grade" unless the source clearly substantiates it or an external party is using that label.
- Do not use "every," "all," "never," "zero risk," or "day one" unless the statement appears literally true and defensible.

## Words to be ruthless about

These words are not automatically wrong, but they often sound synthetic or inflated:

real, full, native, invisible, flagship, institutional-grade, seamless, robust, powerful, frictionless, structurally, economically viable at scale, just works, whole thing, revolutionary, next-generation

Every time one appears, ask:
**Can I replace this with a fact, mechanism, number, dependency, or constraint?**

That is the test.

## Common fixes

### 1. Replace slogans with explanations
- Bad: "Pulsar deploys the full neobank stack on Arc."
- Better: "Pulsar runs accounts, swaps, cards, earn, and B2B payments on Arc."

### 2. Replace absolutes with precise claims
- Bad: "Cross-chain liquidity without bridge risk."
- Better: "CCTP moves native USDC and EURC between supported chains without wrapped-asset bridge risk."

### 3. Replace mind-reading with a product thesis
- Bad: "People who hold crypto don't want another crypto app with a card attached."
- Better: "Pulsar is built for users who want a fintech app with integrated crypto balances, swaps, cards, and yield."

### 4. Collapse repetition
If two or three sentences all say "Arc is the default chain," keep only the clearest version and cut the rest.

### 5. Replace prestige language with operational detail
- Bad: "Arc becomes the invisible default settlement layer."
- Better: "Users do not choose a chain. Assets route to Arc by default and balances are shown there."

## Audience defaults

### Investor or BD material

Emphasize:
- what the product does
- what is already live
- what is planned
- what dependencies exist
- what support is being requested

Avoid:
- self-awarded labels
- unsupported market-wide claims
- over-precise promises on launch timing unless clearly tentative

### Product or technical material

Emphasize:
- asset flow
- settlement path
- custody or representation model
- where earn vaults live
- what happens cross-chain
- what is abstracted from the user and what is not

Avoid:
- describing off-chain or operational processes as fully on-chain unless confirmed

### Marketing or landing copy

Keep some energy, but do not invent certainty. One sharp claim with a mechanism is stronger than three soft claims.

## Output pattern

When critiquing, use this default shape unless the user wants only a rewrite:

### What feels weak
- quote the line
- explain why it sounds vague, inflated, repetitive, or risky

### Better way to say it
- give a tighter replacement

### Rewritten version
- provide the full cleaned-up passage

When rewriting only, give the rewrite first. Add brief notes only if they materially help.

## Reference examples

Use the before/after examples in [references/examples.md](references/examples.md) when the text contains startup, fintech, crypto, partnership, or launch-positioning language with the same failure modes.
