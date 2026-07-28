---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '6'
file_basename: Wode Elf Sentry
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wode-elf-sentry
item_index: '04'
item_name: Wode Elf Sentry
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster.elves-wode.statblock:wode-elf-sentry
scdc:
- 1.1.1:2.28.1:04
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster/elves-wode/statblock
---

~~~ds-statblock
type: statblock
name: Wode Elf Sentry
level: 1
roles:
  - Platoon Support
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "6"
stamina: "30"
speed: 7
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Tracer Longbow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 7 damage
        tier3: 9 damage; the target is marked (save ends)
      - name: Effect
        effect: Allies gain an edge on abilities against a target marked by any wode
          elf.
      - cost: 3 Malice
        effect: The sentry targets two additional creatures or objects.
  - type: feature
    feature_type: ability
    name: Death Blossom
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    usage: Maneuver
    distance: 5 burst
    target: Each marked enemy
    effects:
      - name: Effect
        effect: Each target takes 3 damage.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the sentry that would take a bane from cover or
          concealment have a double bane instead.
~~~