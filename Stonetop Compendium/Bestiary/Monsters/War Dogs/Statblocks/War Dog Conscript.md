---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 3 for four minions
file_basename: War Dog Conscript
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 1
intuition: 0
item_id: war-dog-conscript
item_index: '15'
item_name: War Dog Conscript
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-conscript
scdc:
- 1.1.1:2.51.1:15
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Conscript
level: 1
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 3 for four minions
stamina: "4"
speed: 7
size: 1M
stability: 0
free_strike: 1
with_captain: +1 damage bonus to strikes
might: 2
agility: 0
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Blade
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
      - name: Effect
        effect: If used with the Charge main action, this ability gains an edge.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the conscript is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d3 damage to each adjacent enemy and object.
~~~