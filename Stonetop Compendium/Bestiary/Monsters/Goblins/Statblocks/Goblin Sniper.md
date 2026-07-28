---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: 3 for four minions
file_basename: Goblin Sniper
file_dpath: Monsters/Goblins/Statblocks
free_strike: 2
intuition: 0
item_id: goblin-sniper
item_index: '12'
item_name: Goblin Sniper
level: 1
might: -2
presence: -1
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.goblins.statblock:goblin-sniper
scdc:
- 1.1.1:2.40.1:12
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Goblin Sniper
level: 1
roles:
  - Minion Artillery
ancestry:
  - Goblin
  - Humanoid
ev: 3 for four minions
stamina: "3"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: -2
agility: 2
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Bow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
      - name: Effect
        effect: If the sniper doesn't use a move action this turn, this ability gains an
          edge.
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The sniper doesn't provoke opportunity attacks by moving.
~~~