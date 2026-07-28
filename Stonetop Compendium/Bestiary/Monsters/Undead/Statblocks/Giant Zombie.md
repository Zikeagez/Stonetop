---
agility: -1
ancestry:
- Undead
- Soulless
ev: '24'
file_basename: Giant Zombie
file_dpath: Monsters/Undead/Statblocks
free_strike: 6
intuition: 1
item_id: giant-zombie
item_index: '15'
item_name: Giant Zombie
level: 4
might: 3
presence: 2
reason: -2
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.undead.statblock:giant-zombie
scdc:
- 1.1.1:2.8.1:15
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '140'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Giant Zombie
level: 4
roles:
  - Elite Brute
ancestry:
  - Undead
  - Soulless
ev: "24"
stamina: "140"
immunities:
  - Corruption 4
  - poison 4
speed: 6
size: "3"
stability: 2
free_strike: 6
might: 3
agility: -1
reason: -2
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Rotten Smash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 14 damage; A < 2 grabbed
        tier3: 17 damage; A < 3 grabbed
  - type: feature
    feature_type: ability
    name: Knocking Heads
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self; see below
    trigger: The giant zombie grabs two creatures or objects, or starts their turn
      with two creatures or objects grabbed.
    effects:
      - name: Effect
        effect: The creatures or objects are smashed together using Rotten Smash, which
          has a double edge.
  - type: feature
    feature_type: trait
    name: Endless Knight
    icon: ⭐️
    effects:
      - effect: The first time the giant zombie is reduced to 0 Stamina by damage that
          isn't fire damage or holy damage and their body isn't destroyed, they
          instead have 50 Stamina and fall prone.
  - type: feature
    feature_type: trait
    name: Negative Nerves
    icon: ⭐️
    effects:
      - effect: When the giant zombie is targeted by an ability that deals rolled
          damage, they halve the damage from a tier 1 outcome.
~~~