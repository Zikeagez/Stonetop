---
file_basename: Valok Malice
file_dpath: Monsters/Valok/Features
item_id: valok-malice-malice-features
item_index: '46'
item_name: Valok Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:valok-malice-malice-features
scdc:
- 1.1.1:2.2:46
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Valok Malice
flavor: At the start of any valok's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Repeater
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: One valok acting this turn takes an additional main action.
  - type: feature
    feature_type: trait
    name: I Was Not Commanded to Wait
    icon: 🌀
    cost: 5 Malice
    effects:
      - effect: At the end of each turn until the end of the round, one valok can either
          shift up to 2 squares or make a free strike.
  - type: feature
    feature_type: trait
    name: Rapid Logic Overdrive
    icon: ⭐️
    cost: 7 Malice
    effects:
      - effect: Each valok in the encounter can end one effect on them that can be ended
          by a saving throw, and can move up to their speed (making use of the
          bonus below). Additionally, until the end of the encounter, all valok
          deal an extra 5 damage on strikes and gain a +5 bonus to speed. This
          feature can be activated multiples times, stacking the effects.
~~~