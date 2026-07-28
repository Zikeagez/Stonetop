---
agility: 2
ancestry:
- Human
- Humanoid
ev: '12'
file_basename: Human Blackguard
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 0
item_id: human-blackguard
item_index: '10'
item_name: Human Blackguard
level: 1
might: 3
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-blackguard
scdc:
- 1.1.1:2.20.1:10
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '80'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Blackguard
level: 1
roles:
  - Leader
ancestry:
  - Human
  - Humanoid
ev: "12"
stamina: "80"
immunities:
  - Corruption 2
  - psychic 2
speed: 5
size: 1M
stability: 2
free_strike: 4
might: 3
agility: 2
reason: 2
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Zweihander Swing
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 3 damage; M < 1 slowed (save ends)
        tier2: 6 damage; M < 2 slowed (save ends)
        tier3: 8 damage; M < 3 slowed (save ends)
      - name: Effect
        effect: One ally within 10 squares can make a free strike.
      - cost: 1 Malice
        effect: One ally within 10 squares can use their signature ability instead.
  - type: feature
    feature_type: ability
    name: You!
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One enemy
    effects:
      - name: Effect
        effect: The target is marked until the start of the blackguard's next turn. The
          blackguard and each of their allies gain an edge on abilities used
          against targets marked by the blackguard.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the blackguard can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The blackguard ignores concealment if it's granted by a supernatural
          effect.
  - type: feature
    feature_type: ability
    name: Parry!
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: Self or one ally
    trigger: A creature makes a strike against the blackguard or an ally adjacent to
      them.
    effects:
      - name: Effect
        effect: The damage is halved.
  - type: feature
    feature_type: ability
    name: Advance!
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The blackguard shifts up to their speed. During or after this movement,
          they can use their Zweihander Swing twice.
  - type: feature
    feature_type: ability
    name: Back!
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The blackguard slides each target up to 5 squares.
  - type: feature
    feature_type: ability
    name: I Can Throw My Blade and So Should You!
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
      - Ranged
      - Weapon
    usage: "-"
    distance: 3 cube within 5
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The blackguard uses their Zweihander Swing against each target. Each
          ally within 5 squares of the area can then make a free strike against
          a target (one target per ally).
~~~