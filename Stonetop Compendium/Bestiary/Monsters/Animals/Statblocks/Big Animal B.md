---
agility: 1
ancestry:
- Animal
ev: '16'
file_basename: Big Animal B
file_dpath: Monsters/Animals/Statblocks
free_strike: 5
intuition: 1
item_id: big-animal-b
item_index: '06'
item_name: Big Animal B
level: 2
might: 2
presence: 0
reason: -1
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster.animals.statblock:big-animal-b
scdc:
- 1.1.1:2.34.1:06
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '80'
type: monster/animals/statblock
---

~~~ds-statblock
type: statblock
name: Big Animal B
level: 2
roles:
  - Elite Mount
ancestry:
  - Animal
ev: "16"
stamina: "80"
speed: 6
size: "3"
stability: 3
free_strike: 5
might: 2
agility: 1
reason: -1
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Natural Weapon
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 10 damage; push 1
        tier3: 13 damage; push 2
  - type: feature
    feature_type: ability
    name: Trundle
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The animal moves up to their speed. They can make a free strike against
          each creature who makes an opportunity attack against them during this
          movement.
  - type: feature
    feature_type: ability
    name: Animal Rally
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Ranged 20
    target: One ally
    trigger: The target is knocked prone.
    effects:
      - name: Effect
        effect: The animal moves up to their speed. If they end their turn adjacent to
          the target, they can use the Stand Up maneuver to let the target
          stand, then get on to ride them.
  - type: feature
    feature_type: trait
    name: Beast of Burden
    icon: ⭐️
    effects:
      - effect: While riding the animal, two size 1 allies can occupy the same space.
  - type: feature
    feature_type: trait
    name: Nature's Spirit
    icon: ⭐️
    effects:
      - effect: While outdoors or in a natural environment, the animal can negate a bane
          on their abilities or turn a double bane into a bane.
~~~