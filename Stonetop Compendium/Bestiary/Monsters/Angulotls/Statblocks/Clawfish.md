---
agility: 2
ancestry:
- Angulotl
- Animal
ev: 3 for 4 minions
file_basename: Clawfish
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 2
intuition: -2
item_id: clawfish
item_index: 08
item_name: Clawfish
level: 1
might: 0
presence: 1
reason: -3
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.angulotls.statblock:clawfish
scdc:
- 1.1.1:2.31.1:08
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '5'
type: monster/angulotls/statblock
---

~~~ds-statblock
type: statblock
name: Clawfish
level: 1
roles:
  - Minion Brute
ancestry:
  - Angulotl
  - Animal
ev: 3 for 4 minions
stamina: "5"
immunities:
  - Lightning 3
  - Poison 2
speed: 5
movement: Climb, swim
size: 1S
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: -3
intuition: -2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Hookclaw
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
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage; grabbed
      - name: Effect
        effect: Any target grabbed this way takes 2 lightning damage at the start of
          each of their turns.
  - type: feature
    feature_type: trait
    name: Shocking
    icon: ⭐️
    effects:
      - effect: At the start of each of their turns, the clawfish deals 2 lightning
          damage to each wet enemy within 2 squares.
~~~