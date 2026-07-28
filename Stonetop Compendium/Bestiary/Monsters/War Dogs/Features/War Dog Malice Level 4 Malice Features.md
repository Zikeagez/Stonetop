---
file_basename: War Dog Malice Level 4 Malice Features
file_dpath: Monsters/War Dogs/Features
include_parens_in_filename: 'true'
item_id: war-dog-malice-level-4-malice-features
item_index: '58'
item_name: War Dog Malice (Level 4+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:war-dog-malice-level-4-malice-features
scdc:
- 1.1.1:2.2:58
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: + Malice Features
name: War Dog Malice
level: 4
flavor: At the start of any level 4 or higher war dog's turn, you can spend
  Malice to activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Prior Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The war dog activates a Malice feature available to war dogs of level 3
          or lower.
  - type: feature
    feature_type: ability
    name: Loyalty Unto Death
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Two war dogs
    effects:
      - name: Effect
        effect: Each target who has a loyalty collar shifts up to their speed, then is
          reduced to 0 Stamina. After each target's Loyalty Collar trait is
          resolved, each enemy adjacent to either target makes a Presence test.
        tier1: Push 4; the enemy is frightened of the nearest non-minion war dog (save
          ends)
        tier2: Push 2; the enemy is frightened of the nearest non-minion war dog (EoT)
        tier3: Push 2
~~~