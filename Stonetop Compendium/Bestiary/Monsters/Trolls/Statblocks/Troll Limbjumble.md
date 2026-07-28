---
agility: 1
ancestry:
- Troll
ev: 7 for four minions
file_basename: Troll Limbjumble
file_dpath: Monsters/Trolls/Statblocks
free_strike: 3
intuition: -1
item_id: troll-limbjumble
item_index: '06'
item_name: Troll Limbjumble
level: 5
might: 3
presence: -1
reason: -2
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.trolls.statblock:troll-limbjumble
scdc:
- 1.1.1:2.53.1:06
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '8'
type: monster/trolls/statblock
---

~~~ds-statblock
type: statblock
name: Troll Limbjumble
level: 5
roles:
  - Minion Hexer
ancestry:
  - Troll
ev: 7 for four minions
stamina: "8"
weaknesses:
  - Acid 8
  - fire
speed: 5
size: 1S
stability: 0
free_strike: 3
with_captain: Gain an edge on strikes
might: 3
agility: 1
reason: -2
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Arm and a Leg
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
      - roll: Power Roll + 3
        tier1: 3 damage; A < 2 prone
        tier2: 5 damage; A < 3 prone
        tier3: 6 damage; prone
      - name: Effect
        effect: If a target made prone this way is already prone, they are grabbed
          instead.
  - type: feature
    feature_type: trait
    name: Hyper-Regeneration
    icon: ⭐️
    effects:
      - effect: At the start of each of the limbjumble's squad's turns, the squad's
          Stamina pool increases as if each limbjumble were at full Stamina.
~~~