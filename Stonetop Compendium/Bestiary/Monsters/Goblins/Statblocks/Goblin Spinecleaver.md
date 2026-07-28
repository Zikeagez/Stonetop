---
agility: 0
ancestry:
- Goblin
- Humanoid
ev: 3 for four minions
file_basename: Goblin Spinecleaver
file_dpath: Monsters/Goblins/Statblocks
free_strike: 2
intuition: 0
item_id: goblin-spinecleaver
item_index: '05'
item_name: Goblin Spinecleaver
level: 1
might: 2
presence: -1
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.goblins.statblock:goblin-spinecleaver
scdc:
- 1.1.1:2.40.1:05
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '5'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Goblin Spinecleaver
level: 1
roles:
  - Minion Brute
ancestry:
  - Goblin
  - Humanoid
ev: 3 for four minions
stamina: "5"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 2
agility: 0
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Axe
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
        tier1: 2 damage; push 1
        tier2: 4 damage; push 3
        tier3: 5 damage; push 4
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The spinecleaver doesn't provoke opportunity attacks by moving.
~~~