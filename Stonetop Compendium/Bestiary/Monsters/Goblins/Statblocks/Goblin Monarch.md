---
agility: 3
ancestry:
- Goblin
- Humanoid
ev: '12'
file_basename: Goblin Monarch
file_dpath: Monsters/Goblins/Statblocks
free_strike: 4
intuition: 0
item_id: goblin-monarch
item_index: '06'
item_name: Goblin Monarch
level: 1
might: 0
presence: 3
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster.goblins.statblock:goblin-monarch
scdc:
- 1.1.1:2.40.1:06
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '80'
type: monster/goblins/statblock
---

~~~ds-statblock
type: statblock
name: Goblin Monarch
level: 1
roles:
  - Leader
ancestry:
  - Goblin
  - Humanoid
ev: "12"
stamina: "80"
speed: 6
movement: Climb
size: 1S
stability: 1
free_strike: 4
might: 0
agility: 3
reason: 1
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Handaxe
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage
        tier2: 10 damage
        tier3: 13 damage
      - name: Effect
        effect: One ally within 10 squares of the monarch can make a free strike.
  - type: feature
    feature_type: ability
    name: Get in Here!
    icon: 🏹
    cost: 1 Malice
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 20
    target: Special
    effects:
      - name: Effect
        effect: Two goblin runners appear in unoccupied spaces within distance.
  - type: feature
    feature_type: ability
    name: Meat Shield
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: One ally
    trigger: A creature targets the monarch with a strike.
    effects:
      - name: Effect
        effect: The ally is the target of the triggering strike instead.
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The monarch doesn't provoke opportunity attacks by moving.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the monarch can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - type: feature
    feature_type: ability
    name: What Are You Waiting For?
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target can move up to their speed or make a free strike.
  - type: feature
    feature_type: ability
    name: Focus Fire
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: One enemy or object
    effects:
      - name: Effect
        effect: Each ally within 10 squares of the target can move up to their speed
          toward the target.
  - type: feature
    feature_type: ability
    name: Kill!
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Special
    target: Special
    effects:
      - name: Effect
        effect: Each enemy in the encounter takes 2 damage for each goblin adjacent to
          them.
~~~