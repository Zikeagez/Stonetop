---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 9 for four minions
file_basename: War Dog Shriketroop
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 1
item_id: war-dog-shriketroop
item_index: '06'
item_name: War Dog Shriketroop
level: 7
might: 1
presence: 1
reason: 3
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-shriketroop
scdc:
- 1.1.1:2.51.1:06
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Shriketroop
level: 7
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 9 for four minions
stamina: "10"
speed: 5
size: 1M
stability: 0
free_strike: 4
with_captain: Gain an edge on strikes
might: 1
agility: 4
reason: 3
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Canis Shrikegun
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        tier1: 4 damage
        tier2: 7 damage
        tier3: 8 damage; I < 3 the target is frightened of all shriketroops (EoT)
      - name: Effect
        effect: The target must move their speed in a straight line away from the
          shriketroop.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the shriketroop is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~