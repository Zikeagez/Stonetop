---
agility: 1
ancestry:
- Devil
- Infernal
ev: 7 for four minions
file_basename: Devil Notary
file_dpath: Monsters/Devils/Statblocks
free_strike: 3
intuition: 1
item_id: devil-notary
item_index: '07'
item_name: Devil Notary
level: 5
might: 0
presence: 2
reason: 3
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.devils.statblock:devil-notary
scdc:
- 1.1.1:2.39.1:07
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '8'
type: monster/devils/statblock
---

~~~ds-statblock
type: statblock
name: Devil Notary
level: 5
roles:
  - Minion Hexer
ancestry:
  - Devil
  - Infernal
ev: 7 for four minions
stamina: "8"
immunities:
  - Fire 5
speed: 6
size: 1M
stability: 0
free_strike: 3
with_captain: +5 bonus to ranged distance
might: 0
agility: 1
reason: 3
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Importunity
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 fire damage
        tier2: 5 fire damage; R < 2 the target takes a bane on their next strike
        tier3: 6 fire damage; R < 3 the target takes a bane on their next strike
      - name: Effect
        effect: One non-minion devil within 5 squares of the notary gains an edge on
          their next strike.
  - type: feature
    feature_type: trait
    name: True Name
    icon: ⭐️
    effects:
      - effect: If a creature within 10 squares speaks the notary's true name, the
          notary loses their fire immunity and any nondamaging effects of their
          signature ability until the end of the encounter.
~~~