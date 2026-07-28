---
agility: -2
ancestry:
- Undead
- Soulless
ev: '9'
file_basename: Waxen
file_dpath: Monsters/Undead/Statblocks
free_strike: 4
intuition: 1
item_id: waxen
item_index: '12'
item_name: Waxen
level: 7
might: 4
presence: -2
reason: -4
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster.undead.statblock:waxen
scdc:
- 1.1.1:2.8.1:12
size: 1M
source: mcdm.monsters.v1
speed: 4
stability: 2
stamina: '40'
type: monster/undead/statblock
---

~~~ds-statblock
type: statblock
name: Waxen
level: 7
roles:
  - Horde Artillery
ancestry:
  - Undead
  - Soulless
ev: "9"
stamina: "40"
immunities:
  - Corruption 7
  - poison 7
speed: 4
size: 1M
stability: 2
free_strike: 4
might: 4
agility: -2
reason: -4
intuition: 1
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Wax Fling
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 8 damage
        tier2: 11 damage
        tier3: 12 damage; A < 4 slowed (save ends)
      - name: Effect
        effect: If a target made slowed this way is already slowed, they are instead
          restrained (save ends).
  - type: feature
    feature_type: ability
    name: Erupt
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: If the waxen is ignited (see Burn Bright), they shift up to their speed
          before using this ability. Each target makes an **Agility test**.
        tier1: 10 damage
        tier2: 8 damage
        tier3: 5 damage
      - effect: The waxen is then destroyed and the area is difficult terrain for
          enemies.
  - type: feature
    feature_type: trait
    name: Burn Bright
    icon: ⭐️
    effects:
      - effect: If the waxen takes fire damage, they ignite. While ignited, the waxen
          takes 4 fire damage at the start of each of their turns and their
          strikes deal an extra 4 fire damage.
~~~