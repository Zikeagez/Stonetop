---
agility: 1
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Vertex
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 1
item_id: time-raider-vertex
item_index: 08
item_name: Time Raider Vertex
level: 3
might: 1
presence: 0
reason: 2
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster.time-raiders.statblock:time-raider-vertex
scdc:
- 1.1.1:2.18.1:08
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '62'
type: monster/time-raiders/statblock
---

~~~ds-statblock
type: statblock
name: Time Raider Vertex
level: 3
roles:
  - Platoon Support
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "62"
immunities:
  - Psychic 3
speed: 5
movement: Fly, hover
size: "2"
stability: 2
free_strike: 5
might: 1
agility: 1
reason: 2
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Psionic Slam
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
    usage: Main action
    distance: Melee 2
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage, 2 psychic damage
        tier2: 7 damage, 3 psychic damage
        tier3: 9 damage, 4 psychic damage
      - name: Effect
        effect: Any power roll made against the target gains an edge until the start of
          the vertex's next turn.
  - type: feature
    feature_type: ability
    name: Split Space
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Psionic
      - Ranged
    usage: Main action
    distance: 2 cube within 10
    target: Special
    effects:
      - name: Effect
        effect: A portal fills the area, connecting to a location the vertex has
          experienced on any plane of existence, in person or otherwise. Any
          creature who enters the portal for the first time in a round or starts
          their turn there is instantly teleported to any unoccupied space in
          the portal at the chosen location. The portal lasts until the vertex
          uses this ability again, dismisses the portal (no action required), or
          is transported by the portal.
  - type: feature
    feature_type: ability
    name: Invigorated March
    icon: ❇️
    keywords:
      - Area
      - Psionic
    usage: Maneuver
    distance: 4 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target shifts up to half their speed.
  - type: feature
    feature_type: trait
    name: Foresight
    icon: ⭐️
    effects:
      - effect: The vertex doesn't take a bane on strikes against creatures with
          concealment.
~~~