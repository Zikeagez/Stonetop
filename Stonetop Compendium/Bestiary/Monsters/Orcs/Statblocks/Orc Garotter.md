---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '6'
file_basename: Orc Garotter
file_dpath: Monsters/Orcs/Statblocks
free_strike: 4
intuition: 1
item_id: orc-garotter
item_index: '13'
item_name: Orc Garotter
level: 1
might: 1
presence: -1
reason: 0
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-garotter
scdc:
- 1.1.1:2.16.1:13
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Garotter
level: 1
roles:
  - Platoon Ambusher
ancestry:
  - Humanoid
  - Orc
ev: "6"
stamina: "30"
speed: 5
size: 1L
stability: 0
free_strike: 4
might: 1
agility: 2
reason: 0
intuition: 1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Dagger Feint
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
      - roll: Power Roll + 2
        tier1: 6 damage; the garroter can shift 1 square
        tier2: 9 damage; the garroter shifts up to 2 squares
        tier3: 12 damage; the garroter shifts up to 3 squares
      - name: Effect
        effect: If this ability gains an edge or has a double edge, it deals an extra 4
          damage.
  - type: feature
    feature_type: ability
    name: Strangle
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 9 damage; I < 1 dazed (save ends)
        tier3: 12 damage; grabbed; I < 2 dazed (save ends)
      - name: Effect
        effect: While grabbed this way, a target can't communicate or use magic
          abilities.
  - type: feature
    feature_type: ability
    name: Chroma Cloak
    icon: 👤
    cost: 1 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: "-"
    target: "-"
    effects:
      - effect: The garroter turns invisible until the end of their turn. This
          invisibility ends early if they take damage or use an ability.
  - type: feature
    feature_type: trait
    name: Relentless
    icon: ⭐️
    effects:
      - effect: If the garroter is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the garroter is reduced to 1 Stamina instead.
~~~