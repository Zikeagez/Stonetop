---
file_basename: Holy Idol
file_dpath: Dynamic Terrain/Power Fixtures
item_id: holy-idol-level-5-relic-support
item_index: '02'
item_name: Holy Idol (Level 5 Relic Support)
scc:
- mcdm.monsters.v1:dynamic-terrain.power-fixture:holy-idol-level-5-relic-support
scdc:
- 1.1.1:4.4:02
source: mcdm.monsters.v1
type: dynamic-terrain/power-fixture
---

~~~ds-featureblock
type: featureblock
featureblock_type: Relic Support
name: Holy Idol
level: 5
ev: "7"
flavor: An empowering monument to a higher power enables a villain's machinations.
stamina: "35"
size: "2"
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: The holy idol must be completely destroyed.
  - type: feature
    feature_type: trait
    name: Empowered Will
    icon: ⭐️
    effects:
      - effect: At the start of each round while the holy idol is intact, the Director
          gains a d6 that lasts until the end of the round. When a
          Director-controlled creature deals or takes damage, the Director can
          roll the d6 to increase the damage the creature deals or reduce the
          damage the creature takes by an amount equal to the roll (to a minimum
          of 2 damage). If multiple idols are in play, only one d6 can be
          applied to a single instance of damage.
~~~