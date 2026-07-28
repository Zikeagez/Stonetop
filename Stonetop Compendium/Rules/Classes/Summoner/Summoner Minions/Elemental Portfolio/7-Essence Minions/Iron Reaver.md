~~~ds-statblock
type: statblock
name: Iron Reaver
level: .
roles:
  - Minion Harrier
ancestry:
  - Elemental (Earth, Fire, Void)
ev: 7 essence for three minions
speed: 6
size: 1L
stamina: 10|10|10
movement: Burrow
weaknesses:
stability: R
free_strike: 6
might: 3
agility: 4
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: trait
    name: ⭐ Decentralized Segments
    icon: ⭐️
    effects:
      - effect: The reaver has cover while adjacent to another reaver they were summoned with. Whenever they receive an effect tha tallows them to move or shift outside of their move action, they share the effect with each adjacent reaver they were summoned with.
  - type: feature
    feature_type: trait
    name: ⭐ Bladed Strike
    icon: ⭐️
    effects:
      - effect: The reaver's free strikes inflict `M < WEAK` bleeding (save ends). Each time the reaver inflicts bleeding on a creature, they can shift 2 and make an additional free strike on a new target.
  - type: feature
    feature_type: trait
    name: ⭐ Iron Barricade
    cost: 1 Essence
    icon: ⭐️
    effects:
      - effect: When the reaver is reduced to 0 Stamina, they create a line equal to 2 x their size centered on their space of iron shards on the ground until the end of the encounter. You or any ally has cover and damage immunity 2 while occupying an affected square.
~~~


