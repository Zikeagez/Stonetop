---
agility: 0
ancestry:
- Abyssal
- Demon
- Hobgoblin
ev: '24'
file_basename: Slaughter Demon
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 1
item_id: slaughter-demon
item_index: '14'
item_name: Slaughter Demon
level: 4
might: 3
presence: 0
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:slaughter-demon
scdc:
- 1.1.1:2.22.1:14
size: '3'
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '140'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Slaughter Demon
level: 4
roles:
  - Elite Brute
ancestry:
  - Abyssal
  - Demon
  - Hobgoblin
ev: "24"
stamina: "140"
immunities:
  - Fire 5
speed: 7
movement: Burrow
size: "3"
stability: 3
free_strike: 6
might: 3
agility: 0
reason: -1
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Steely Skewer
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 14 damage; A < 2 bleeding (save ends)
        tier3: 17 damage; A < 3 bleeding and restrained (save ends)
      - name: Effect
        effect: A creature restrained this way moves with the slaughter demon. The
          slaughter demon can have up to six creatures or objects restrained at
          once.
  - type: feature
    feature_type: ability
    name: Tail Stinger
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 5
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 10 poison damage; M < 1 weakened (save ends)
        tier2: 16 poison damage; M < 2 weakened (save ends)
        tier3: 20 poison damage; M < 3 weakened (save ends)
      - name: Effect
        effect: A target weakened this way also has damage weakness 3.
  - type: feature
    feature_type: trait
    name: Drag Below
    icon: ⭐️
    effects:
      - effect: The slaughter demon can make a free strike as part of using the Dig
          maneuver. If the target of the free strike has M < 2, they are grabbed
          and take a bane on the Escape Grab maneuver.
  - type: feature
    feature_type: ability
    name: Devour Soul
    icon: ❗️
    keywords:
      - Area
      - Magic
    usage: Triggered action
    distance: 5 burst
    target: The triggering creature
    trigger: A creature within distance who has a soul dies.
    effects:
      - name: Effect
        effect: The target can't be brought back to life. Until the end of the
          encounter, the slaughter demon gains an edge on power rolls.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the slaughter demon can't be hidden
          from them.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the slaughter demon is winded, they gain an edge on strikes, and
          any strike made against them gains an edge.
~~~