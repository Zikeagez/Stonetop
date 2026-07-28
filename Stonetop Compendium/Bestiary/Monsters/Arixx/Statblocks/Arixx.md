---
agility: 1
ancestry:
- Arixx
- Beast
ev: '36'
file_basename: Arixx
file_dpath: Monsters/Arixx/Statblocks
free_strike: 5
intuition: 1
item_id: arixx
item_index: '01'
item_name: Arixx
level: 1
might: 3
presence: -4
reason: -3
roles:
- Solo
scc:
- mcdm.monsters.v1:monster.arixx.statblock:arixx
scdc:
- 1.1.1:2.30.1:01
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '200'
type: monster/arixx/statblock
---

~~~ds-statblock
type: statblock
name: Arixx
level: 1
roles:
  - Solo
ancestry:
  - Arixx
  - Beast
ev: "36"
stamina: "200"
speed: 5
movement: Burrow
size: "2"
stability: 2
free_strike: 5
might: 3
agility: 1
reason: -3
intuition: 1
presence: -4
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the arixx can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The arixx can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Earthwalk
    icon: ⭐️
    effects:
      - effect: Difficult terrain composed of earth or loose rock doesn't cost the arixx
          extra movement.
  - type: feature
    feature_type: trait
    name: Soft Underbelly
    icon: ⭐️
    effects:
      - effect: A prone creature making a melee strike against the arixx has a double
          edge on the strike instead of taking a bane.
  - type: feature
    feature_type: ability
    name: Bite
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
        tier1: 9 damage; grabbed
        tier2: 13 damage; grabbed
        tier3: 16 damage; grabbed
      - name: Effect
        effect: A size 1 target grabbed this way takes 3 acid damage at the start of
          each of their turns.
  - type: feature
    feature_type: ability
    name: Claw Swing
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage; A < 1 grabbed
        tier2: 8 damage; A < 2 grabbed
        tier3: 11 damage; A < 3 grabbed
      - name: Effect
        effect: The arixx can vertically slide each grabbed target up to 3 squares.
  - type: feature
    feature_type: ability
    name: Spitfire
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 4 acid damage
        tier2: 6 acid damage
        tier3: 7 acid damage; prone
      - name: Effect
        effect: The ground beneath each target is covered in burning acid until the end
          of the encounter. Any enemy who enters an affected space for the first
          time in a round or starts their turn there takes 2 acid damage.
  - type: feature
    feature_type: ability
    name: Dirt Devil
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
    usage: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 4 damage
        tier2: 6 damage; push 2
        tier3: 7 damage; push 4
      - name: Effect
        effect: The arixx flings rocks and debris to fill the area, and has a double
          edge on the power roll if they started their turn underground. The
          area is difficult terrain.
  - type: feature
    feature_type: ability
    name: Dust Cloud
    icon: ❇️
    keywords:
      - Area
    usage: Maneuver
    distance: 1 burst
    target: Special
    effects:
      - name: Effect
        effect: The arixx kicks up dust to fill the area until the start of their next
          turn, then moves up to their speed. Any enemy in the area or who
          targets a creature in the area takes a bane on power rolls.
  - type: feature
    feature_type: ability
    name: Skitter
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The arixx takes damage.
    effects:
      - name: Effect
        effect: The arixx halves the damage and shifts up to 3 squares after the
          triggering effect resolves.
  - type: feature
    feature_type: ability
    name: Acid Spew
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 10 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 acid damage
        tier2: 8 acid damage
        tier3: 11 acid damage
      - name: Effect
        effect: The ground in the area is covered in a puddle of acid until the end of
          the encounter. Any enemy who enters the area for the first time in a
          round or starts their turn there takes 2 acid damage.
  - type: feature
    feature_type: ability
    name: Sinkhole
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The arixx shifts up to their speed. If they end this shift above ground
          and within 2 squares of a creature, they use Bite against the creature
          and can then use the Dig maneuver.
  - type: feature
    feature_type: ability
    name: Acid and Claws
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 2 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 acid damage; M < 1 weakened (save ends)
        tier2: 8 acid damage; M < 2 weakened (save ends)
        tier3: 11 acid damage; M < 3 weakened (save ends)
~~~