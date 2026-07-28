---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Warrior
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: goblin-warrior
item_index: '01'
item_name: Goblin Warrior
level: 1
might: -2
presence: -1
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster.goblins.statblock:goblin-warrior
scdc:
- 1.1.1:2.40.1:01
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '15'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Goblin Warrior
level: 1
roles:
  - Horde Harrier
ancestry:
  - Goblin
  - Humanoid
ev: "3"
stamina: "15"
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 1
might: -2
agility: 2
reason: 0
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Spear Charge
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 4 damage
        tier3: 5 damage
  - type: feature
    feature_type: ability
    name: Bury the Point
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; M < 0 bleeding (save ends)
        tier2: 6 damage; M < 1 bleeding (save ends)
        tier3: 7 damage; M < 2 bleeding (save ends)
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The warrior doesn't provoke opportunity attacks by moving.
~~~