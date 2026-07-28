---
agility: 2
ancestry:
- Basilisk
- Beast
ev: '12'
file_basename: Basilisk Tonguesnapper
file_dpath: Monsters/Basilisks/Statblocks
free_strike: 4
intuition: -1
item_id: basilisk-tonguesnapper
item_index: '02'
item_name: Basilisk Tonguesnapper
level: 1
might: 1
presence: -1
reason: -3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster.basilisks.statblock:basilisk-tonguesnapper
scdc:
- 1.1.1:2.44.1:02
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '40'
type: monster/basilisks/statblock
---

~~~ds-statblock
type: statblock
name: Basilisk Tonguesnapper
level: 1
roles:
  - Elite Hexer
ancestry:
  - Basilisk
  - Beast
ev: "12"
stamina: "40"
immunities:
  - Acid 2
  - Poison 2
speed: 8
size: "2"
stability: 2
free_strike: 4
might: 1
agility: 2
reason: -3
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Prehensile Tongue
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 8 acid damage; pull 1
        tier2: 10 acid damage; pull 2
        tier3: 14 acid damage; pull 3
      - name: Effect
        effect: This ability can pull targets restrained by Petrifying Eye Beams, and
          ignores stability if it does so.
      - cost: 3 Malice
        effect: The tonguesnapper targets two additional creatures or objects.
  - type: feature
    feature_type: ability
    name: Petrifying Eye Beams
    icon: 🔳
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 5 x 2 line within 1
    target: Special
    effects:
      - name: Special
        effect: The area extends from both the tonguesnapper's eyes, and this ability
          targets the first creature without cover on either side of the area.
      - roll: Power Roll + 2
        tier1: A < 0 restrained (save ends)
        tier2: A < 1 restrained (save ends)
        tier3: Slowed (save ends); or if A < 2 restrained (save ends)
      - name: Effect
        effect: If a target is already slowed, the potency increases by 1 for that
          target. A target restrained this way magically begins to turn to
          stone, and a target who ends two consecutive turns restrained this way
          is petrified. A target restrained this way or a creature adjacent to
          them can use a main action to cut encroaching stone from the target's
          body, dealing 8 damage to the target that can't be reduced in any way
          and ending this effect.
  - type: feature
    feature_type: ability
    name: Wink
    icon: ⚔️
    cost: 2 Malice
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 8 corruption damage; R < 0 dazed (save ends)
        tier2: 10 corruption damage; R < 1 dazed (save ends)
        tier3: 14 corruption damage; R < 2 dazed and slowed (save ends)
      - name: Effect
        effect: A creature dazed this way can't benefit from edges or double edges and
          can't gain or use surges.
  - type: feature
    feature_type: ability
    name: Neurotoxin Splash
    icon: ❗️
    keywords:
      - Area
    usage: Triggered action
    distance: 2 burst
    target: Each enemy in the area
    trigger: The tonguesnapper takes damage from a melee ability.
    effects:
      - name: Effect
        effect: Each target takes 4 acid damage. Any target who has M < 2 is also slowed
          (save ends).
  - type: feature
    feature_type: trait
    name: Petrifying Fumes
    icon: ⭐️
    effects:
      - effect: Any creature who starts their turn adjacent to the tonguesnapper and has
          M < 1 is slowed (save ends).
~~~