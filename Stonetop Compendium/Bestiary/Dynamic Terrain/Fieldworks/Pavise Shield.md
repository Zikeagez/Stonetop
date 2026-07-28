---
file_basename: Pavise Shield
file_dpath: Dynamic Terrain/Fieldworks
item_id: pavise-shield-level-1-fortification-defender
item_index: '03'
item_name: Pavise Shield (Level 1 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:pavise-shield-level-1-fortification-defender
scdc:
- 1.1.1:4.3:03
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Defender
name: Pavise Shield
level: 1
ev: "1"
flavor: A reinforced metal shield embedded in the ground acts as cover for the
  creature controlling it.
stamina: "9"
size: 1M
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a pavise shield controlled by
          another creature can make a **Might test**.
        tier1: The creature controlling the shield retains control of it and can make an
          opportunity attack against the creature making the test.
        tier2: The creature controlling the shield retains control of it.
        tier3: The creature making the test grabs the shield and takes control of it.
  - type: feature
    feature_type: trait
    name: Controlling the Shield
    icon: ⭐️
    effects:
      - effect: >-
          While a creature has the pavise shield grabbed, they have cover and
          take half damage from abilities whose line of effect extends through
          the shield. The pavise shield takes the other half of the damage.


          While a creature has a pavise shield grabbed, their speed is halved
          and they move the shield like a grabbed creature.
~~~