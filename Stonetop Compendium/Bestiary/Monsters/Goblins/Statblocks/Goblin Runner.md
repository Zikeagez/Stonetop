---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: 3 for four minions
file_basename: Goblin Runner
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: goblin-runner
item_index: 08
item_name: Goblin Runner
level: 1
might: -2
presence: -1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.goblins.statblock:goblin-runner
scdc:
- 1.1.1:2.40.1:08
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Goblin Runner
level: 1
roles:
  - Minion Harrier
ancestry:
  - Goblin
  - Humanoid
ev: 3 for four minions
stamina: "4"
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: -2
agility: 2
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Club Charge
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
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The runner doesn't provoke opportunity attacks by moving.
~~~