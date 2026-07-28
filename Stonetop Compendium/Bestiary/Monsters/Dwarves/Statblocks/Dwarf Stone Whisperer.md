---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: '10'
file_basename: Dwarf Stone Whisperer
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 5
intuition: 2
item_id: dwarf-stone-whisperer
item_index: '07'
item_name: Dwarf Stone Whisperer
level: 3
might: 1
presence: 0
reason: 2
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster.dwarves.statblock:dwarf-stone-whisperer
scdc:
- 1.1.1:2.52.1:07
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '52'
type: monster/dwarves/statblock
---

~~~ds-statblock
type: statblock
name: Dwarf Stone Whisperer
level: 3
roles:
  - Platoon Controller
ancestry:
  - Dwarf
  - Humanoid
ev: "10"
stamina: "52"
speed: 5
movement: Burrow
size: 1M
stability: 2
free_strike: 5
might: 1
agility: 0
reason: 2
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Tile Slide
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 2 cube within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; slide 1; M < 0 slowed (save ends)
        tier2: 8 damage; slide 3; M < 1 slowed (save ends)
        tier3: 11 damage; slide 5; M < 2 restrained (save ends)
      - name: Effect
        effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
  - type: feature
    feature_type: ability
    name: Stone Wave
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage; push 2; R < 1 slowed (save ends)
        tier2: 6 damage; push 3; R < 2 slowed (save ends)
        tier3: 9 damage; push 3; R < 3 slowed (save ends)
      - name: Effect
        effect: The area is difficult terrain for enemies. A target restrained by a
          dwarf can be force moved by this ability. This forced movement doesn't
          end the restrained condition unless the Director determines otherwise.
  - type: feature
    feature_type: trait
    name: Stone Walker
    icon: ⭐️
    effects:
      - effect: Whenever the stone whisperer willingly moves, they can phase through up
          to 2 squares of stone as part of that movement. If they end their
          movement inside stone, they are shunted out into the space from which
          they entered it.
~~~