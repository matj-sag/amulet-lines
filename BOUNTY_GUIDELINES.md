# Bounty Guidelines

Guidelines for writing, solving, and verifying bounties for Amulet combo lines.

A bounty is a precise request for a combo line under specified starting conditions. Bounties should be written so that another player can independently check whether a proposed line works.

## Table of Contents

- [Default Bounty Assumptions](#default-bounty-assumptions)
- [What Makes a Bounty Solution Valid?](#what-makes-a-bounty-solution-valid)
- [How to Submit a Solution](#how-to-submit-a-solution)
- [Bounty Template](#bounty-template)

## Default Bounty Assumptions

Unless a bounty explicitly says otherwise, every bounty uses the following assumptions:

1. Your graveyard starts empty.
2. You cannot mill.
3. You cannot draw.
4. You have no land drop available.

A bounty may override one or more of these assumptions, but it must say so explicitly.

For example:

```md
Special assumptions:
- You have one land drop available.
- Your graveyard contains exactly Shifting Woodland and Simic Growth Chamber.
```

## What Makes a Bounty Solution Valid?

A valid bounty solution must satisfy the exact starting conditions and success condition of the bounty.

In general, a solution should establish a self-contained engine or deterministic result during the combo turn. Unless the bounty says otherwise, it is not enough to merely generate a large amount of mana once or pass the turn hoping to continue later.

## How to Submit a Solution

A proposed solution should include enough detail to be replayed exactly.

Please include:

- Starting battlefield.
- Starting hand.
- Starting graveyard.
- Floating mana.
- Whether a land drop is available.
- Relevant library contents.
- Each search/tutor choice.
- Mana produced and spent at each important step.
- Trigger ordering when relevant.
- Final result.

Prefer this format:

```md
## Bounty Name

### Starting Conditions

- Battlefield:
- Hand:
- Graveyard:
- Floating mana:
- Land drop available:
- Relevant library contents:

### Line

1. ...
2. ...
3. ...

### Result

Describe the established engine, kill, or deterministic result.

### Notes

Mention assumptions, alternate choices, or verification details.
```

## Bounty Template

Copy this template when adding a new bounty to [`BOUNTIES.md`](./BOUNTIES.md).

```md
## Bounty: <Short Name>

### Status

Open

### Starting Conditions

- Battlefield:
- Hand:
- Graveyard: Empty, unless otherwise specified.
- Floating mana:
- Land drop available: No, unless otherwise specified.
- Relevant library contents:

### Default Assumptions

This bounty uses the default bounty assumptions unless overridden below.

### Special Assumptions

- None.

### Goal

Find a line that achieves:

- <success condition>

### Restrictions

- <restriction>
- <restriction>

### Notes

- <note>
```
