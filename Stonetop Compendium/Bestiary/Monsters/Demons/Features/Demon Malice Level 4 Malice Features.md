---
file_basename: Demon Malice Level 4 Malice Features
file_dpath: Monsters/Demons/Features
include_parens_in_filename: 'true'
item_id: demon-malice-level-4-malice-features
item_index: '37'
item_name: Demon Malice (Level 4+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:demon-malice-level-4-malice-features
scdc:
- 1.1.1:2.2:37
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: + Malice Features
name: Demon Malice
level: 4
flavor: At the start of any level 4 or higher demon's turn, you can spend Malice
  to activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Prior Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The demon activates a Malice feature available to demons of level or
          lower.
  - type: feature
    feature_type: trait
    name: Abyssal Jaunt
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: One demon acting this turn folds space around them, temporarily slipping
          in and out of the Abyssal Wasteland. Until the start of the demon's
          next turn, they ignore difficult terrain, can move through solid
          matter, and don't provoke opportunity attacks by moving. If the demon
          ends their turn inside solid matter, they are shunted out into the
          space from which they entered it.
~~~