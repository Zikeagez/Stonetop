---
agility: 1
ancestry:
- Abyssal
- Demon
ev: '4'
file_basename: Bendrak
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: 0
item_id: bendrak
item_index: '27'
item_name: Bendrak
level: 2
might: 0
presence: 2
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster.demons.statblock:bendrak
scdc:
- 1.1.1:2.35.1:27
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Bendrak
level: 2
roles:
  - Horde Hexer
ancestry:
  - Abyssal
  - Demon
ev: "4"
stamina: "15"
weaknesses:
  - Holy 3
speed: 5
size: 1L
stability: 0
free_strike: 2
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Warp Perceptions
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 4 psychic damage
        tier2: 5 psychic damage; P < 1 weakened (save ends)
        tier3: 7 psychic damage; P < 2 weakened (save ends)
      - name: Effect
        effect: If the target makes a strike while weakened this way, the bendrak can
          choose a second target within distance for the strike. The first
          target takes half of any damage from the strike and the second target
          takes any remaining damage.
  - type: feature
    feature_type: ability
    name: Vanish
    icon: 🏹
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Self or one ally
    effects:
      - name: Effect
        effect: The target is invisible until the start of their next turn. They can
          then move up to 3 squares and attempt to hide.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the bendrak is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the bendrak can't be hidden from them.
~~~