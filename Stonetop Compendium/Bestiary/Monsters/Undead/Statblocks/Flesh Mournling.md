---
agility: 1
ancestry:
- Undead
ev: '6'
file_basename: Flesh Mournling
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 2
item_id: flesh-mournling
item_index: '31'
item_name: Flesh Mournling
level: 4
might: 3
presence: -1
reason: 0
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster.undead.statblock:flesh-mournling
scdc:
- 1.1.1:2.8.1:31
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '35'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Flesh Mournling
level: 4
roles:
  - Horde Defender
ancestry:
  - Undead
ev: "6"
stamina: "35"
immunities:
  - Corruption 4
  - poison 4
speed: 6
size: "2"
stability: 2
free_strike: 2
might: 3
agility: 1
reason: 0
intuition: 2
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Multiarm Strike
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage
        tier2: 7 damage
        tier3: 9 damage
      - name: Effect
        effect: The target can't shift until the end of their next turn.
      - cost: 1 Malice
        effect: This ability targets one additional target.
  - type: feature
    feature_type: ability
    name: Horrid Wail
    icon: ❇️
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 2 psychic damage
        tier2: 3 psychic damage; I < 2 frightened (save ends)
        tier3: 4 psychic damage; I < 3 frightened (save ends)
      - name: Effect
        effect: A target who is still frightened this way at the end of the encounter
          can't take a respite activity during their next respite.
  - type: feature
    feature_type: trait
    name: Arise
    icon: ⭐️
    effects:
      - effect: The first time the mournling is reduced to 0 Stamina by damage that
          isn't fire damage or holy damage and their body isn't destroyed, they
          instead have 10 Stamina and fall prone.
  - type: feature
    feature_type: trait
    name: Immutable Form
    icon: ⭐️
    effects:
      - effect: The mournling's shape can't be changed by any external effect.
~~~