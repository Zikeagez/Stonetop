---
agility: 1
ancestry:
- Abyssal
- Demon
ev: '3'
file_basename: Torlas
file_dpath: Monsters/Demons/Statblocks
free_strike: 1
intuition: 0
item_id: torlas
item_index: '33'
item_name: Torlas
level: 1
might: 0
presence: 2
reason: 0
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster.demons.statblock:torlas
scdc:
- 1.1.1:2.35.1:33
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Torlas
level: 1
roles:
  - Horde Controller
ancestry:
  - Abyssal
  - Demon
ev: "3"
stamina: "10"
weaknesses:
  - Holy 3
speed: 5
size: 1S
stability: 0
free_strike: 1
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Floor to Flesh
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: Slide 3
        tier2: Slide 4
        tier3: Slide 5
      - name: Effect
        effect: The ground in the area turns into a morass of spongy flesh before the
          targets are force moved. Until the start of the torlas's next turn,
          the area is difficult terrain, and each creature who moves in the area
          takes 1 damage for each square moved.
  - type: feature
    feature_type: ability
    name: Grasping Tendons
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - name: Effect
        effect: The torlas pulls each target up to 3 squares.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the torlas is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the torlas can't be hidden from them.
~~~