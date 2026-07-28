---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '10'
file_basename: Orc Juggernaut
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: -1
item_id: orc-juggernaut
item_index: '15'
item_name: Orc Juggernaut
level: 3
might: 2
presence: 2
reason: -1
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-juggernaut
scdc:
- 1.1.1:2.16.1:15
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '60'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Juggernaut
level: 3
roles:
  - Platoon Brute
ancestry:
  - Humanoid
  - Orc
ev: "10"
stamina: "60"
speed: 6
size: 1L
stability: 0
free_strike: 5
might: 2
agility: 2
reason: -1
intuition: -1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Haymaker Greataxe
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
        tier1: 7 damage
        tier2: 11 damage; prone
        tier3: 14 damage; prone; M < 2 bleeding (save ends)
      - name: Effect
        effect: A target who is already prone takes an extra 6 damage.
  - type: feature
    feature_type: ability
    name: Hrraaaaaagh!
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: The juggernaut takes damage.
    effects:
      - name: Effect
        effect: The juggernaut moves up to their speed and can make a free strike.
  - type: feature
    feature_type: trait
    name: Blood in the Water
    icon: ⭐️
    effects:
      - effect: Whenever the juggernaut willingly moves, they can move 3 additional
          squares if they end their movement closer to a prone creature.
  - type: feature
    feature_type: trait
    name: Relentless
    icon: ⭐️
    effects:
      - effect: If the juggernaut is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the juggernaut is reduced to 1 Stamina instead.
~~~