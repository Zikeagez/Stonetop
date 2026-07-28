---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: 3 for 4 minions
file_basename: Dwarf Catchpole
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 2
intuition: 0
item_id: dwarf-catchpole
item_index: '05'
item_name: Dwarf Catchpole
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.dwarves.statblock:dwarf-catchpole
scdc:
- 1.1.1:2.52.1:05
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '7'
type: monster/dwarves/statblock
---

~~~ds-statblock
type: statblock
name: Dwarf Catchpole
level: 1
roles:
  - Minion Brute
ancestry:
  - Dwarf
  - Humanoid
ev: 3 for 4 minions
stamina: "7"
speed: 5
size: 1M
stability: 2
free_strike: 2
with_captain: +2 bonus to Stamina
might: 2
agility: 0
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Maul
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage; grabbed or prone
      - name: Effect
        effect: If the target is restrained, they take an extra 2 damage.
~~~