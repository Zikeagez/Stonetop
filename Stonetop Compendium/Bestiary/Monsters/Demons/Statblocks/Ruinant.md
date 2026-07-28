---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '3'
file_basename: Ruinant
file_dpath: Monsters/Demons/Statblocks
free_strike: 1
intuition: 0
item_id: ruinant
item_index: '32'
item_name: Ruinant
level: 1
might: 0
presence: 1
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:ruinant
scdc:
- 1.1.1:2.35.1:32
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '15'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Ruinant
level: 1
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Demon
ev: "3"
stamina: "15"
weaknesses:
  - Holy 3
speed: 6
size: 1M
stability: 0
free_strike: 1
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Bloodletting Claws
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 4 damage
        tier3: 5 damage; M < 2 bleeding (save ends)
  - type: feature
    feature_type: ability
    name: Salt Wounds
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - name: Special
        effect: Each target must be at less than full Stamina.
      - roll: Power Roll + 2
        tier1: 1 corruption damage
        tier2: 2 corruption damage
        tier3: 3 corruption damage
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the ruinant is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the ruinant can't be hidden from them.
~~~