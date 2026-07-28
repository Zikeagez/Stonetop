---
file_basename: Undead Malice Level 10 Malice Features
file_dpath: Monsters/Undead/Features
include_parens_in_filename: 'true'
item_id: undead-malice-level-10-malice-features
item_index: 09
item_name: Undead Malice (Level 10 Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:undead-malice-level-10-malice-features
scdc:
- 1.1.1:2.2:09
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Undead Malice
level: 10
flavor: At the start of any level 10 undead's turn, you can spend Malice to
  activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Prior Malice Features
    icon: ⭐️
    cost: 2-7+ Malice
    effects:
      - effect: The undead activates a Malice feature available to undead of level 9 or
          lower.
  - type: feature
    feature_type: trait
    name: Death Tax
    icon: ❇️
    cost: 7 Malice
    effects:
      - effect: The undead attempts to rend the vitality of their foes. Each enemy
          within 5 squares of the undead makes a **Might test**.
        tier1: 10 corruption damage; the target loses 2 Recoveries
        tier2: 8 corruption damage; the target loses 1 Recovery
        tier3: 5 corruption damage
      - name: Effect
        effect: A target who has fewer Recoveries than they would lose is also weakened
          (save ends).
      - name: Special
        effect: This ability can't be used by a minion.
~~~