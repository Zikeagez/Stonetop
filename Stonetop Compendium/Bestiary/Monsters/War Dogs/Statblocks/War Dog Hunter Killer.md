---
agility: 5
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 12 for four minions
file_basename: War Dog Hunter Killer
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 5
intuition: 5
item_id: war-dog-hunter-killer
item_index: '11'
item_name: War Dog Hunter-Killer
level: 10
might: 1
presence: 2
reason: 3
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-hunter-killer
scdc:
- 1.1.1:2.51.1:11
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '14'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog Hunter-Killer
level: 10
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 12 for four minions
stamina: "14"
speed: 5
size: 1M
stability: 0
free_strike: 5
with_captain: +4 damage bonus to strikes
might: 1
agility: 5
reason: 3
intuition: 5
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Fuse-Iron Rocket
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
      - roll: Power Roll + 5
        tier1: 5 damage; push 2
        tier2: 8 damage; push 3
        tier3: 10 damage; push 4
      - name: Effect
        effect: Each enemy adjacent to the target before the forced movement takes 5
          fire damage.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the hunter-killer is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
~~~