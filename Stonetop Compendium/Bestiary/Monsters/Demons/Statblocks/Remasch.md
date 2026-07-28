---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '4'
file_basename: Remasch
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 0
item_id: remasch
item_index: '26'
item_name: Remasch
level: 2
might: 0
presence: 2
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster.demons.statblock:remasch
scdc:
- 1.1.1:2.35.1:26
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Remasch
level: 2
roles:
  - Horde Ambusher
ancestry:
  - Abyssal
  - Demon
ev: "4"
stamina: "20"
weaknesses:
  - Holy 3
speed: 5
movement: Teleport
size: 1S
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Abyssal Strike
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; the remasch can teleport up to 2 squares
        tier2: 6 damage; the remasch can teleport up to 3 squares
        tier3: 8 damage; the remasch can teleport up to 5 squares
      - cost: 5 Malice
        effect: The remasch takes an adjacent creature with them when they teleport. The
          creature appears in an unoccupied space adjacent to the remasch's
          destination.
  - type: feature
    feature_type: ability
    name: Grasping Shadow
    icon: 👤
    cost: 3 Malice
    keywords:
      - Magic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The remasch can teleport up to 2 squares and uses Abyssal Strike.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the remasch is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the remasch can't be hidden from them.
~~~