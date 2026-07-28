---
agility: 4
ancestry:
- Undead
ev: 9 for four minions
file_basename: Faded Echo Spirit
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 1
item_id: faded-echo-spirit
item_index: '04'
item_name: Faded Echo Spirit
level: 7
might: -3
presence: -3
reason: -5
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.undead.statblock:faded-echo-spirit
scdc:
- 1.1.1:2.8.1:04
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '10'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Faded Echo Spirit
level: 7
roles:
  - Minion Hexer
ancestry:
  - Undead
ev: 9 for four minions
stamina: "10"
immunities:
  - Corruption 7
  - poison 7
speed: 5
movement: Fly, hover
size: 1M
stability: 1
free_strike: 3
with_captain: Gain an edge on strikes
might: -3
agility: 4
reason: -5
intuition: 1
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Hollow Grasp
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
      - roll: Power Roll + 4
        tier1: 3 corruption damage
        tier2: 6 corruption damage; P < 3 weakened
        tier3: 7 corruption damage; P < 4 weakened
      - name: Effect
        effect: This weakened condition ends if an affected target ends their turn with
          no spirit within 5 squares of them.
  - type: feature
    feature_type: trait
    name: Corruptive Phasing
    icon: ⭐️
    effects:
      - effect: The spirit can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the spirit moves through a creature, that creature
          takes 4 corruption damage. The spirit doesn't take damage from being
          force moved into objects.
~~~