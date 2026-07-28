---
agility: 3
ancestry:
- Abyssal
- Demon
ev: 6 for four minions
file_basename: Wobalas
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 2
item_id: wobalas
item_index: '02'
item_name: Wobalas
level: 4
might: 1
presence: 1
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster.demons.statblock:wobalas
scdc:
- 1.1.1:2.35.1:02
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '7'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Wobalas
level: 4
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Demon
ev: 6 for four minions
stamina: "7"
weaknesses:
  - Holy 5
speed: 6
size: 1M
stability: 0
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 1
agility: 3
reason: 1
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Despair Bolt
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 20
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        tier1: 3 psychic damage
        tier2: 5 psychic damage
        tier3: 7 psychic damage
      - name: Effect
        effect: The target takes a bane on their next strike. If the target is winded,
          they have a double bane on their next strike instead.
~~~