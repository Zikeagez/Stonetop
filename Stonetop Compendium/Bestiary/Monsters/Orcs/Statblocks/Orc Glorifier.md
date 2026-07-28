---
agility: 1
ancestry:
- Humanoid
- Orc
ev: 3 for four minions
file_basename: Orc Glorifier
file_dpath: Monsters/Orcs/Statblocks
free_strike: 1
intuition: 0
item_id: orc-glorifier
item_index: '02'
item_name: Orc Glorifier
level: 1
might: 0
presence: 2
reason: 0
roles:
- Minion Controller
scc:
- mcdm.monsters.v1:monster.orcs.statblock:orc-glorifier
scdc:
- 1.1.1:2.16.1:02
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '3'
type: monster/orcs/statblock
---

~~~ds-statblock
type: statblock
name: Orc Glorifier
level: 1
roles:
  - Minion Controller
ancestry:
  - Humanoid
  - Orc
ev: 3 for four minions
stamina: "3"
speed: 6
size: 1M
stability: 0
free_strike: 1
with_captain: +5 bonus to ranged distance
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Call to Victory
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 sonic damage
        tier2: 2 sonic damage; P < 1 slowed (save ends)
        tier3: 3 sonic damage; P < 2 slowed (save ends)
      - name: Effect
        effect: Allies gain an edge on melee strikes against the target until the
          glorifier and each other glorifier in their squad are killed.
  - type: feature
    feature_type: trait
    name: Bloodfire Burn
    icon: ⭐️
    effects:
      - effect: If the glorifier is reduced to 0 Stamina, they can make a free strike
          before dying.
~~~