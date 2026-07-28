---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Crucibite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-crucibite
item_index: '05'
item_name: War Dog Crucibite
level: 1
might: 0
presence: 0
reason: 0
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-crucibite
scdc:
- 1.1.1:2.51.1:05
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Crucibite
level: 1
roles:
  - Horde Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "10"
immunities:
  - Fire 2
speed: 5
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
    name: Flamebelcher
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 5 x 1 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 2 fire damage
        tier2: 4 fire damage
        tier3: 5 fire damage
      - name: Effect
        effect: The area is covered in sticky fire until the start of the crucibite's
          next turn. Any creature who enters the area for the first time in a
          round or starts their turn there takes 2 fire damage.
      - cost: 3 Malice
        effect: The area becomes a 10 x 1 line, and if any ally of the crucibite is in
          the area when it is created, the ability deals an extra 2 damage to
          each target.
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
      - effect: When the crucibite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~