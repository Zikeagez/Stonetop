---
agility: 2
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '16'
file_basename: Hobgoblin Grandguard
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 0
item_id: hobgoblin-grandguard
item_index: '07'
item_name: Hobgoblin Grandguard
level: 6
might: 3
presence: 2
reason: 3
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:hobgoblin-grandguard
scdc:
- 1.1.1:2.22.1:07
size: '2'
source: mcdm.monsters.v1
speed: 4
stability: 4
stamina: '111'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Hobgoblin Grandguard
level: 6
roles:
  - Platoon Defender
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "16"
stamina: "111"
immunities:
  - Fire 6
speed: 4
size: "2"
stability: 4
free_strike: 6
might: 3
agility: 2
reason: 3
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Tower Shield Smash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 14 damage
        tier3: 17 damage; prone
      - cost: 3 Malice
        effect: Each ally adjacent to a prone target can make a free strike against that
          target.
  - type: feature
    feature_type: ability
    name: Thunder Rush
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Charge
      - Weapon
    usage: Main action
    distance: 1 x 2 line within 1
    target: Each enemy or object in the area
    effects:
      - roll: Power Roll + 3
        tier1: 6 damage
        tier2: 11 damage
        tier3: 14 damage
      - name: Effect
        effect: Each target is pushed up to 10 squares in the same direction, and the
          grandguard shifts into the area left behind by the targets.
  - type: feature
    feature_type: trait
    name: Wide Guard
    icon: ⭐️
    effects:
      - effect: Any strike made against an ally within 2 squares of the grandguard takes
          a bane.
  - type: feature
    feature_type: trait
    name: Infernal Ichor
    icon: ⭐️
    effects:
      - effect: When the grandguard is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the grandguard takes 3 fire damage.
~~~