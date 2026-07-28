---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 12 for four minions
file_basename: War Dog Blood Jumper
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 3
item_id: war-dog-blood-jumper
item_index: 08
item_name: War Dog Blood Jumper
level: 10
might: 5
presence: 2
reason: 2
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-blood-jumper
scdc:
- 1.1.1:2.51.1:08
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '15'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Blood Jumper
level: 10
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 12 for four minions
stamina: "15"
speed: 7
movement: Fly
size: 1M
stability: 2
free_strike: 4
with_captain: +3 bonus to speed
might: 5
agility: 4
reason: 2
intuition: 3
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Jumplance
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        tier1: 4 damage
        tier2: 7 damage
        tier3: 9 damage; A < 4 bleeding (save ends)
  - type: feature
    feature_type: trait
    name: Drop Troop
    icon: ⭐️
    effects:
      - effect: If the jumper doesn't end their turn on the ground, they fall prone.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the jumper is reduced to 0 Stamina, their loyalty collar explodes,
          dealing 3d6 damage to each adjacent enemy and object.
~~~