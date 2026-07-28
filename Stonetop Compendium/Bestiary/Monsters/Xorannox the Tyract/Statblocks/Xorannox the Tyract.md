---
agility: 2
ancestry:
- Horror
- Overmind
ev: '96'
file_basename: Xorannox the Tyract
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 7
intuition: 3
item_id: xorannox-the-tyract
item_index: '04'
item_name: Xorannox the Tyract
level: 6
might: 4
presence: 3
reason: 4
roles:
- Solo
scc:
- mcdm.monsters.v1:monster.xorannox the tyract.statblock:xorannox-the-tyract
scdc:
- 1.1.1:2.41.1:04
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '450'
type: monster/xorannox the tyract/statblock
---

~~~ds-statblock
type: statblock
name: Xorannox the Tyract
level: 6
roles:
  - Solo
ancestry:
  - Horror
  - Overmind
ev: "96"
stamina: "450"
speed: 5
movement: Fly, hover
size: "3"
stability: 2
free_strike: 7
might: 4
agility: 2
reason: 4
intuition: 3
presence: 3
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of his turns, Xorannox can take 10 damage to end one
          effect on him that can be ended by a saving throw. This damage can't
          be reduced in any way.
      - name: Solo Turns
        effect: Xorannox can take two turns each round. He can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Eyes of the Tyract
    icon: 🌀
    effects:
      - effect: Six unique eyestalks float around Xorannox, acting on his turn at his
          command until they are reduced to 0 Stamina. On each of Xorannox's
          turns, he directs one eyestalk to move and use a signature ability.
  - type: feature
    feature_type: ability
    name: Toothful Thrashing
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 12 damage; slide 2; M < 2 bleeding (EoT)
        tier2: 20 damage; slide 3; M < 3 bleeding (EoT)
        tier3: 23 damage; vertical slide 3; M < 4 bleeding (EoT)
  - type: feature
    feature_type: ability
    name: Grav Spike
    icon: ❇️
    keywords:
      - Area
      - Psionic
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: Vertical push 3
        tier2: Vertical push 5
        tier3: Vertical push 7
      - name: Effect
        effect: Xorannox shifts up to his speed before or after using this ability.
  - type: feature
    feature_type: ability
    name: Optical Collusion
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Xorannox commands all his eyestalks to move up to their speed.
  - type: feature
    feature_type: ability
    name: Shutout
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 5 x 2 line within 1
    target: Special
    effects:
      - name: Effect
        effect: Xorannox ends all ongoing supernatural effects and suppresses
          supernatural effects from treasures in the area. New supernatural
          effects can't be activated in the area until the end of Xorannox's
          next turn.
  - type: feature
    feature_type: ability
    name: Cower!
    icon: ❗️
    keywords:
      - Psionic
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance deals damage to Xorannox.
    effects:
      - name: Effect
        effect: If the target has I < 3 they are frightened (save ends)
  - type: feature
    feature_type: trait
    name: Above It All
    icon: ⭐️
    effects:
      - effect: Xorannox can't be made frightened or knocked prone, and he can't be
          flanked.
  - type: feature
    feature_type: trait
    name: Natural Enemies
    icon: ⭐️
    effects:
      - effect: If Xorannox perceives another overmind or a voiceless talker on the
          encounter map, he targets that threat one or more times on each of his
          turns.
  - type: feature
    feature_type: ability
    name: Disruption Beam
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: "-"
    distance: Ranged 10
    target: Three creatures
    effects:
      - roll: Power Roll + 4
        tier1: 11 psychic damage; R < 2 dazed (save ends)
        tier2: 17 psychic damage; R < 3 dazed (save ends)
        tier3: 20 psychic damage; R < 4 dazed (save ends)
  - type: feature
    feature_type: ability
    name: All Eyes, All Rise
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Xorannox recreates any destroyed eyestalks, which return in unoccupied
          spaces on the encounter map with full Stamina.
  - type: feature
    feature_type: ability
    name: Panoptibeam
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
    usage: "-"
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Xorannox directs each of his eyestalks to use a signature ability
          against any target.
~~~