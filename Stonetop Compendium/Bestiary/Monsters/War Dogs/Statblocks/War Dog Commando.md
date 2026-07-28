---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 3 for four minions
file_basename: War Dog Commando
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-commando
item_index: '22'
item_name: War Dog Commando
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-commando
scdc:
- 1.1.1:2.51.1:22
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '4'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Commando
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 3 for four minions
stamina: "4"
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Daggers
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
      - name: Effect
        effect: After using this ability, the commando can attempt to hide even if
          observed.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the commando is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d3 damage to each adjacent enemy and object.
~~~