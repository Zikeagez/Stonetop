---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '6'
file_basename: Fangling
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: 0
item_id: fangling
item_index: 09
item_name: Fangling
level: 4
might: 3
presence: 0
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:fangling
scdc:
- 1.1.1:2.35.1:09
size: 1L
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '30'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Fangling
level: 4
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Demon
ev: "6"
stamina: "30"
weaknesses:
  - Holy 5
speed: 8
size: 1L
stability: 0
free_strike: 2
might: 3
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Tooth! Tusk! Claw!
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
      - roll: Power Roll + 3
        tier1: 5 damage
        tier2: 7 damage
        tier3: 9 damage
      - name: Effect
        effect: Each enemy adjacent to the fangling takes 2 damage.
  - type: feature
    feature_type: ability
    name: Tumbling Gore
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    usage: Maneuver
    distance: 8 x 3 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage; pull 1; A < 1 bleeding (save ends)
        tier2: 3 damage; pull 1; A < 2 bleeding (save ends)
        tier3: 4 damage; pull 1; A < 3 bleeding (save ends)
  - type: feature
    feature_type: trait
    name: Made of Teeth
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the fangling or uses a melee ability
          against the fangling, they take 2 damage.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the fangling is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the fangling can't be hidden from them.
~~~