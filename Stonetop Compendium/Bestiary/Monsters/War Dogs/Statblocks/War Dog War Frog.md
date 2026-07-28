---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 6 for four minions
file_basename: War Dog War Frog
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 2
item_id: war-dog-war-frog
item_index: '41'
item_name: War Dog War Frog
level: 4
might: -1
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster.war-dogs.statblock:war-dog-war-frog
scdc:
- 1.1.1:2.51.1:41
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '8'
type: monster/war-dogs/statblock
---

~~~ds-statblock
type: statblock
name: War Dog War Frog
level: 4
roles:
  - Minion Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 6 for four minions
stamina: "8"
immunities:
  - Poison 4
speed: 5
movement: Climb, swim
size: 1S
stability: 0
free_strike: 3
with_captain: +2 bonus to speed
might: -1
agility: 3
reason: 0
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Poisoned Dagger
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 4
    target: One creature per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 poison damage
        tier2: 5 poison damage
        tier3: 7 poison damage
      - name: Effect
        effect: The war frog can jump 3 squares before or after making the strike. If
          they end this jump in cover or concealment, they can attempt to hide.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the war frog is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~