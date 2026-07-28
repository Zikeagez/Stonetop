---
agility: -2
ancestry:
- Construct
- Servok
- Soulless
- Valok
ev: '44'
file_basename: Servok Builder
file_dpath: Monsters/Valok/Statblocks
free_strike: 10
intuition: -1
item_id: servok-builder
item_index: '03'
item_name: Servok Builder
level: 9
might: 4
presence: -5
reason: -4
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.valok.statblock:servok-builder
scdc:
- 1.1.1:2.43.1:03
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 8
stamina: '240'
type: monster/valok/statblock
---

~~~ds-statblock
type: statblock
name: Servok Builder
level: 9
roles:
  - Elite Brute
ancestry:
  - Construct
  - Servok
  - Soulless
  - Valok
ev: "44"
stamina: "240"
speed: 5
size: "3"
stability: 8
free_strike: 10
might: 4
agility: -2
reason: -4
intuition: -1
presence: -5
features:
  - type: feature
    feature_type: ability
    name: Wrecking Ball
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 3 cube within 5
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target must make either an Agility test or an **Intuition test**.
        tier1: 15 damage; push 5, prone
        tier2: 12 damage; push 3
        tier3: 8 damage
  - type: feature
    feature_type: ability
    name: Construction Arm
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 16 damage
        tier2: 23 damage; grabbed
        tier3: 28 damage; grabbed; M < 4 vertical push 5
  - type: feature
    feature_type: ability
    name: Lay the Foundation
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
    usage: Main action
    distance: 6 x 3 line within 1
    target: Special
    effects:
      - name: Effect
        effect: The area is covered in wet concrete and is difficult terrain. An enemy
          who starts their turn in the concrete makes a **Might test**.
        tier1: Restrained (EoT)
        tier2: Slowed (EoT)
        tier3: No effect
  - type: feature
    feature_type: ability
    name: Build Wall
    icon: 🔳
    keywords:
      - Area
      - Ranged
    usage: Maneuver
    distance: 6 wall within 3
    target: Special
    effects:
      - name: Effect
        effect: The builder creates a concrete wall. They can also remove any unoccupied
          squares of wet concrete within 3 squares of them, creating two
          additional squares of wall for each square of concrete removed.
  - type: feature
    feature_type: ability
    name: Sputter
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Melee
    usage: Free triggered action
    distance: Melee 3
    target: The triggering creature or object
    trigger: A creature or object within distance deals damage to the builder.
    effects:
      - roll: Power Roll + 4
        tier1: A < 2 restrained (save ends)
        tier2: A < 3 restrained (save ends)
        tier3: A < 4 restrained (save ends)
      - name: Effect
        effect: While a creature is restrained this way, or if the target is an object,
          the target and their space are encased in wet concrete. A creature no
          longer restrained leaves squares of wet concrete behind.
  - type: feature
    feature_type: trait
    name: Servok Siege Machine
    icon: ⭐️
    effects:
      - effect: The builder ignores difficult terrain, and their abilities deal an extra
          15 damage to objects.
  - type: feature
    feature_type: trait
    name: Crafted to Perfection
    icon: ⭐️
    effects:
      - effect: The builder's shape can't be changed by any external effect.
  - type: feature
    feature_type: trait
    name: Valiar Might
    icon: ⭐️
    effects:
      - effect: While the builder isn't bleeding, weakened, or winded, any power roll
          made against them is automatically a tier 1 outcome. A critical hit
          still grants its additional main action.
~~~