---
agility: 1
ancestry:
- Dwarf
- Humanoid
ev: 3 for 4 minions
file_basename: Dwarf Driver
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 1
intuition: 0
item_id: dwarf-driver
item_index: '02'
item_name: Dwarf Driver
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.dwarves.statblock:dwarf-driver
scdc:
- 1.1.1:2.52.1:02
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '6'
type: monster/dwarves/statblock
---

~~~ds-statblock
type: statblock
name: Dwarf Driver
level: 1
roles:
  - Minion Harrier
ancestry:
  - Dwarf
  - Humanoid
ev: 3 for 4 minions
stamina: "6"
speed: 7
size: 1M
stability: 1
free_strike: 1
with_captain: +2 bonus to Stamina
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Handaxes
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
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage; push 1
        tier2: 2 damage; push 2
        tier3: 3 damage; push 4
      - name: Effect
        effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
~~~