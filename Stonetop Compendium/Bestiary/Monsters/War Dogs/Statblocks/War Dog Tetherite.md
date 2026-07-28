---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 3 for four minions
file_basename: War Dog Tetherite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-tetherite
item_index: '36'
item_name: War Dog Tetherite
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-tetherite
scdc:
- 1.1.1:2.51.1:36
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '5'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Tetherite
level: 1
roles:
  - Minion Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 3 for four minions
stamina: "5"
speed: 5
size: 1M
stability: 1
free_strike: 2
with_captain: Gain an edge on strikes
might: 2
agility: 0
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Banded Dagger
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
  - type: feature
    feature_type: trait
    name: Tethered
    icon: ⭐️
    effects:
      - effect: A captain attached to a tetherite squad has their stability increased by
          the number of tetherites within 2 squares of them.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the tetherite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d3 damage to each adjacent enemy and object.
~~~