---
agility: 2
ancestry:
- Dwarf
- Humanoid
ev: 3 for 4 minions
file_basename: Dwarf Hunter
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 1
intuition: 0
item_id: dwarf-hunter
item_index: '10'
item_name: Dwarf Hunter
level: 1
might: 1
presence: 0
reason: 0
roles:
- Minion Support
scc:
- mcdm.monsters.v1:monster.dwarves.statblock:dwarf-hunter
scdc:
- 1.1.1:2.52.1:10
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '6'
type: monster/dwarves/statblock
---

~~~ds-statblock
type: statblock
name: Dwarf Hunter
level: 1
roles:
  - Minion Support
ancestry:
  - Dwarf
  - Humanoid
ev: 3 for 4 minions
stamina: "6"
speed: 5
size: 1M
stability: 1
free_strike: 1
with_captain: +2 bonus to Stamina
might: 1
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Snaring Javelin
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage; pull 1
        tier2: 2 damage; pull 2
        tier3: 3 damage; pull 4
      - name: Effect
        effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
~~~