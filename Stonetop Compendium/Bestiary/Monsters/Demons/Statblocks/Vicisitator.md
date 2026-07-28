---
agility: 5
ancestry:
- Abyssal
- Demon
ev: '12'
file_basename: Vicisitator
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: -2
item_id: vicisitator
item_index: '11'
item_name: Vicisitator
level: 10
might: 4
presence: -3
reason: -1
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:vicisitator
scdc:
- 1.1.1:2.35.1:11
size: 1M
source: mcdm.monsters.v1
speed: 9
stability: 0
stamina: '60'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Vicisitator
level: 10
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Demon
ev: "12"
stamina: "60"
weaknesses:
  - Holy 5
speed: 9
size: 1M
stability: 0
free_strike: 4
might: 4
agility: 5
reason: -1
intuition: -2
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Warp Touch
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        tier1: 9 damage
        tier2: 12 damage
        tier3: 14 damage; I < 5 the target is slowed and weakened (save ends)
      - name: Special
        effect: The effects of being slowed and weakened this way can't be ignored.
  - type: feature
    feature_type: ability
    name: Soul Flay
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 6 x 3 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: 4 psychic damage; P < 3 bleeding (save ends)
        tier2: 7 psychic damage; P < 4 bleeding (save ends)
        tier3: 9 psychic damage; P < 5 bleeding (save ends)
      - name: Effect
        effect: Any creature who is bleeding from this ability loses 2d6 Stamina instead
          of 1d6.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the vicisitator is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the vicisitator can't be hidden from
          them.
~~~