---
agility: 1
ancestry:
- Abyssal
- Gnoll
ev: 4 for four minions
file_basename: Gnoll Mage Mauler
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 0
item_id: gnoll-mage-mauler
item_index: '10'
item_name: Gnoll Mage Mauler
level: 2
might: 2
presence: 0
reason: -1
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster.gnolls.statblock:gnoll-mage-mauler
scdc:
- 1.1.1:2.6.1:10
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '4'
type: monster/gnolls/statblock
---

~~~ds-statblock
type: statblock
name: Gnoll Mage Mauler
level: 2
roles:
  - Minion Hexer
ancestry:
  - Abyssal
  - Gnoll
ev: 4 for four minions
stamina: "4"
speed: 5
size: 1M
stability: 1
free_strike: 2
with_captain: +2 bonus to melee distance
might: 2
agility: 1
reason: -1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Wizard Ripper
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 acid damage
        tier2: 3 cold damage
        tier3: 5 lightning damage; the target can't use magic abilities (EoT)
      - name: Effect
        effect: The target takes a bane on their next power roll.
  - type: feature
    feature_type: trait
    name: Death Circle
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the mage mauler is
          reduced to 0 Stamina, the mage mauler can move up to their speed.
~~~