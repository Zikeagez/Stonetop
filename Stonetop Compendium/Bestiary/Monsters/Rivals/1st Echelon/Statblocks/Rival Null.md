---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Null
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 2
item_id: rival-null
item_index: '01'
item_name: Rival Null
level: 2
might: 0
presence: 0
reason: 1
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster.rivals.1st echelon.statblock:rival-null
scdc:
- 1.1.1:2.5.1.1:01
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '80'
type: monster/rivals/1st echelon/statblock
---

~~~ds-statblock
type: statblock
name: Rival Null
level: 2
roles:
  - Elite Harrier
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "80"
speed: 7
size: 1M
stability: 3
free_strike: 5
might: 0
agility: 2
reason: 1
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Nimble Step
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
      - roll: Power Roll + 2
        tier1: 7 damage; the null shifts up to 2 squares
        tier2: 10 damage; the null shifts up to 3 squares
        tier3: 13 damage; the null shifts up to 4 squares
  - type: feature
    feature_type: ability
    name: Numb
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    usage: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; R < 0 slowed (EoT)
        tier2: 10 damage; R < 1 slowed (EoT)
        tier3: 13 damage; R < 2 dazed and slowed (EoT)
  - type: feature
    feature_type: trait
    name: Inertial Shield
    icon: ⭐️
    effects:
      - effect: The first time each round that the null is targeted by a damage-dealing
          strike, they halve the damage.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the null chooses one creature within their
          line of effect. Both the null and the creature can add a d3 roll to
          power rolls they make against each other.
~~~