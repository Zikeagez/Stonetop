---
agility: 0
ancestry:
- Elemental
ev: '20'
file_basename: Essence of Tides
file_dpath: Monsters/Elementals/Statblocks
free_strike: 5
intuition: -1
item_id: essence-of-tides
item_index: '01'
item_name: Essence of Tides
level: 3
might: 2
presence: 2
reason: 1
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster.elementals.statblock:essence-of-tides
scdc:
- 1.1.1:2.42.1:01
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '80'
type: monster/elementals/statblock
---

~~~ds-statblock
type: statblock
name: Essence of Tides
level: 3
roles:
  - Elite Controller
ancestry:
  - Elemental
ev: "20"
stamina: "80"
immunities:
  - Cold 5
speed: 7
movement: Swim
size: 1M
stability: 1
free_strike: 5
might: 2
agility: 0
reason: 1
intuition: -1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Water Wing
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; slide 1
        tier2: 11 damage; slide 2
        tier3: 14 damage; slide 3
      - name: Effect
        effect: If a target has P < 2, their stability is reduced to 0 and they move 2
          additional squares whenever they are force moved (save ends).
  - type: feature
    feature_type: ability
    name: Convocation of Waves
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - name: Effect
        effect: Until the start of the essence's next turn, the target has cold immunity
          5.
      - cost: 3 Malice
        effect: Until the end of the encounter, the ground within 1 square of the target
          is a pool of water that is difficult terrain. This water extends out
          behind the target as they move, creating a stream that lasts until the
          end of the encounter. Any enemy who ends their turn in the stream and
          has M < 2 is slowed (save ends).
  - type: feature
    feature_type: ability
    name: Sea-Salted Wounds
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: One enemy
    trigger: An ally deals rolled damage to the target.
    effects:
      - name: Effect
        effect: The essence makes a free strike against the target.
  - type: feature
    feature_type: trait
    name: Fickle and Free
    icon: ⭐️
    effects:
      - effect: The essence can't be restrained, slowed, or knocked prone, and they
          ignore difficult terrain.
  - type: feature
    feature_type: trait
    name: Water Glide
    icon: ⭐️
    effects:
      - effect: Whenever the essence starts their turn in a space containing water, they
          can fly until the end of their turn. While flying, the essence doesn't
          provoke opportunity attacks.
~~~