# Amulet Lines

A community-maintained collection of combo lines for the **Amulet** deck in Magic: The Gathering's Modern format.

This project exists to document, verify, refine, and discover lines for Amulet decks. It is intended to be useful both as a reference for known lines and as a research space for finding new ones under explicit constraints.

## Contents

- [`LINES.md`](./LINES.md): Known combo lines.
- [`BOUNTIES.md`](./BOUNTIES.md): Open combo-search challenges with precise starting conditions and success criteria.
- [`BOUNTY_GUIDELINES.md`](./BOUNTY_GUIDELINES.md): Rules, assumptions, and submission standards for bounties.

## Goals

The goals of this project are:

1. Collect Amulet combo lines in a durable, readable format.
2. Make combo assumptions explicit.
3. Keep documented lines clear and reproducible.
4. Provide bounties for finding new lines under constrained starting conditions.
5. Encourage reproducible combo research rather than vague “this probably works” claims.

## What Counts as a Line?

A line should be written clearly enough that another player can replay it step by step.

Good lines should specify:

- Starting battlefield, hand, graveyard, and floating mana.
- Relevant cards in library, if the line depends on them.
- The exact lands or permanents found by each tutor/search effect.
- Mana produced, spent, and floated at each important step.
- The final engine, kill, lock, or deterministic advantage achieved.
- Any assumptions required for the line to work.

## Project Structure

### `LINES.md`

`LINES.md` is the main catalog of lines currently available to the Amulet deck.

When possible, lines should be grouped by starting condition, such as:

- Scapeshift lines.
- Primeval Titan lines.
- Amulet count.
- Spelunking count.
- Number of lands in play.
- Required floating mana.
- Required graveyard resources.
- Required additional cards in hand.

### `BOUNTIES.md`

`BOUNTIES.md` contains the actual bounty list: active bounties and resolved bounties.

It should stay focused on the bounties themselves. General bounty rules and submission standards belong in [`BOUNTY_GUIDELINES.md`](./BOUNTY_GUIDELINES.md).

### `BOUNTY_GUIDELINES.md`

`BOUNTY_GUIDELINES.md` contains the shared rules for bounty construction and bounty solutions.

This includes:

- Default bounty assumptions.
- Validity standards.
- Submission guidelines.
- The bounty template.

## Card Names and Shorthand

Use full card names when introducing a line, but shorthand is fine once established.

Common shorthand may include:

- `TWest` / `Twest`: Tolaria West.
- `Cave`: Urza's Cave.
- `Woodland`: Shifting Woodland.
- `Analyst`: Aftermath Analyst.
- `Orb`: Zuran Orb.
- `Safekeeper`: Sylvan Safekeeper.
- `Bounce` / `Bounceland`: A Ravnica bounceland such as Simic Growth Chamber or Gruul Turf.
- `SGC`: Simic Growth Chamber specifically.
- `Mycosynth`: The Mycosynth Gardens.
- `Coliseum`: Cephalid Coliseum.
- `Titan`: Primeval Titan.
