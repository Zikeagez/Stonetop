---
file_basename: Voiceless Talker Malice
file_dpath: Monsters/Voiceless Talkers/Features
item_id: voiceless-talker-malice-malice-features
item_index: '49'
item_name: Voiceless Talker Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:voiceless-talker-malice-malice-features
scdc:
- 1.1.1:2.2:49
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Voiceless Talker Malice
flavor: At the start of any voiceless talker's turn, you can spend Malice to
  activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Guise
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: One non-minion voiceless talker projects a psionic screen over their
          body, preventing other creatures from treating them as an enemy until
          the end of the voiceless talker's next turn.
  - type: feature
    feature_type: ability
    name: Memory Thief
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Psionic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 6 psychic damage; R < 1 the target can't treat their allies as allies
          (save ends)
        tier2: 10 psychic damage; R < 2 the target perceives their allies as enemies
          (save ends)
        tier3: 13 psychic damage; R < 3 the target perceives their allies as enemies
          (save ends)
      - name: Special
        effect: This ability can't be used by a minion.
  - type: feature
    feature_type: trait
    name: Evolutionary Circuit
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: All voiceless talkers link their minds, creating a circuit that empowers
          them while two or more voiceless talkers remain in the encounter.
          While this circuit is active, any psionic strike made by a voiceless
          talker deals an extra 5 damage. Additionally, when a non-minion
          voiceless talker takes damage, they can use a free triggered action to
          swap places with any voiceless talker minion on the encounter map. The
          minion takes the damage instead.
~~~