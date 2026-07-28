---
agility: 3
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '14'
file_basename: Hobgoblin Firerunner
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 1
item_id: hobgoblin-firerunner
item_index: '15'
item_name: Hobgoblin Firerunner
level: 5
might: 2
presence: 0
reason: 1
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster.hobgoblins.statblock:hobgoblin-firerunner
scdc:
- 1.1.1:2.22.1:15
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '70'
type: monster/hobgoblins/statblock
---

~~~ds-statblock
type: statblock
name: Hobgoblin Firerunner
level: 5
roles:
  - Platoon Harrier
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "14"
stamina: "70"
immunities:
  - Fire 5
speed: 8
size: 1M
stability: 0
free_strike: 6
might: 2
agility: 3
reason: 1
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Flaming Kick
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 9 fire damage
        tier2: 13 fire damage
        tier3: 16 fire damage; A < 3 dazed (EoT)
  - type: feature
    feature_type: ability
    name: Blazing Trail
    icon: 👤
    keywords:
      - Magic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The firerunner moves up to their speed and creates an 8 wall of fire
          along the path of their movement. Creatures can enter and pass through
          the wall. Any enemy who enters the wall for the first time in a round
          or starts their turn there takes 5 fire damage.
  - type: feature
    feature_type: trait
    name: Hot to Go
    icon: ⭐️
    effects:
      - effect: Whenever the firerunner takes fire damage for the first time in round,
          their speed and the size of the wall they can create with Blazing
          Trail increases by 4 until the end of their next turn.
  - type: feature
    feature_type: trait
    name: Kindlestep
    icon: ⭐️
    effects:
      - effect: The firerunner ignores difficult terrain.
  - type: feature
    feature_type: trait
    name: Infernal Ichor
    icon: ⭐️
    effects:
      - effect: When the firerunner is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the firerunner takes 3 fire damage.
~~~