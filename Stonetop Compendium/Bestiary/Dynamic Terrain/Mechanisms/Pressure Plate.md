---
file_basename: Pressure Plate
file_dpath: Dynamic Terrain/Mechanisms
item_id: pressure-plate-level-1-trigger-support
item_index: '03'
item_name: Pressure Plate (Level 1 Trigger Support)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:pressure-plate-level-1-trigger-support
scdc:
- 1.1.1:4.1:03
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
type: featureblock
featureblock_type: Trigger Support
name: Pressure Plate
level: 1
ev: "2"
flavor: This mechanism acts as a trigger for another linked mechanism, and is
  skillfully hidden from view in the floor.
stamina: "-"
size: Any area
stats:
  - name: Typical Space
    value: One square, up to a 4 x 4-square area
  - name: Link
    value: A pressure plate is linked to another mechanism that it activates when
      triggered.
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a pressure plate can make an
          **Agility test**.
        tier1: The creature triggers the pressure plate.
        tier2: The pressure plate is deactivated but the creature is slowed (EoT).
        tier3: The pressure plate is deactivated and doesn't trigger.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: The pressure plate is calibrated to be triggered by creatures or objects
          of a particular size. The pressure plate triggers when a creature or
          object of the appropriate size enters its area.
      - name: Effect
        effect: The linked mechanism is activated. A pressure plate automatically resets
          and can be triggered repeatedly.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Tripwire
        cost: −1 EV
        effect: The pressure plate is a tripwire, which can trigger once and must be
          manually reset. A concealed tripwire can be discovered with an **easy
          Intuition test**.
  - type: feature
    feature_type: trait
    name: Hidden
    icon: ⭐️
    effects:
      - effect: The pressure plate is hidden until triggered or detected.
~~~