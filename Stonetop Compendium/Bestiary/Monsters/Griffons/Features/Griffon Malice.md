---
file_basename: Griffon Malice
file_dpath: Monsters/Griffons/Features
item_id: griffon-malice-malice-features
item_index: '10'
item_name: Griffon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:griffon-malice-malice-features
scdc:
- 1.1.1:2.2:10
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Griffon Malice
flavor: At the start of any griffon's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: ability
    name: Swoop
    icon: 👤
    cost: 3 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The griffon flies up to their speed, and can make a free strike against
          each creature who makes an opportunity attack against them during this
          movement.
  - type: feature
    feature_type: trait
    name: Piercing Cry
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: A griffon acting this turn unleashes a hideous screech at one enemy
          within 5 squares of them, forcing that creature to make an **Intuition
          test**.
        tier1: Frightened (save ends)
        tier2: Frightened (EoT)
        tier3: No effect.
  - type: feature
    feature_type: trait
    name: Wildwinds
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: Winds bluster and blow across the encounter map. Until the end of the
          encounter, each creature who can't fly or isn't mounted on a flying
          creature takes a −3 penalty to stability, and any forced movement
          effect targeting such a creature moves them an additional 5 squares.
~~~