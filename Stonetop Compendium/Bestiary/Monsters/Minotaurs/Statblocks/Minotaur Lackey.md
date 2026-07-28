---
agility: 4
ancestry:
- Accursed
- Humanoid
- Minotaur
ev: 10 for four minions
file_basename: Minotaur Lackey
file_dpath: Monsters/Minotaurs/Statblocks
free_strike: 3
intuition: 1
item_id: minotaur-lackey
item_index: '01'
item_name: Minotaur Lackey
level: 8
might: 3
presence: -1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.minotaurs.statblock:minotaur-lackey
scdc:
- 1.1.1:2.21.1:01
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '13'
type: monster/minotaurs/statblock
---

~~~ds-statblock
type: statblock
name: Minotaur Lackey
level: 8
roles:
  - Minion Harrier
ancestry:
  - Accursed
  - Humanoid
  - Minotaur
ev: 10 for four minions
stamina: "13"
speed: 8
size: "2"
stability: 2
free_strike: 3
with_captain: +2 bonus to speed
might: 3
agility: 4
reason: 0
intuition: 1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Horn Vault
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
      - roll: Power Roll + 4
        tier1: 3 damage
        tier2: 6 damage; slide 1
        tier3: 8 damage; slide 3
      - name: Effect
        effect: A target who is force moved into an obstacle and has M < 3 is bleeding
          (save ends).
  - type: feature
    feature_type: trait
    name: Minotaur Sense
    icon: ⭐️
    effects:
      - effect: The lackey can't obtain less than a tier 2 outcome when making tests to
          navigate, search, or seek.
~~~