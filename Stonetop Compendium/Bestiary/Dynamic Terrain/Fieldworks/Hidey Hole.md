---
file_basename: Hidey Hole
file_dpath: Dynamic Terrain/Fieldworks
item_id: hidey-hole-level-1-fortification-ambusher
item_index: '04'
item_name: Hidey-Hole (Level 1 Fortification Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:hidey-hole-level-1-fortification-ambusher
scdc:
- 1.1.1:4.3:04
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Ambusher
name: Hidey-Hole
level: 1
ev: "1"
flavor: A cavity in a floor, wall, or ceiling might hold hidden threats.
stamina: "-"
size: One or more squares
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a hidey-hole can make a **Might
          test**.
        tier1: The creature is restrained (save ends).
        tier2: The hidey-hole collapses but the creature is slowed (save ends).
        tier3: The hidey-hole collapses and can no longer be used until repaired.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature starts the encounter in the hidey-hole or ends their turn
          there.
      - name: Effect
        effect: The triggering creature can attempt to hide as a free triggered action.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Network
        cost: +1 EV per hidey-hole
        effect: The hidey-hole is connected to a tunnel network. A creature familiar
          with the network can move from one hidey-hole to any space adjacent to
          a connected hidey-hole if they have movement available equal to the
          straight-line distance to that space. A creature unfamiliar with the
          network can use a maneuver to make a **hard Intuition test** to
          discover a connected hidey-hole.
~~~