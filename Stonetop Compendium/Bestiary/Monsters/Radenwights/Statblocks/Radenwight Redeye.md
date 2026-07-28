---
agility: 2
ancestry:
- Humanoid
- Radenwight
ev: 3 for 4 minions
file_basename: Radenwight Redeye
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 2
intuition: 0
item_id: radenwight-redeye
item_index: '07'
item_name: Radenwight Redeye
level: 1
might: 1
presence: 0
reason: -1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.radenwights.statblock:radenwight-redeye
scdc:
- 1.1.1:2.19.1:07
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster/radenwights/statblock
---

~~~ds-statblock
type: statblock
name: Radenwight Redeye
level: 1
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Radenwight
ev: 3 for 4 minions
stamina: "3"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 1
agility: 2
reason: -1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Eyes-On-Me-Shot
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
        effect: One ally of the redeye within 2 squares of the target shifts up to 2
          squares.
  - type: feature
    feature_type: ability
    name: Ready Rodent
    icon: ❗️
    keywords:
      - Melee
      - Weapon
    usage: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - name: Effect
        effect: The redeye makes a free strike against the target.
~~~