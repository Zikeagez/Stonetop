---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 6 for four minions
file_basename: War Dog Sweeper
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 2
item_id: war-dog-sweeper
item_index: '34'
item_name: War Dog Sweeper
level: 4
might: 0
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-sweeper
scdc:
- 1.1.1:2.51.1:34
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '8'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Sweeper
level: 4
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 6 for four minions
stamina: "8"
speed: 6
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 3
reason: 0
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Shrikegun Shot
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 3
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 2 damage
        tier2: 4 damage; push 1
        tier3: 6 damage; push 3
      - name: Effect
        effect: Any target within 2 squares of the sweeper takes an extra 3 damage.
  - type: feature
    feature_type: trait
    name: Shrapnel-Laced Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the sweeper is reduced to 0 Stamina, their loyalty collar explodes,
          dealing 1d6 damage to each enemy and object within 2 squares of them.
~~~