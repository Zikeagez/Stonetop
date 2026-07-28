---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: 3 for four minions
file_basename: Wode Elf Lookout
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 1
intuition: 0
item_id: wode-elf-lookout
item_index: 08
item_name: Wode Elf Lookout
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Support
scc:
- mcdm.monsters.v1:monster.elves-wode.statblock:wode-elf-lookout
scdc:
- 1.1.1:2.28.1:08
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster/elves-wode/statblock
---

~~~ds-statblock
type: statblock
name: Wode Elf Lookout
level: 1
roles:
  - Minion Support
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: 3 for four minions
stamina: "4"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Longbow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 8
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
  - type: feature
    feature_type: trait
    name: There!
    icon: ⭐️
    effects:
      - effect: Any wode elf within 5 squares of the lookout can make ranged strikes as
          if occupying the lookout's space.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the lookout that would take a bane from cover or
          concealment have a double bane instead.
~~~