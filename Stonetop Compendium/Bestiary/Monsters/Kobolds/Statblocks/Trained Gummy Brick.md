---
agility: -1
ancestry:
- Kobold
- Ooze
- Soulless
ev: '12'
file_basename: Trained Gummy Brick
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 4
intuition: 0
item_id: trained-gummy-brick
item_index: '06'
item_name: Trained Gummy Brick
level: 1
might: 2
presence: -2
reason: -3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster.kobolds.statblock:trained-gummy-brick
scdc:
- 1.1.1:2.10.1:06
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '40'
type: monster/kobolds/statblock
---

~~~ds-statblock
type: statblock
name: Trained Gummy Brick
level: 1
roles:
  - Elite Hexer
ancestry:
  - Kobold
  - Ooze
  - Soulless
ev: "12"
stamina: "40"
immunities:
  - Acid 3
speed: 5
size: "2"
stability: 2
free_strike: 4
might: 2
agility: -1
reason: -3
intuition: 0
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Engulf
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 acid damage; A < 0 dazed (save ends)
        tier2: 10 acid damage; A < 1 dazed (save ends)
        tier3: 14 acid damage; A < 2 restrained (save ends)
      - name: Effect
        effect: A size 2 or smaller creature restrained this way is pulled into the
          brick's space, moves with the brick, and takes 4 acid damage at the
          start of each of their turns. An engulfed creature who is no longer
          restrained moves to the nearest unoccupied space adjacent to the
          brick. The brick can have as many creatures or objects engulfed as
          will fit within their space.
      - cost: 2 Malice
        effect: This ability targets one additional target.
  - type: feature
    feature_type: ability
    name: You Didn't Pay Attention!
    icon: ❗️
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: One creature or object
    trigger: A creature moves or is force moved adjacent to the brick.
    effects:
      - name: Effect
        effect: The brick uses Engulf against the triggering creature and has a double
          edge.
  - type: feature
    feature_type: trait
    name: Translucent Brick
    icon: ⭐️
    effects:
      - effect: The brick completely occupies their space, blocking line of effect for
          enemies. The brick is hidden until they act.
~~~