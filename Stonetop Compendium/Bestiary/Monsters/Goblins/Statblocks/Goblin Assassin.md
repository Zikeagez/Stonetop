---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Assassin
file_dpath: Monsters/Goblins/Statblocks
free_strike: 2
intuition: 0
item_id: goblin-assassin
item_index: '04'
item_name: Goblin Assassin
level: 1
might: -2
presence: -2
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster.goblins.statblock:goblin-assassin
scdc:
- 1.1.1:2.40.1:04
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '15'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Goblin Assassin
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Goblin
  - Humanoid
ev: "3"
stamina: "15"
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 2
might: -2
agility: 2
reason: 0
intuition: 0
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Sword Stab
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 6 damage
        tier3: 7 damage
      - name: Effect
        effect: If this ability gains an edge or has a double edge, it deals an extra 2
          damage.
  - type: feature
    feature_type: ability
    name: Shadow Chains
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: Three creatures
    effects:
      - roll: Power Roll + 2
        tier1: 2 corruption damage; A < 0 restrained (save ends)
        tier2: 4 corruption damage; A < 1 restrained (save ends)
        tier3: 5 corruption damage; A < 2 restrained (save ends)
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The assassin doesn't provoke opportunity attacks by moving.
  - type: feature
    feature_type: trait
    name: Slip Away
    icon: ⭐️
    effects:
      - effect: The assassin can attempt to hide even while observed.
~~~