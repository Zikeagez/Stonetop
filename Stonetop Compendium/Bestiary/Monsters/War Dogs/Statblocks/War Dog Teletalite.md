---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Teletalite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-teletalite
item_index: '28'
item_name: War Dog Teletalite
level: 1
might: 0
presence: 0
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-teletalite
scdc:
- 1.1.1:2.51.1:28
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Teletalite
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "15"
speed: 5
movement: Teleport
size: 1M
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Corrupted Ash Daggers
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage; slide 1
        tier2: 6 damage; slide 2
        tier3: 7 damage; slide 3
      - name: Effect
        effect: The teletalite gains an edge on this ability if any ally is adjacent to
          the target.
      - cost: 1 Malice
        effect: The teletalite teleports the target 3 squares before sliding them.
  - type: feature
    feature_type: ability
    name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - name: Effect
        effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
  - type: feature
    feature_type: ability
    name: Corrupted Ash Teleport
    icon: 👤
    cost: 1 Malice
    keywords:
      - Magic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The teletalite can teleport up to 5 squares and gains an edge on strikes
          until the end of their turn.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the teletalite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~