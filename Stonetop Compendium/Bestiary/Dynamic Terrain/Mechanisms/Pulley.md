---
file_basename: Pulley
file_dpath: Dynamic Terrain/Mechanisms
item_id: pulley-level-1-trigger-support
item_index: 08
item_name: Pulley (Level 1 Trigger Support)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:pulley-level-1-trigger-support
scdc:
- 1.1.1:4.1:08
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
type: featureblock
featureblock_type: Trigger Support
name: Pulley
level: 1
ev: "1"
flavor: A counterweighted pulley system can be used to quickly ascend to the top
  of a wall, scaffold, tower, or other structure.
stamina: "1"
size: 1S
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a pulley can make an **Agility
          test**.
        tier1: The creature triggers the pulley.
        tier2: The pulley is deactivated but the creature is slowed (EoT).
        tier3: The pulley is deactivated and doesn't trigger.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature adjacent to the pulley uses a maneuver to release the pulley.
      - name: Effect
        effect: The triggering creature is lifted to the top of the structure the pulley
          is attached to. The pulley must be manually reset.
  - type: feature
    feature_type: trait
    name: Climbable
    icon: ⭐️
    effects:
      - effect: A creature adjacent to the pulley can climb its ropes with an **easy
          Agility test** to ascend to the top of the structure it's attached to.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Looped Chain
        cost: +1 EV
        effect: Instead of a rope and pulley, the system uses a counterweighted looped
          chain. A looped chain automatically resets and can be triggered
          repeatedly.
~~~