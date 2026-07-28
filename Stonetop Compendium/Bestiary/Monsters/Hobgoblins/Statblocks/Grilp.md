---
agility: 3
ancestry:
- Devil
- Hobgoblin
- Infernal
ev: 6 for four minions
file_basename: Grilp
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 3
intuition: 1
item_id: grilp
item_index: '04'
item_name: Grilp
level: 4
might: -1
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:grilp
scdc:
- 1.1.1:2.22.1:04
size: 1T
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '8'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Grilp
level: 4
roles:
  - Minion Ambusher
ancestry:
  - Devil
  - Hobgoblin
  - Infernal
ev: 6 for four minions
stamina: "8"
immunities:
  - Fire 2
speed: 7
movement: Fly
size: 1T
stability: 0
free_strike: 3
with_captain: +2 bonus to speed
might: -1
agility: 3
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Flyby Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 damage
        tier2: 5 damage
        tier3: 7 damage; the grilp shifts up to 2 squares
      - name: Effect
        effect: The grilp moves up to their speed and can attempt to hide.
  - type: feature
    feature_type: trait
    name: Bat Out Of Hell
    icon: ⭐️
    effects:
      - effect: Any enemy who makes a saving throw takes a −1 penalty to the saving
          throw for each grilp adjacent to them.
  - type: feature
    feature_type: trait
    name: Shifting Camouflage
    icon: ⭐️
    effects:
      - effect: The grilp has concealment from all creatures.
~~~