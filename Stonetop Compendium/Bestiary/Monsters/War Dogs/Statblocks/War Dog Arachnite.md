---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '8'
file_basename: War Dog Arachnite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 2
item_id: war-dog-arachnite
item_index: '32'
item_name: War Dog Arachnite
level: 6
might: 0
presence: 1
reason: 2
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-arachnite
scdc:
- 1.1.1:2.51.1:32
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '35'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Arachnite
level: 6
roles:
  - Horde Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "8"
stamina: "35"
immunities:
  - Psychic 6
speed: 5
movement: Climb
size: 1L
stability: 0
free_strike: 4
might: 0
agility: 3
reason: 2
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Longarm Shrikegun
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage
        tier2: 9 damage
        tier3: 11 damage; A < 3 bleeding (save ends)
      - name: Effect
        effect: "This ability ignores cover and concealment. The arachnite chooses one
          of the following damage types when making the strike: acid, cold,
          fire, lightning, poison, psychic, or sonic."
      - cost: 2 Malice
        effect: The arachnite can use this ability as if they were in the space of any
          ally within distance.
  - type: feature
    feature_type: ability
    name: Web Vial
    icon: 🔳
    keywords:
      - Area
      - Ranged
    usage: Maneuver
    distance: 2 cube within 10
    target: Special
    effects:
      - name: Effect
        effect: The area is difficult terrain until the end of the encounter.
  - type: feature
    feature_type: trait
    name: Eight-Eyed Sight
    icon: ⭐️
    effects:
      - effect: At the start of each of their turns, the arachnite automatically knows
          the location of each hidden creature within 10 squares of them.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the arachnite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~