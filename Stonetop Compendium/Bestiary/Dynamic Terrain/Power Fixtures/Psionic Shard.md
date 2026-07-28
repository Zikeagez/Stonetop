---
file_basename: Psionic Shard
file_dpath: Dynamic Terrain/Power Fixtures
item_id: psionic-shard-level-5-fortification-defender
item_index: '01'
item_name: Psionic Shard (Level 5 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.power-fixture:psionic-shard-level-5-fortification-defender
scdc:
- 1.1.1:4.4:01
source: mcdm.monsters.v1
type: dynamic-terrain/power-fixture
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Defender
name: Psionic Shard
level: 5
ev: "7"
flavor: A massive humming crystal makes the air around it feel thick.
stamina: "40"
size: "2"
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: The psionic shard must be completely destroyed.
  - type: feature
    feature_type: trait
    name: Psionic Barrier
    icon: ⭐️
    effects:
      - effect: A psionic shard is attuned to one side in an encounter. While a psionic
          shard is intact, any damage dealt to each ally of the shard in the
          encounter is halved.
  - type: feature
    feature_type: ability
    name: Psionic Pulse
    icon: ❗️
    keywords:
      - "-"
    usage: Free triggered action
    distance: Special
    target: Special
    trigger: The shard is destroyed.
    effects:
      - name: Effect
        effect: The shard releases a shockwave channeled through each creature affected
          by Psionic Barrier. Each ally in the encounter is dazed until the end
          of their next turn.
~~~