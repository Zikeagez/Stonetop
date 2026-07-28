---
agility: 1
ancestry:
- Animal
- Swarm
ev: '12'
file_basename: Animal Swarm
file_dpath: Monsters/Animals/Statblocks
free_strike: 4
intuition: 2
item_id: animal-swarm
item_index: '03'
item_name: Animal Swarm
level: 1
might: -2
presence: -3
reason: -3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster.animals.statblock:animal-swarm
scdc:
- 1.1.1:2.34.1:03
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '40'
type: monster/animals/statblock
---

~~~ds-statblock
type: statblock
name: Animal Swarm
level: 1
roles:
  - Elite Hexer
ancestry:
  - Animal
  - Swarm
ev: "12"
stamina: "40"
speed: 5
size: "2"
stability: 1
free_strike: 4
might: -2
agility: 1
reason: -3
intuition: 2
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Flurry
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 9 damage; pull 1
        tier3: 12 damage; pull 2
      - name: Effect
        effect: If the target is pulled into the animal swarm, that forced movement
          deals damage only at the Director's determination.
  - type: feature
    feature_type: trait
    name: Swarm
    icon: ⭐️
    effects:
      - effect: The animal swarm can move through spaces as if they were a size 1M
          creature, and can occupy other creatures' spaces. At the start of each
          of the animal swarm's turns, they can make a free strike against each
          creature whose space they share.
  - type: feature
    feature_type: ability
    name: Impede
    icon: ❇️
    keywords:
      - Area
    usage: Maneuver
    distance: 1 aura
    target: Special
    effects:
      - name: Effect
        effect: The area is difficult terrain for enemies until the start of the animal
          swarm's next turn.
  - type: feature
    feature_type: trait
    name: Nature's Spirit
    icon: ⭐️
    effects:
      - effect: While outdoors or in a natural environment, the animal swarm can negate
          a bane on their abilities or turn a double bane into a bane.
~~~