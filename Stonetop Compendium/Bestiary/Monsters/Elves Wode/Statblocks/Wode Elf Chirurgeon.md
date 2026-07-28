---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '8'
file_basename: Wode Elf Chirurgeon
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 4
intuition: 0
item_id: wode-elf-chirurgeon
item_index: '13'
item_name: Wode Elf Chirurgeon
level: 2
might: 1
presence: 1
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster.elves-wode.statblock:wode-elf-chirurgeon
scdc:
- 1.1.1:2.28.1:13
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '40'
type: monster/elves-wode/statblock
---

~~~ds-statblock
type: statblock
name: Wode Elf Chirurgeon
level: 2
roles:
  - Platoon Harrier
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "8"
stamina: "40"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 4
might: 1
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Wild Ax
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage; push 1
        tier2: 9 damage; push 3
        tier3: 12 damage; push 5
      - name: Effect
        effect: The chirurgeon can make a ranged free strike before using this ability.
      - cost: 5 Malice
        effect: The chirurgeon uses this ability again.
  - type: feature
    feature_type: ability
    name: The Wode Protects Us
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Self and three allies
    effects:
      - name: Effect
        effect: Each target can teleport up to 10 squares to a space that has cover or
          concealment.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the chirurgeon that would take a bane from cover or
          concealment have a double bane instead.
~~~