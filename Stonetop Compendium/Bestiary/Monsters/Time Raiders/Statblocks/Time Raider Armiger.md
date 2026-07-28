---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Armiger
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 2
item_id: time-raider-armiger
item_index: '03'
item_name: Time Raider Armiger
level: 3
might: 0
presence: 0
reason: 2
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster.time-raiders.statblock:time-raider-armiger
scdc:
- 1.1.1:2.18.1:03
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster/time-raiders/statblock
---

~~~ds-statblock
type: statblock
name: Time Raider Armiger
level: 3
roles:
  - Platoon Defender
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "60"
immunities:
  - Psychic 3
speed: 5
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 2
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Serrated Saber
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 10 damage
        tier3: 13 damage; R < 2 weakened (save ends)
      - cost: 2 Malice
        effect: A creature weakened this way is also bleeding.
  - type: feature
    feature_type: ability
    name: Shared Sickness
    icon: ❗️
    keywords:
      - Psionic
      - Ranged
    usage: Triggered action
    distance: Ranged 20
    target: The triggering creature
    trigger: A creature deals damage to any ally of the armiger who the armiger has
      line of effect to.
    effects:
      - roll: Power Roll + 2
        tier1: 4 psychic damage; R < 0 5 poison damage
        tier2: 6 psychic damage; R < 1 5 poison damage
        tier3: 9 psychic damage; R < 2 5 poison damage
  - type: feature
    feature_type: trait
    name: Foresight
    icon: ⭐️
    effects:
      - effect: The armiger doesn't take a bane on strikes against creatures with
          concealment.
  - type: feature
    feature_type: trait
    name: Kuran'zoi Heraldry
    icon: ⭐️
    effects:
      - effect: Any time raider who starts their turn with line of effect to the armiger
          can end one condition affecting the.
~~~