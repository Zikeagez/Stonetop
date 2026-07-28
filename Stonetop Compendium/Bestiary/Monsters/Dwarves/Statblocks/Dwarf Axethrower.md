---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: 3 for 4 minions
file_basename: Dwarf Axethrower
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 1
intuition: 2
item_id: dwarf-axethrower
item_index: 08
item_name: Dwarf Axethrower
level: 1
might: 1
presence: 0
reason: 0
roles:
- Minion Defender
scc:
- mcdm.monsters.v1:monster.dwarves.statblock:dwarf-axethrower
scdc:
- 1.1.1:2.52.1:08
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '7'
type: monster/dwarves/statblock
---

~~~ds-statblock
type: statblock
name: Dwarf Axethrower
level: 1
roles:
  - Minion Defender
ancestry:
  - Dwarf
  - Humanoid
ev: 3 for 4 minions
stamina: "7"
speed: 5
size: 1M
stability: 2
free_strike: 1
with_captain: +2 bonus to Stamina
might: 1
agility: 0
reason: 0
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Whistling Axes
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage; one ally adjacent to the target can make a free strike
      - name: Effect
        effect: The target can't use triggered actions until the start of the next
          round.
~~~