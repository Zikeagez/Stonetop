---
agility: 1
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Marauder
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 0
item_id: gnoll-marauder
item_index: '03'
item_name: Gnoll Marauder
level: 2
might: 1
presence: 1
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster.gnolls.statblock:gnoll-marauder
scdc:
- 1.1.1:2.6.1:03
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '20'
type: monster/gnolls/statblock
---

~~~ds-statblock
type: statblock
name: Gnoll Marauder
level: 2
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "20"
speed: 7
size: 1M
stability: 1
free_strike: 2
might: 1
agility: 1
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Fury Flail
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 5 damage
        tier3: 7 damage; prone; A < 2 bleeding (save ends)
      - cost: 2+ Malice
        effect: This ability targets one additional target for each 2 Malice spent.
  - type: feature
    feature_type: ability
    name: Marauder's Cackletongue
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 2 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target shifts up to their speed. If any target hasn't used their
          own Cackletongue maneuver on this turn, they can use it immediately at
          no cost.
  - type: feature
    feature_type: trait
    name: Death Frenzy
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 7 squares of the marauder is reduced
          to 0 Stamina, the marauder moves up to their speed and can make a
          melee free strike.
~~~