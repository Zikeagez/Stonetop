---
file_basename: Tree of Might
file_dpath: Dynamic Terrain/Power Fixtures
item_id: tree-of-might-level-5-hazard-hexer
item_index: '03'
item_name: Tree of Might (Level 5 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.power-fixture:tree-of-might-level-5-hazard-hexer
scdc:
- 1.1.1:4.4:03
source: mcdm.monsters.v1
type: dynamic-terrain/power-fixture
---

~~~ds-featureblock
type: featureblock
featureblock_type: Hazard Hexer
name: Tree of Might
level: 5
ev: "14"
flavor: A gnarled tree has unearthed roots that writhe and curl.
stamina: "60"
size: "3"
stats:
  - name: Immunity
    value: 5 to all damage except corruption or fire damage
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: The tree of might must be completely destroyed.
  - type: feature
    feature_type: trait
    name: Tree's Nourishment
    icon: ⭐️
    effects:
      - effect: At the start of each round while the tree of might is intact, each enemy
          touching the ground in the encounter area who has M < 0 takes 10
          corruption damage, and the tree of might grows a fruit. The potency
          increases by 1 each subsequent round.
  - type: feature
    feature_type: trait
    name: Mighty Fruit
    icon: ⭐️
    effects:
      - effect: Once per round, any creature adjacent to the tree of might can take a
          fruit from the tree and eat it (no action required). The creature
          gains 10 temporary Stamina and has their Might score increased by 1
          (to a maximum of 6) until the end of the encounter.
~~~