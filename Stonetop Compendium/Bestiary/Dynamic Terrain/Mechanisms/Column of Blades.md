---
file_basename: Column of Blades
file_dpath: Dynamic Terrain/Mechanisms
item_id: column-of-blades-level-3-fortification-defender
item_index: '04'
item_name: Column of Blades (Level 3 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:column-of-blades-level-3-fortification-defender
scdc:
- 1.1.1:4.1:04
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Defender
name: Column of Blades
level: 3
ev: "3"
flavor: A spinning wooden column is affixed with sharp blades to slash the unwary.
stamina: "5"
size: 1L
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: The column of blades must be completely destroyed.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature or object moves adjacent to the column of blades.
      - name: Effect
        effect: The **Spinning Blades** ability.
  - type: feature
    feature_type: ability
    name: Spinning Blades
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object moves within distance of the column.
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 6 damage; M < 2 bleeding (save ends)
        tier3: 9 damage; M < 3 bleeding (save ends)
  - type: feature
    feature_type: trait
    name: Upgrades
    icon: ⭐️
    effects:
      - name: Stone Column
        cost: +1 EV
        effect: The column is made of stone and has 8 Stamina.
      - name: Metal Column
        cost: +1 EV
        effect: The column is made of metal and has 11 Stamina.
      - name: Concealed
        cost: +1 EV
        effect: The blades are concealed inside the column, which remains motionless
          until triggered.
      - name: Spiked Flails
        cost: +4 EV
        effect: Instead of blades, the column is affixed with heavy spiked balls
          attached by long chains. The **Whirling Flails** ability replaces
          **Spinning Blades**.
  - type: feature
    feature_type: ability
    name: Whirling Flails
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Free triggered action
    distance: Melee 2
    target: The triggering creature or object
    trigger: A creature or object moves within distance of the column.
    effects:
      - tier1: 5 damage
        tier2: 8 damage; M < 2 dazed (save ends)
        tier3: 11 damage; M < 3 dazed (save ends)
  - type: feature
    feature_type: trait
    name: Allied Awareness
    icon: ⭐️
    effects:
      - effect: Allies who shift don't trigger the column. A creature observing an ally
          shift this way can make an **Intuition test** to shift in imitation of
          their movements.
      - roll: Power Roll + 2
        tier1: The creature triggers the column and the column's ability gains an edge.
        tier2: The creature triggers the column.
        tier3: The creature doesn't trigger the column.
~~~