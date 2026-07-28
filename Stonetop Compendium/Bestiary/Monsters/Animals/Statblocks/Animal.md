---
agility: 2
ancestry:
- Animal
ev: '12'
file_basename: Animal
file_dpath: Monsters/Animals/Statblocks
free_strike: 4
intuition: 1
item_id: animal
item_index: '04'
item_name: Animal
level: 1
might: 0
presence: -2
reason: -2
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster.animals.statblock:animal
scdc:
- 1.1.1:2.34.1:04
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '60'
type: monster/animals/statblock
---

~~~ds-statblock
type: statblock
name: Animal
level: 1
roles:
  - Elite Harrier
ancestry:
  - Animal
ev: "12"
stamina: "60"
speed: 6
size: 1M
stability: 0
free_strike: 4
might: 0
agility: 2
reason: -2
intuition: 1
presence: -2
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
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 9 damage
        tier3: 12 damage
      - name: Effect
        effect: The animal shifts up to 2 squares between strikes.
  - type: feature
    feature_type: ability
    name: Rush
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The animal moves up to their speed.
  - type: feature
    feature_type: trait
    name: Nature's Spirit
    icon: ⭐️
    effects:
      - effect: While outdoors or in a natural environment, the animal can negate a bane
          on their abilities or turn a double bane into a bane.
~~~