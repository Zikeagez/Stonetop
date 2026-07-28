---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '20'
file_basename: Orc Warleader
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: 2
item_id: orc-warleader
item_index: '06'
item_name: Orc Warleader
level: 3
might: 3
presence: 2
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-warleader
scdc:
- 1.1.1:2.16.1:06
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '120'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Warleader
level: 3
roles:
  - Leader
ancestry:
  - Humanoid
  - Orc
ev: "20"
stamina: "120"
speed: 6
size: 1M
stability: 2
free_strike: 5
might: 3
agility: 2
reason: 1
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Go.
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
    usage: Main action
    distance: Ranged 10
    target: One ally
    effects:
      - name: Effect
        effect: The target moves up to their speed and can use a main action.
      - cost: 1 Malice
        effect: The warleader targets two allies.
      - cost: 3 Malice
        effect: The warleader targets one ally and a minion squad.
  - type: feature
    feature_type: ability
    name: Mace Lariat
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Each enemy
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage; push 1; M < 1 dazed (save ends)
        tier2: 10 damage; push 3; M < 2 dazed (save ends)
        tier3: 13 damage; push 5; M < 3 dazed (save ends)
  - type: feature
    feature_type: ability
    name: Lockdown
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Ranged
    usage: Maneuver
    distance: Self and ranged 10
    target: Self and three allies
    effects:
      - name: Effect
        effect: Each target moves up to their speed and can use the Grab maneuver, which
          gains an edge.
  - type: feature
    feature_type: ability
    name: Courtesy Call
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: One creature
    trigger: The target obtains a tier 1 outcome on one power roll.
    effects:
      - name: Effect
        effect: The target has a double edge on their next power roll before the end of
          the encounter.
  - type: feature
    feature_type: ability
    name: Close In
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target moves up to their speed. Each enemy adjacent to a target
          after this move makes an Intuition test.
        tier1: Frightened of the warleader (save ends)
        tier2: Frightened of the warleader (EoT)
        tier3: No effect
  - type: feature
    feature_type: ability
    name: Familial Reinforcements
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: Self
    effects:
      - name: Effect
        effect: The warleader shifts up to their speed, and four orc blitzers appear in
          unoccupied spaces within distance.
  - type: feature
    feature_type: ability
    name: I'll Do This Myself
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Three times in succession, the warleader shifts up to their speed and
          can use Mace Lariat.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the warleader can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Relentless
    icon: ⭐️
    effects:
      - effect: If the warleader is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the warleader is reduced to 1 Stamina instead.
~~~