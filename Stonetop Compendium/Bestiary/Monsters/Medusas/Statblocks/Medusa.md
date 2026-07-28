---
agility: 4
ancestry:
- Accursed
- Humanoid
- Medusa
ev: '84'
file_basename: Medusa
file_dpath: Monsters/Medusas/Statblocks
free_strike: 8
intuition: 0
item_id: medusa
item_index: '01'
item_name: Medusa
level: 5
might: 2
presence: 0
reason: 0
roles:
- Solo
scc:
- mcdm.monsters.v1:monster.medusas.statblock:medusa
scdc:
- 1.1.1:2.32.1:01
size: 1M
source: mcdm.monsters.v1
speed: 10
stability: 5
stamina: '420'
type: monster/medusas/statblock
---

~~~ds-statblock
type: statblock
name: Medusa
level: 5
roles:
  - Solo
ancestry:
  - Accursed
  - Humanoid
  - Medusa
ev: "84"
stamina: "420"
speed: 10
size: 1M
stability: 5
free_strike: 8
might: 2
agility: 4
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the medusa can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The medusa can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: ability
    name: Snake Bites
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
      - roll: Power Roll + 4
        tier1: 11 damage; M < 2 slowed (save ends)
        tier2: 16 damage; M < 3 slowed (save ends)
        tier3: 19 damage; M < 4 slowed (save ends)
  - type: feature
    feature_type: ability
    name: Damning Gaze
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage; push 3
        tier2: 16 damage; push 5
        tier3: 19 damage; push 7
      - cost: 3 Malice
        effect: The medusa targets two additional creatures or objects.
  - type: feature
    feature_type: ability
    name: Petrify
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: M < 2 restrained (save ends)
        tier2: M < 3 restrained (save ends)
        tier3: Slowed (save ends); or if M < 4 restrained (save ends)
      - name: Effect
        effect: A target with cover reduces the potency by 1, while a slowed target
          increases the potency by 1. A target restrained this way magically
          begins to turn to stone, and a target who ends two consecutive turns
          restrained this way is petrified.
  - type: feature
    feature_type: ability
    name: Nimble Escape
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The medusa shifts up to 3 squares and can attempt to hide even if
          observed.
  - type: feature
    feature_type: ability
    name: Venomous Spit
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: A creature within distance deals damage to the medusa.
    effects:
      - roll: Power Roll + 4
        tier1: 13 acid damage
        tier2: 18 acid damage
        tier3: 22 acid damage
  - type: feature
    feature_type: trait
    name: Cunning Edge
    icon: ⭐️
    effects:
      - effect: The medusa gains an edge on power rolls against any creature who is
          restrained or slowed by Petrify.
  - type: feature
    feature_type: trait
    name: Many Peering Eyes
    icon: ⭐️
    effects:
      - effect: The medusa can't be flanked.
  - type: feature
    feature_type: ability
    name: Mass Petrify
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Magic
      - Ranged
    usage: "-"
    distance: Ranged 50
    target: Each enemy
    effects:
      - name: Effect
        effect: The medusa can use Petrify against each target without spending Malice.
          A target who doesn't have cover increases the potency by 1.
  - type: feature
    feature_type: ability
    name: Serpent Wings
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The medusa temporarily manifests wings and flies up to their speed
          without provoking opportunity attacks. During or after this movement,
          they can use Snake Bites and Damning Gaze once each.
  - type: feature
    feature_type: ability
    name: Stone Puppets
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 10 burst
    target: Special
    effects:
      - roll: Power Roll + 4
        tier1: 8 acid damage; P < 3 weakened (save ends)
        tier2: 13 acid damage; P < 4 weakened (save ends)
        tier3: 17 acid damage; P < 5 weakened (save ends)
      - name: Effect
        effect: As a free triggered action, each stone statue and creature restrained or
          slowed by Petrify within distance moves up to their speed and uses a
          signature ability that gains an edge, targeting an enemy of the
          medusa's choice. A stone statue without its own statistics has speed 5
          and uses the medusa's free strike.
~~~