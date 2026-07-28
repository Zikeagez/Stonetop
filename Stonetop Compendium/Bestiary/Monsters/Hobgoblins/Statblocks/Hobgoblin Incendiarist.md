---
agility: 3
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '14'
file_basename: Hobgoblin Incendiarist
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 2
item_id: hobgoblin-incendiarist
item_index: '12'
item_name: Hobgoblin Incendiarist
level: 5
might: 1
presence: 1
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:hobgoblin-incendiarist
scdc:
- 1.1.1:2.22.1:12
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Hobgoblin Incendiarist
level: 5
roles:
  - Platoon Artillery
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "14"
stamina: "60"
immunities:
  - Fire 5
speed: 5
size: 1M
stability: 0
free_strike: 6
might: 1
agility: 3
reason: 0
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Fire Crossbow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 9 fire damage
        tier2: 14 fire damage
        tier3: 17 fire damage; A < 3 burning (save ends)
      - name: Effect
        effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - type: feature
    feature_type: ability
    name: Fireball Volley
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 4 cube within 10
    target: Each enemy or object in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 fire damage; A < 1 burning (save ends)
        tier2: 9 fire damage; A < 2 burning (save ends)
        tier3: 11 fire damage; prone; A < 3 burning (save ends)
      - name: Effect
        effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - type: feature
    feature_type: trait
    name: Raining Cinders
    icon: ⭐️
    effects:
      - effect: The ranged free strike of each ally within 3 squares of the incendiarist
          has a distance of 10 and deals fire damage.
  - type: feature
    feature_type: trait
    name: Infernal Ichor
    icon: ⭐️
    effects:
      - effect: When the incendiarist is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the incendiarist takes 3 fire damage.
~~~