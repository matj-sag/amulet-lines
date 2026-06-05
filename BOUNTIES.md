# Bounties

Open and resolved combo-search challenges for Amulet in Modern.

For the rules governing bounties, see [`BOUNTY_GUIDELINES.md`](./BOUNTY_GUIDELINES.md).

## Table of Contents

- [Open Bounties](#open-bounties)
- [Resolved Bounties](#resolved-bounties)

## Open Bounties

## Bounty: 1 Spelunking, 0 Amulet, 5-Land Scapeshift

### Status

Open

### Offered By

@aljce

### Reward

500 USD for a valid accepted solution.

### Starting Conditions

* Battlefield:

  * 1 Spelunking.
  * 0 Amulet of Vigor.
  * 5 lands:

    * 1 Simic Growth Chamber.
    * 4 Forest.
* Hand:

  * Scapeshift.
* Graveyard:

  * Empty.
* Floating mana:

  * 1, after casting Scapeshift.
* Land drop available:

  * No.
* Other resources:

  * None.

### Default Assumptions

This bounty uses the default bounty assumptions from [`BOUNTY_GUIDELINES.md`](./BOUNTY_GUIDELINES.md).

### Special Assumptions

* The starting lands before casting Scapeshift are exactly Simic Growth Chamber and four Forests.
* The line begins with exactly 1 floating mana.

### Goal

Find a line that establishes a deterministic Analyst loop or win from the stated position.

### Deckbuilding Restriction

The submitted line must be legal using the following list, with **at most three cards changed** from the list:

```txt
1 Aftermath Analyst
4 Amulet of Vigor
4 Arboreal Grazer
3 Boseiju, Who Endures
3 Crumbling Vestige
1 Cultivator Colossus
1 Dryad Arbor
1 Echoing Deeps
3 Forest
3 Green Sun's Zenith
4 Gruul Turf
1 Hanweir Battlements
3 Malevolent Rumble
1 Mirrorpool
1 Otawara, Soaring City
3 Primeval Titan
3 Scapeshift
1 Shifting Woodland
3 Simic Growth Chamber
4 Spelunking
2 Summoner's Pact
3 The Mycosynth Gardens
1 Tolaria West
1 Urza's Cave
4 Urza's Saga
1 Vexing Bauble
1 Zuran Orb
```

### Notes

* The changed card(s) should be explicitly identified in the submitted solution.

## Bounty: 2 Amulet Titan Kill That Does Not Die to Spelunking

### Status

Open

### Offered By

@aljce

### Reward

500 USD for a valid accepted solution.

### Starting Conditions

* Battlefield:

  * 2 Amulet of Vigor.
  * Spelunking.
* Hand:

  * Primeval Titan.
* Graveyard:

  * Empty.
* Floating mana:

  * 0, after casting Titan.
* Land drop available:

  * No.
* Other resources:

  * None.

### Default Assumptions

This bounty uses the default bounty assumptions from [`BOUNTY_GUIDELINES.md`](./BOUNTY_GUIDELINES.md), unless explicitly overridden here.

### Special Assumptions

* The line starts with 2 Amulet of Vigor and Primeval Titan as the only relevant resources.
* The line must produce a deterministic kill.
* The line must not “die to Spelunking.”

### Goal

Find a deterministic Primeval Titan line from the stated position that kills the opponent and does not fail in the presence of Spelunking.

For this bounty, a line “dies to Spelunking” if it relies on lands entering tapped in a way that would stop working when Spelunking causes those lands to enter untapped instead.

### Deckbuilding Restriction

The submitted line must be legal using the following list, with **at most two cards changed** from the list:

```txt
1 Aftermath Analyst
4 Amulet of Vigor
4 Arboreal Grazer
3 Boseiju, Who Endures
3 Crumbling Vestige
1 Cultivator Colossus
1 Dryad Arbor
1 Echoing Deeps
3 Forest
3 Green Sun's Zenith
4 Gruul Turf
1 Hanweir Battlements
3 Malevolent Rumble
1 Mirrorpool
1 Otawara, Soaring City
3 Primeval Titan
3 Scapeshift
1 Shifting Woodland
3 Simic Growth Chamber
4 Spelunking
2 Summoner's Pact
3 The Mycosynth Gardens
1 Tolaria West
1 Urza's Cave
4 Urza's Saga
1 Vexing Bauble
1 Zuran Orb
```

### Notes

* The changed card(s) should be explicitly identified in the submitted solution.
* The solution should explicitly explain why the line does not die to Spelunking.

### Proposed solution

Proposed solution by Matt Johnson

#### Starting Conditions

- Battlefield:
  - 2 Amulet of Vigor.
  - Spelunking (optional)
- Hand:
  - Primeval Titan.
- Graveyard:
  - Empty.
- Floating mana:
  - 0, after casting Titan.
- Land drop available:
  - No.
- Relevant library contents:
  - Mirrorpool
  - Echoing deeps x2 (additional card 1)
  - Vesuva (additional card 2)
  - 3 any colour bounce, 1 red bounce
  - Oran Rief the vastwood (additional card 3)
  - Kavaron, Memorial World (additional card 4)

#### Line

1. Cast titan get Mirropool+ Bounce (1 titan)
2. Float Cxxxx, bounce the bounce, activate mirrorpool to copy titan (2 titans)
3. Get Echoing Deeps+ bounce
4. Copy mirrorpool, Float Cxxxx, bounce the bounce, activate mirrorpool to copy titan (3 titans)
5. Get Echoing Deeps+ bounce
6. Copy mirrorpool, Float Cxxxx, bounce the bounce, activate mirrorpool to copy titan (4 titans)
7. Get Kavaron, Memorial World+ red bounce
8. Float Rx(xx), bounce the bounce (stack empty). Station Kavaron with 2 titans (12), then activae Kavaron to give the remaining 2 haste
9. Attack, get 2 titan triggers
10. First one get Oran Rief (2 untaps) and anything, tap Oran Rief twice
11. Second one get Vesuva and anything, copy Oran Rief (2 untaps) and tap it twice
12. Titans are now both 10/10 for 20 damage.

#### Result

Attack for 20

#### Notes

All lands have 'enters tapped' on them, so all untap twice even under spelunking.

This line is +4 cards, but only because the original list doesn't have vesuva. Most lists will have 1 vesuva

## Resolved Bounties

Move solved bounties here once a valid line has been found and checked.

Each resolved bounty should link to the corresponding line in [`LINES.md`](./LINES.md).
