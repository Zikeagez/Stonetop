~~~ds-statblock
type: statblock
name: Quite of Snow
level: .
roles:
  - Minion Artillery
ancestry:
  - Elemental (Air, Rot, Water)
ev: 3 essence for three minions
speed: 5
size: 1L
stamina: 4|4|4
movement: Fly, hover
immunities:
  - Sonic R
  - cold R
stability: 1
free_strike: 4
might: -1
agility: 2
reason: 0
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: 🏹 Freezing Howl 2d10 + R
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Ranged
      - Strike
    distance: Ranged 5
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 4 cold damage; `M < WEAK` slowed (EoT)
        tier2: 6 cold damage; `M < AVERAGE` slowed (EoT)
        tier3: 8 cold damage; `M < STRONG` speed is 0 (EoT)
        effect: Frost slows the enemy down, allowing one ally adjacent to each target to shift 2 and either hide or defend.
  - type: feature
    feature_type: trait
    name: ⭐ Cold Surge
    icon: ⭐️
    effects:
      - effect: When the quiet is reduced to 0 Stamina, they launch a refreshing blast of air into an area equal to their size + 1 within 5 before being destroyed. Each ally in the affected area gains a surge.


~~~


