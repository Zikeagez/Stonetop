---
file_basename: Rhodars Malice
file_dpath: Monsters/Count Rhodar Von Glauer/Features
item_id: rhodars-malice-malice-features
item_index: '39'
item_name: Rhodar's Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:rhodars-malice-malice-features
scdc:
- 1.1.1:2.2:39
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Rhodar's Malice
flavor: At the start of Rhodar's turn, you can spend Malice to activate one of
  the following features.
features:
  - type: feature
    feature_type: trait
    name: Slip
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: During this turn, Rhodar can move through creatures and objects at his
          usual speed, but can't end his turn inside a creature or object.
          Additionally, he doesn't take damage from being force moved.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: Rhodar takes an additional main action on his turn. He can use this
          feature even if he is dazed.
  - type: feature
    feature_type: trait
    name: Suffocating Dark
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: Rhodar throws one of his spears into an unoccupied space within 10
          squares, or chooses one of his spears that he has already thrown.
          Until that spear returns to him or he uses this feature again, the
          spear emanates magical darkness in a 5 aura. Rhodar can see through
          this darkness, and any enemy is suffocating while in the darkness.
  - type: feature
    feature_type: trait
    name: The Mirror Lies
    icon: 🏹
    cost: 7 Malice
    effects:
      - effect: Rhodar chooses two creatures or objects within 20 squares of him. The
          targets immediately teleport to swap places. Any enemy teleported by
          this feature who has I < 5 is dazed until the end of their next turn.
~~~