---
agility: 0
ancestry:
- Abyssal
- Demon
ev: '8'
file_basename: Tormenauk
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 1
item_id: tormenauk
item_index: '28'
item_name: Tormenauk
level: 6
might: 3
presence: 2
reason: 2
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster.demons.statblock:tormenauk
scdc:
- 1.1.1:2.35.1:28
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '45'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Tormenauk
level: 6
roles:
  - Horde Brute
ancestry:
  - Abyssal
  - Demon
ev: "8"
stamina: "45"
weaknesses:
  - Holy 5
speed: 6
size: "2"
stability: 2
free_strike: 4
might: 3
agility: 0
reason: 2
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Many Maws
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage
        tier2: 9 damage
        tier3: 11 damage; grabbed, and the target takes a bane on the Escape Grab
          maneuver
      - name: Effect
        effect: Any target grabbed this way takes 4 psychic damage at the start of each
          of the tormenauk's turns.
  - type: feature
    feature_type: ability
    name: Agony Wail
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 4 psychic damage; I < 1 dazed (save ends)
        tier2: 6 psychic damage; I < 2 dazed (save ends)
        tier3: 8 psychic damage; I < 3 dazed (save ends)
      - name: Effect
        effect: The potency increases by 1 if the target is grabbed by the tormenauk.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the tormenauk is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the tormenauk can't be hidden from
          them.
~~~