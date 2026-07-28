---
agility: -2
ancestry:
- Construct
- Servok
- Soulless
- Valok
ev: '48'
file_basename: Servok War Engine
file_dpath: Monsters/Valok/Statblocks
free_strike: 10
intuition: -1
item_id: servok-war-engine
item_index: '02'
item_name: Servok War Engine
level: 10
might: 5
presence: -5
reason: -4
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.valok.statblock:servok-war-engine
scdc:
- 1.1.1:2.43.1:02
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 8
stamina: '260'
type: monster/valok/statblock
---

~~~ds-statblock
type: statblock
name: Servok War Engine
level: 10
roles:
  - Elite Brute
ancestry:
  - Construct
  - Servok
  - Soulless
  - Valok
ev: "48"
stamina: "260"
speed: 5
size: "3"
stability: 8
free_strike: 10
might: 5
agility: -2
reason: -4
intuition: -1
presence: -5
features:
  - type: feature
    feature_type: ability
    name: Blade Rake
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 15 damage
        tier2: 21 damage; pull 3
        tier3: 25 damage; pull 6
  - type: feature
    feature_type: ability
    name: Prismacore Cannon
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 20
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        tier1: 22 damage
        tier2: 29 damage; I < 4 dazed (save ends)
        tier3: 34 damage; I < 5 dazed (save ends)
      - name: Effect
        effect: This damage can't be reduced in any way. This ability can't be used
          again until the start of the next round.
  - type: feature
    feature_type: ability
    name: Destructive Rollout
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The war engine moves up to their speed in a straight line, automatically
          destroying mundane size 1 objects or walls in their path. The first
          time the war engine moves through a creature's space during this
          movement, that creature can choose to either fall prone or take 10
          damage.
  - type: feature
    feature_type: ability
    name: Burning Oil
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 20 x 1 line within 1
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        tier1: 16 fire damage; the target is burning (save ends)
        tier2: 12 fire damage; the target is burning (EoT)
        tier3: 8 fire damage
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round. Additionally, the area is burning until the end of the
          encounter. While the area is burning, it is difficult terrain and any
          enemy takes 3 fire damage for each square of the area they enter.
  - type: feature
    feature_type: ability
    name: Quick Blast
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Free triggered action
    distance: Ranged 20
    target: One creature or object
    trigger: The target deals damage to the war engine.
    effects:
      - roll: Power Roll + 5
        tier1: 8 damage; push 2
        tier2: 12 damage; push 5
        tier3: 16 damage; push 8
      - name: Effect
        effect: This damage can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Servok Siege Machine
    icon: ⭐️
    effects:
      - effect: The war engine ignores difficult terrain, and their abilities deal an
          extra 15 damage to objects.
  - type: feature
    feature_type: trait
    name: Crafted to Perfection
    icon: ⭐️
    effects:
      - effect: The war engine's shape can't be changed by any external effect.
  - type: feature
    feature_type: trait
    name: Valiar Might
    icon: ⭐️
    effects:
      - effect: While the war engine isn't bleeding, weakened, or winded, any power roll
          made against them is automatically a tier 1 outcome. A critical hit
          still grants its additional main action.
~~~