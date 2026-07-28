---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '7'
file_basename: Fiktin
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 1
item_id: fiktin
item_index: '12'
item_name: Fiktin
level: 5
might: 2
presence: 3
reason: 2
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster.demons.statblock:fiktin
scdc:
- 1.1.1:2.35.1:12
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '35'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Fiktin
level: 5
roles:
  - Horde Ambusher
ancestry:
  - Abyssal
  - Demon
ev: "7"
stamina: "35"
weaknesses:
  - Holy 5
speed: 6
size: 1M
stability: 0
free_strike: 3
might: 2
agility: 2
reason: 2
intuition: 1
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Violent Transformation
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 3 corruption damage
        tier2: 6 corruption damage
        tier3: 7 corruption damage; I < 3 dazed (save ends)
      - name: Effect
        effect: The fiktin violently changes shape, dealing an extra 6 damage to any
          target they were hidden from with their Aggressive Mimicry ability.
  - type: feature
    feature_type: ability
    name: Aggressive Mimicry
    icon: 👤
    cost: 1 Malice
    keywords:
      - Magic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The fiktin transforms into a mundane object of their size or smaller and
          is automatically hidden. They can revert to their true form as a free
          maneuver.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the fiktin is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the fiktin can't be hidden from them.
~~~