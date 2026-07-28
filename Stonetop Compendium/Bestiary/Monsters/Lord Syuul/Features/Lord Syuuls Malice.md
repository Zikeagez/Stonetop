---
file_basename: Lord Syuuls Malice
file_dpath: Monsters/Lord Syuul/Features
item_id: lord-syuuls-malice-malice-features
item_index: '30'
item_name: Lord Syuul's Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:lord-syuuls-malice-malice-features
scdc:
- 1.1.1:2.2:30
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Lord Syuul's Malice
flavor: At the start of Lord Syuul's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Guise
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: Lord Syuul projects a psionic screen over his body, preventing other
          creatures from treating him as an enemy until the end of his next
          turn.
  - type: feature
    feature_type: trait
    name: Do It for Me
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: Lord Syuul psionically plunders the minds of each creature within 2
          squares of him. Each such creature makes a **Reason test**.
        tier1: 13 psychic damage; the target uses a signature ability against a creature
          of Lord Syuul's choice
        tier2: 10 psychic damage; the target makes a free strike against a creature of
          Lord Syuul's choice
        tier3: No effect.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: Lord Syuul takes an additional main action on his turn. He can use this
          feature even if he is dazed.
  - type: feature
    feature_type: trait
    name: Overpower
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Lord Syuul sends out a psionic burst to completely overpower his
          greatest threats. He makes a **Reason test** (2d10 + 4).
        tier1: Lord Syuul has damage weakness 5.
        tier2: Lord Syuul has damage immunity 2.
        tier3: Lord Syuul has damage immunity 5.
      - effect: >-
          Once per round as a maneuver, Lord Syuul can repeat this test,
          replacing the previous Overpower effect.


          Whenever an Overpower effect is active, any hero who has one or more
          psionic abilities can use a maneuver to push back by making a **Reason
          test**, replacing the previous Overpower effect.
        tier1: Lord Syuul has damage immunity 5.
        tier2: Lord Syuul has damage immunity 2.
        tier3: Lord Syuul has damage weakness 5.
      - effect: The Overpower effect lasts until the end of the encounter.
~~~