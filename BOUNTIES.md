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
  - 3 any colour bounce, 1 red bounce
  - Oran Rief the vastwood (additional card 2 - not in the alternative B line)
  - Kavaron, Memorial World (additional card 3)
- Alternative A:
  - A third deeps instead of the Oran Rief
- Alternative B: 
  - Neither deeps 3 nor Oran Rief needed 

#### Line

1. Cast titan get Mirropool+ Bounce (1 titan)
2. Float Cxxxx, bounce the bounce, activate mirrorpool to copy titan (2 titans)
3. Get Echoing Deeps+ bounce
4. Copy mirrorpool, Float Cxxxx, bounce the bounce, activate mirrorpool to copy titan (3 titans)
5. Get Echoing Deeps+ bounce
6. Copy mirrorpool, Float Cxxxx, bounce the bounce, activate mirrorpool to copy titan (4 titans)
7. Get Kavaron, Memorial World+ Crumbling Vestige
8. Float RRx, leaving Vestige untapped. Station Kavaron with 2 titans (12), then activate Kavaron, sacrificing itself to give the remaining 2 haste, +1/+0 and create a 3/2 haste
9. Attack, get 2 titan triggers
10. First one get Oran Rief (2 untaps) and anything, tap Oran Rief twice
11. Titans are now both 9/8, the token is a 3/2, for 21 damage

#### Alternative A

The same up to 9, then the standard titan + 2 amulet line after attacks, which needs the third deeps, but not the Oran Rief.

#### Alternative B [credit to Epreez for the initial idea, adapted to work correctly]

The same up to 9.
10. Get Otawara and The Mycosynth Gardens (one untap each), activate Gardens with Otawara to copy amulet
11. Get Urza's Cave and SGC, float 4 mana from SGC, return Otawara. Bounce the nontoken titan to hand with Otawara, leaving SGC, Cave and the Vestige untapped
12. 2nd main, crack cave using SGC and the untapped land from pre-combat. Grab a bounceland, floating 6 mana and casting a titan.
13. Get Twest + bounce, floating 9 mana, returning tolaria west with the bounce trigger. Transmute for pact, pact for analyst.
14. Cast and crack analyst, returning mirrorpool, tolaria west, a bounceland, urza's cave, and 2 echoing deeps each copying urza's cave.
15. Float 2+3+6+1 mana leaving mirrorpool and 2 caves untapped, bouncing tolaria west. Activate mirrorpool to copy titan (7 mana)
16. Get 2 crumbling vestige floating 8 mana = 15 mana floating
17. Crack 2 caves, one for shifting woodlands and 1 for urza's saga (1 untap each) floating 2 mana = (15-6+2 = 11 mana). Transmute tolaria west for zuran orb and cast it: 8 mana
18. sac all your lands (including saga to get delirium), activate shifting woodlands for 4+4 = 8 to loop.

#### Result

Attack for 21

Alternative A/B: win with analyst loop (technically next turn, but after bouncing all their permanents and destroying all their lands)

#### Notes

Lands that don't have 'enter tapped' on them marked as only untapping once.

Alternative B is only +2 cards (Kavaron and another deeps)

## Resolved Bounties

Move solved bounties here once a valid line has been found and checked.

Each resolved bounty should link to the corresponding line in [`LINES.md`](./LINES.md).
