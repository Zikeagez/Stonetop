---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Hijack
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 2
item_id: time-raider-hijack
item_index: '02'
item_name: Time Raider Hijack
level: 3
might: 0
presence: 1
reason: 2
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster.time-raiders.statblock:time-raider-hijack
scdc:
- 1.1.1:2.18.1:02
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '50'
type: monster/time-raiders/statblock
---

~~~ds-statblock
type: statblock
name: Time Raider Hijack
level: 3
roles:
  - Platoon Ambusher
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "50"
immunities:
  - Psychic 3
speed: 6
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 2
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Golden Sickles
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage
        tier3: 14 damage; A < 2 bleeding (save ends)
      - name: Effect
        effect: The hijack is hidden from any creature who is bleeding from this ability
          until that condition ends.
  - type: feature
    feature_type: ability
    name: Psi-Sickle
    icon: 🏹
    keywords:
      - Psionic
      - Ranged
      - Weapon
    usage: Maneuver
    distance: Ranged 5
    target: One creature or object
    effects:
      - name: Effect
        effect: The hijack psychically latches their sickle onto the target and closes
          the distance between them. If the target is larger than the hijack,
          the hijack moves adjacent to the target. Otherwise, the target is
          pulled up to 4 squares toward the hijack.
  - type: feature
    feature_type: trait
    name: Foresight
    icon: ⭐️
    effects:
      - effect: The hijack doesn't take a bane on strikes against creatures with
          concealment.
~~~