---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '8'
file_basename: War Dog Thanatite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 3
item_id: war-dog-thanatite
item_index: '23'
item_name: War Dog Thanatite
level: 6
might: 1
presence: 1
reason: 2
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-thanatite
scdc:
- 1.1.1:2.51.1:23
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '35'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Thanatite
level: 6
roles:
  - Horde Controller
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "8"
stamina: "35"
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 1
agility: 1
reason: 2
intuition: 3
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Snaking Entrails
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
    usage: Main action
    distance: Ranged 10
    target: One ally
    effects:
      - name: Effect
        effect: The target dies and the thanatite makes one power roll against each
          enemy within 2 squares of the target.
      - roll: Power Roll + 3
        tier1: 3 corruption damage; A < 1 slowed (save ends)
        tier2: 5 corruption damage; A < 2 slowed (save ends)
        tier3: 7 corruption damage; A < 3 restrained (save ends)
      - cost: 3 Malice
        effect: If an affected enemy is adjacent to any corpse, they are frightened of
          the thanatite (save ends).
  - type: feature
    feature_type: ability
    name: Wall of Flesh
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 10 wall within 10
    target: One corpse
    effects:
      - name: Effect
        effect: The target spawns a wall of bloody muscle and pulsing viscera that must
          share one or more squares with the target. Each enemy in the area when
          the wall is created vertically slides up to 2 squares and is knocked
          prone. Each square of the wall has 3 Stamina.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the thanatite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~