---
agility: 1
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Fury
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 0
item_id: rival-fury
item_index: '02'
item_name: Rival Fury
level: 2
might: 2
presence: 0
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster.rivals.1st echelon.statblock:rival-fury
scdc:
- 1.1.1:2.5.1.1:02
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '100'
type: monster/rivals/1st echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Fury
level: 2
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "100"
speed: 5
size: 1M
stability: 3
free_strike: 5
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Brutal Impact
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; push 1
        tier2: 11 damage; push 2
        tier3: 14 damage; push 3
      - cost: 2 Malice
        effect: Each target who has M < 1 is slowed (save ends).
  - type: feature
    feature_type: ability
    name: Let's Tussle
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 8 damage; M < 0 grabbed
        tier2: 13 damage; M < 1 grabbed
        tier3: 16 damage; M < 2 grabbed
      - name: Effect
        effect: The target must be the fury's size or smaller. While the target is
          grabbed this way, the fury gains an edge on strikes against them.
  - type: feature
    feature_type: trait
    name: Overwhelm
    icon: ⭐️
    effects:
      - effect: Once per turn, when the fury force moves a creature or object, or shifts
          adjacent to a creature or object, they can make a free strike against
          that creature or object.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the fury chooses one creature within their
          line of effect. Both the fury and the creature can add a d3 roll to
          power rolls they make against each other.
~~~