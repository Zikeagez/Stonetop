---
agility: 2
ancestry:
- Elemental
- High Elf
ev: '6'
file_basename: Ceramic Horse
file_dpath: Monsters/Elves High/Statblocks
free_strike: 3
intuition: 0
item_id: ceramic-horse
item_index: '11'
item_name: Ceramic Horse
level: 1
might: 2
presence: 1
reason: 0
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster.elves-high.statblock:ceramic-horse
scdc:
- 1.1.1:2.14.1:11
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 2
stamina: '30'
type: monster/elves-high/statblock
---

~~~ds-statblock
type: statblock
name: Ceramic Horse
level: 1
roles:
  - Platoon Mount
ancestry:
  - Elemental
  - High Elf
ev: "6"
stamina: "30"
speed: 10
size: "2"
stability: 2
free_strike: 3
might: 2
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Elemental Charge
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 7 fire damage
        tier3: 9 lightning damage; M < 2 prone
  - type: feature
    feature_type: ability
    name: Stomp
    icon: ❇️
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 5 damage
        tier3: 7 damage
      - name: Effect
        effect: Any target who is prone takes an extra 2 damage.
  - type: feature
    feature_type: ability
    name: Buck
    icon: 👤
    cost: 2 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: The horse's rider
    effects:
      - name: Effect
        effect: The horse vertical slides the target up to 3 squares, ignoring
          stability. The target can use a ranged ability at any point during
          this forced movement, and takes no damage if they then fall.
  - type: feature
    feature_type: trait
    name: Shared Otherworldly Grace
    icon: ⭐️
    effects:
      - effect: If the ceramic horse's rider has the Otherworldly Grace trait, the
          ceramic horse also has that trait.
~~~