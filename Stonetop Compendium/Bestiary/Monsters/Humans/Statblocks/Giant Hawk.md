---
agility: 2
ancestry:
- Animal
- Human
ev: '6'
file_basename: Giant Hawk
file_dpath: Monsters/Humans/Statblocks
free_strike: 3
intuition: 1
item_id: giant-hawk
item_index: '12'
item_name: Giant Hawk
level: 1
might: 2
presence: -2
reason: -3
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster.humans.statblock:giant-hawk
scdc:
- 1.1.1:2.20.1:12
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Giant Hawk
level: 1
roles:
  - Platoon Mount
ancestry:
  - Animal
  - Human
ev: "6"
stamina: "30"
speed: 5
movement: Fly
size: "2"
stability: 0
free_strike: 3
might: 2
agility: 2
reason: -3
intuition: 1
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Talons
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
        tier1: 5 damage
        tier2: 7 damage
        tier3: 9 damage; grabbed
      - cost: 2 Malice
        effect: If this ability gains an edge or has a double edge, it deals an extra 2
          damage.
  - type: feature
    feature_type: ability
    name: Dive
    icon: 👤
    cost: 1 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The hawk moves up to their speed.
  - type: feature
    feature_type: trait
    name: Mounted Platform
    icon: ⭐️
    effects:
      - effect: Once per turn when the hawk moves, any creature riding the hawk can make
          a free strike during or after the movement.
~~~