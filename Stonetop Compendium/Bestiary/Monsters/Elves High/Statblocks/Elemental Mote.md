---
agility: 0
ancestry:
- Elemental
- High Elf
- Soulless
ev: 3 for four minions
file_basename: Elemental Mote
file_dpath: Monsters/Elves High/Statblocks
free_strike: 1
intuition: 0
item_id: elemental-mote
item_index: '03'
item_name: Elemental Mote
level: 1
might: 0
presence: 2
reason: 0
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.elves-high.statblock:elemental-mote
scdc:
- 1.1.1:2.14.1:03
size: 1T
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/elves-high/statblock
---

~~~ds-statblock
type: statblock
name: Elemental Mote
level: 1
roles:
  - Minion Hexer
ancestry:
  - Elemental
  - High Elf
  - Soulless
ev: 3 for four minions
stamina: "3"
speed: 5
movement: Fly
size: 1T
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 0
agility: 0
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Dweomer Plume
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage; R < 1 damage weakness 3 (save ends)
        tier3: 3 damage; R < 2 damage weakness 3 (save ends)
  - type: feature
    feature_type: trait
    name: Spark of Life
    icon: ⭐️
    effects:
      - effect: On their turn, the mote can leave the encounter in a flash of light to
          revive one adjacent dead soot crow, brambleguard, or ceramic horse.
          The revived creature returns with 3 Stamina.
~~~