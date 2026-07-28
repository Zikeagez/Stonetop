---
file_basename: Brambles
file_dpath: Dynamic Terrain/Environmental Hazards
item_id: brambles-level-1-hazard-defender
item_index: '03'
item_name: Brambles (Level 1 Hazard Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.environmental-hazard:brambles-level-1-hazard-defender
scdc:
- 1.1.1:4.5:03
source: mcdm.monsters.v1
type: dynamic-terrain/environmental-hazard
---

~~~ds-featureblock
type: featureblock
featureblock_type: Hazard Defender
name: Brambles
level: 1
ev: 1 per 10 x 10 thicket
flavor: This thicket features close-growing vines tipped with sharp thorns.
stamina: 3 per square
size: One or more squares of difficult terrain
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: Each square of brambles must be individually destroyed.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature enters a square of brambles without shifting.
      - name: Effect
        effect: A creature takes 1 damage per square of brambles they enter.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Poisonous Thorns
        cost: +1 EV
        effect: The brambles are poisonous. Any creature who takes damage from brambles
          is also bleeding (save ends).
~~~