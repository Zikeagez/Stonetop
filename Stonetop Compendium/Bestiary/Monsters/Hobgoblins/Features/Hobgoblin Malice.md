---
file_basename: Hobgoblin Malice
file_dpath: Monsters/Hobgoblins/Features
item_id: hobgoblin-malice-malice-features
item_index: '23'
item_name: Hobgoblin Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:hobgoblin-malice-malice-features
scdc:
- 1.1.1:2.2:23
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Hobgoblin Malice
flavor: At the start of any hobgoblin's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Goblin Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The hobgoblin activates a Malice Feature available to goblins.
  - type: feature
    feature_type: trait
    name: Operation Goblin Mode
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each goblin in the encounter gains a +3 bonus to speed until the end of
          the round.
  - type: feature
    feature_type: trait
    name: Operation Tactical Swarm
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Each hobgoblin in the encounter shifts up to their speed and can take
          the Defend main action.
  - type: feature
    feature_type: trait
    name: Operation Earth Sear
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Until the end of the round, the ground throughout the encounter map
          becomes blazing hot. Any enemy takes 1 fire damage for each square of
          the ground they enter. Any enemy who ends their turn on the ground has
          fire weakness 2 until the start of their next turn.
~~~