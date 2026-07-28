---
agility: 3
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 7
intuition: 0
item_id: rival-shadow
item_index: '07'
item_name: Rival Shadow
level: 5
might: 0
presence: 2
reason: 1
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster.rivals.2nd echelon.statblock:rival-shadow
scdc:
- 1.1.1:2.5.2.1:07
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '140'
type: monster/rivals/2nd echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Shadow
level: 5
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "140"
speed: 7
size: 1M
stability: 1
free_strike: 7
might: 0
agility: 3
reason: 1
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Ambuscade
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
      - roll: Power Roll + 3
        tier1: 10 damage
        tier2: 15 damage; A < 2 bleeding (save ends)
        tier3: 18 damage; A < 3 bleeding (save ends)
      - cost: 1 Malice
        effect: The shadow can teleport up to 6 squares, then can attempt to hide.
  - type: feature
    feature_type: ability
    name: Poison the Blade
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The shadow coats their weapon with poison. They gain an edge on their
          next strike, and any potency for that strike increases by 1.
  - type: feature
    feature_type: trait
    name: Exploit Opening
    icon: ⭐️
    effects:
      - effect: The shadow deals an extra 7 damage to any bleeding target.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
~~~