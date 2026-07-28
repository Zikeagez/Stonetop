---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '6'
file_basename: Wode Elf Greenskeeper
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wode-elf-greenskeeper
item_index: 09
item_name: Wode Elf Greenskeeper
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster.elves-wode.statblock:wode-elf-greenskeeper
scdc:
- 1.1.1:2.28.1:09
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '40'
type: monster/elves-wode/statblock
---

~~~ds-statblock
type: statblock
name: Wode Elf Greenskeeper
level: 1
roles:
  - Platoon Defender
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "6"
stamina: "40"
speed: 7
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Growing Longsword
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
        tier1: 5 damage
        tier2: 7 damage
        tier3: 9 damage
      - name: Effect
        effect: The target is taunted until the end of their next turn, and the
          greenskeeper shifts up to 3 squares.
      - cost: 2 Malice
        effect: The distance increases to Melee 5.
  - type: feature
    feature_type: ability
    name: Overgrowth
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
    usage: Maneuver
    distance: 3 cube within 10
    target: Special
    effects:
      - name: Effect
        effect: The area is overgrown with heavy brush and brambles until the end of the
          encounter, providing cover and concealment for the greenskeeper and
          their allies. The area is difficult terrain for enemies and any enemy
          who starts their turn in the area takes 3 damage.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the greenskeeper that would take a bane from cover
          or concealment have a double bane instead.
~~~