---
agility: 2
ancestry:
- Elemental
- High Elf
ev: 3 for four minions
file_basename: Soot Crow
file_dpath: Monsters/Elves High/Statblocks
free_strike: 1
intuition: 0
item_id: soot-crow
item_index: '10'
item_name: Soot Crow
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.elves-high.statblock:soot-crow
scdc:
- 1.1.1:2.14.1:10
size: 1T
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster/elves-high/statblock
---

~~~ds-statblock
type: statblock
name: Soot Crow
level: 1
roles:
  - Minion Harrier
ancestry:
  - Elemental
  - High Elf
ev: 3 for four minions
stamina: "4"
speed: 7
movement: Fly
size: 1T
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Heckle
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage; taunted (EoT)
      - name: Effect
        effect: Until the end of their turn, the soot crow ignores opportunity attacks
          from the target.
~~~