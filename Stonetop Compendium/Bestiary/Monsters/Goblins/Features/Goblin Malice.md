---
file_basename: Goblin Malice
file_dpath: Monsters/Goblins/Features
item_id: goblin-malice-malice-features
item_index: '43'
item_name: Goblin Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:goblin-malice-malice-features
scdc:
- 1.1.1:2.2:43
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Goblin Malice
flavor: At the start of any goblin's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Goblin Mode
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each goblin in the encounter gains a +2 bonus to speed until the end of
          the round.
  - type: feature
    feature_type: trait
    name: Tiny Stabs
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: Each enemy in the encounter takes 1 damage for each goblin adjacent to
          them.
  - type: feature
    feature_type: trait
    name: Swamp Stink
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: The encounter map is covered in a green mist that lasts until the end of
          the round, and which can't be dispersed by wind. All areas of the map
          are difficult terrain for non-goblins, and each non-goblin on the map
          makes a **Might test**.
        tier1: 5 poison damage; the creature is weakened until the mist disappears.
        tier2: The creature is weakened until the mist disappears.
        tier3: No effect.
~~~