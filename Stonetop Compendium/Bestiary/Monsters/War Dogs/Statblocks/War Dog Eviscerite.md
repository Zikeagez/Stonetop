---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Eviscerite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 1
intuition: 0
item_id: war-dog-eviscerite
item_index: '04'
item_name: War Dog Eviscerite
level: 1
might: 1
presence: 0
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-eviscerite
scdc:
- 1.1.1:2.51.1:04
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '15'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Eviscerite
level: 1
roles:
  - Horde Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "15"
speed: 7
size: 1M
stability: 0
free_strike: 1
might: 1
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Chainsaw Whip
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 4 damage; pull 1
        tier3: 5 damage; pull 2
      - name: Effect
        effect: The eviscerite can automatically grab a target pulled adjacent to them
          this way.
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
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the eviscerite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~