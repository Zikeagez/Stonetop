---
agility: 2
ancestry:
- Humanoid
- Orc
ev: 3 for four minions
file_basename: Orc Blitzer
file_dpath: Monsters/Orcs/Statblocks
free_strike: 1
intuition: 0
item_id: orc-blitzer
item_index: '11'
item_name: Orc Blitzer
level: 1
might: 1
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-blitzer
scdc:
- 1.1.1:2.16.1:11
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Blitzer
level: 1
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Orc
ev: 3 for four minions
stamina: "4"
speed: 7
size: 1M
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 1
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Lugged Spear
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
      - name: Effect
        effect: A target who starts their next turn adjacent to three or more blitzers
          takes 3 damage.
  - type: feature
    feature_type: trait
    name: Bloodfire Bur
    icon: ⭐️
    effects:
      - effect: If the blitzer is reduced to 0 Stamina, they can make a free strike
          before dying.
~~~