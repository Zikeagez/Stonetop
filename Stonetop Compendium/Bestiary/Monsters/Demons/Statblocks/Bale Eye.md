---
agility: 0
ancestry:
- Abyssal
- Demon
ev: '7'
file_basename: Bale Eye
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 3
item_id: bale-eye
item_index: '31'
item_name: Bale Eye
level: 5
might: 0
presence: 3
reason: 3
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster.demons.statblock:bale-eye
scdc:
- 1.1.1:2.35.1:31
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '30'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Bale Eye
level: 5
roles:
  - Horde Hexer
ancestry:
  - Abyssal
  - Demon
ev: "7"
stamina: "30"
weaknesses:
  - Holy 5
speed: 6
movement: Fly
size: "4"
stability: 2
free_strike: 3
might: 0
agility: 0
reason: 3
intuition: 3
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Wilting Visions
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 15
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 6 psychic damage
        tier2: 8 psychic damage
        tier3: 9 psychic damage
      - name: Effect
        effect: The target has corruption weakness 5 (EoT).
      - cost: 2 Malice
        effect: If the target has I < 2, they have corruption weakness 5 (save ends).
  - type: feature
    feature_type: ability
    name: Demonwarp Tears
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 4 cube within 5
    target: Each enemy in the area
    effects:
      - name: Special
        effect: The bale eye must create the cube beneath themself.
      - roll: Power Roll + 3
        tier1: 3 psychic damage; A < 1 the target is warped (save ends)
        tier2: 5 psychic damage; A < 2 the target is warped (save ends)
        tier3: 6 psychic damage; A < 3 the target is warped (save ends)
      - name: Effect
        effect: While warped, a creature has a double bane on power rolls using any
          characteristic higher than 0, and has a double edge on power rolls
          using any characteristic lower than 0.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the bale eye is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 5 squares of the bale eye can't be hidden from them.
~~~