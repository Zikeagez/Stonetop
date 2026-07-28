---
agility: 5
ancestry:
- Accursed
- Humanoid
- Minotaur
- Swarm
ev: 12 for four minions
file_basename: Minotaur Stampede
file_dpath: Monsters/Minotaurs/Statblocks
free_strike: 4
intuition: 2
item_id: minotaur-stampede
item_index: '03'
item_name: Minotaur Stampede
level: 10
might: 5
presence: -1
reason: 0
roles:
- Minion Defender
scc:
- mcdm.monsters.v1:monster.minotaurs.statblock:minotaur-stampede
scdc:
- 1.1.1:2.21.1:03
size: '4'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '17'
type: monster/minotaurs/statblock
---

~~~ds-statblock
type: statblock
name: Minotaur Stampede
level: 10
roles:
  - Minion Defender
ancestry:
  - Accursed
  - Humanoid
  - Minotaur
  - Swarm
ev: 12 for four minions
stamina: "17"
speed: 8
size: "4"
stability: 2
free_strike: 4
with_captain: Gain an edge on strikes
might: 5
agility: 5
reason: 0
intuition: 2
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Bull Rush
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        tier1: 4 damage
        tier2: 7 damage; prone
        tier3: 9 damage; prone; M < 5 can't stand (save ends)
      - name: Effect
        effect: If this ability is used as part of the Charge main action, each creature
          the stampede moves through who has M < 4 is knocked prone.
  - type: feature
    feature_type: trait
    name: Swarm
    icon: ⭐️
    effects:
      - effect: The stampede can move through spaces as if they were a size 2 creature,
          and can occupy other creatures' spaces. At the start of each of the
          stampede's turns, they can make a free strike against each creature
          whose space they share.
~~~