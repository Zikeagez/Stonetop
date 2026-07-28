---
agility: 2
ancestry:
- Animal
- Fey
- Shadow Elf
ev: '12'
file_basename: Brush Stalker
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 5
intuition: 1
item_id: brush-stalker
item_index: '06'
item_name: Brush Stalker
level: 4
might: 3
presence: 1
reason: -1
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster.elves-shadow.statblock:brush-stalker
scdc:
- 1.1.1:2.27.1:06
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 3
stamina: '60'
type: monster/elves-shadow/statblock
---

~~~ds-statblock
type: statblock
name: Brush Stalker
level: 4
roles:
  - Platoon Mount
ancestry:
  - Animal
  - Fey
  - Shadow Elf
ev: "12"
stamina: "60"
speed: 8
size: "2"
stability: 3
free_strike: 5
might: 3
agility: 2
reason: -1
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Gore
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage
        tier2: 10 damage
        tier3: 13 damage
  - type: feature
    feature_type: ability
    name: Reclamation
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 4 corruption damage; M < 1 weakened (save ends)
        tier2: 7 corruption damage; M < 2 weakened (save ends)
        tier3: 10 corruption damage; M < 3 weakened (save ends)
  - type: feature
    feature_type: trait
    name: Suneater
    icon: ⭐️
    effects:
      - effect: The area within 2 squares of the brush stalker is devoid of light and
          provides concealment.
  - type: feature
    feature_type: trait
    name: Wyrd Dyr
    icon: ⭐️
    effects:
      - effect: While they have line of effect to the brush stalker, any animal except
          another brush stalker is frightened.
~~~