---
agility: 0
ancestry:
- Elemental
ev: '28'
file_basename: Field of Growth
file_dpath: Monsters/Elementals/Statblocks
free_strike: 6
intuition: 2
item_id: field-of-growth
item_index: '02'
item_name: Field of Growth
level: 3
might: 2
presence: 2
reason: 0
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster.elementals.statblock:field-of-growth
scdc:
- 1.1.1:2.42.1:02
size: '3'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '120'
type: monster/elementals/statblock
---

~~~ds-statblock
type: statblock
name: Field of Growth
level: 3
roles:
  - Elite Controller
ancestry:
  - Elemental
ev: "28"
stamina: "120"
immunities:
  - Poison 5
speed: 8
movement: Climb
size: "3"
stability: 2
free_strike: 6
might: 2
agility: 0
reason: 0
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Hampering Roots
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 8
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 8 damage
        tier2: 13 damage; R < 1 prone and can't stand (save ends)
        tier3: 16 damage; R < 2 prone and can't stand (save ends)
      - name: Effect
        effect: If a target made prone this way is already prone, they are instead
          restrained (save ends). If the target was also unable to stand, that
          effect ends when they are no longer restrained this way.
  - type: feature
    feature_type: ability
    name: Convocation of Verdure
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - name: Effect
        effect: The target gains 15 temporary Stamina that lasts until the start of the
          field's next turn.
      - cost: 3 Malice
        effect: Until the end of the encounter, the ground within 1 square of the target
          is overgrown with underbrush and vines. Whenever any enemy makes a
          strike against the target while within line of effect of that area,
          the enemy is pulled 5 squares toward the area after the strike is
          resolved. Any enemy who enters the area for the first time in a round
          or starts their turn there is knocked prone.
  - type: feature
    feature_type: ability
    name: Rose Thorn Lash
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Magic
      - Melee
    usage: Triggered action
    distance: Melee 3
    target: The triggering creature or object
    trigger: A creature or object within distance deals damage to the field.
    effects:
      - name: Effect
        effect: The target takes 6 damage, and if they have A < 2, they are bleeding
          (save ends).
  - type: feature
    feature_type: trait
    name: Fickle and Free
    icon: ⭐️
    effects:
      - effect: The field can't be restrained, slowed, or knocked prone, and they ignore
          difficult terrain.
  - type: feature
    feature_type: trait
    name: Roots Run Deep
    icon: ⭐️
    effects:
      - effect: The field can target any creature touching the ground with their
          abilities, even if they don't have line of effect to that creature.
~~~