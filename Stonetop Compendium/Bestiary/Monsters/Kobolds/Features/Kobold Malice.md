---
file_basename: Kobold Malice
file_dpath: Monsters/Kobolds/Features
item_id: kobold-malice-malice-features
item_index: '11'
item_name: Kobold Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:kobold-malice-malice-features
scdc:
- 1.1.1:2.2:11
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Kobold Malice
flavor: At the start of any kobolds's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Maniple Tactics
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Up to 3 kobolds make a free strike, swaps positions with an adjacent
          kobold, and then that kobold makes a free strike.
  - type: feature
    feature_type: trait
    name: Set the Initiative
    icon: 🌀
    cost: 5 Malice
    effects:
      - effect: Two kobolds take their turns in a row.
  - type: feature
    feature_type: trait
    name: Shield Wall
    icon: ⭐️
    cost: 7 Malice
    effects:
      - effect: Until the end of the round, all kobolds with Shield? Shield! impose an
          additional bane on incoming strikes and abilities.
~~~