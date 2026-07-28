---
agility: 2
ancestry:
- Giant
- Troll
ev: 11 for four minions
file_basename: Troll Ravager
file_dpath: Monsters/Trolls/Statblocks
free_strike: 4
intuition: 1
item_id: troll-ravager
item_index: '05'
item_name: Troll Ravager
level: 9
might: 4
presence: 1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.trolls.statblock:troll-ravager
scdc:
- 1.1.1:2.53.1:05
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '15'
type: monster/trolls/statblock
---

~~~ds-statblock
type: statblock
name: Troll Ravager
level: 9
roles:
  - Minion Harrier
ancestry:
  - Giant
  - Troll
ev: 11 for four minions
stamina: "15"
weaknesses:
  - Acid 5
  - fire
speed: 8
size: "2"
stability: 2
free_strike: 4
with_captain: +2 bonus to speed
might: 4
agility: 2
reason: 0
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Dine and Dash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        tier1: 4 damage; the ravager can shift 1 square
        tier2: 6 damage; the ravager shifts up to 2 squares
        tier3: 8 damage; the ravager shifts up to 3 squares
      - name: Effect
        effect: The ravager's squad's Stamina pool regains Stamina equal to half the
          damage dealt.
  - type: feature
    feature_type: trait
    name: Group Appetite
    icon: ⭐️
    effects:
      - effect: The ravager dies only if their squad's Stamina pool is reduced to 0
          Stamina by acid or fire damage, if they end their turn with 0 Stamina
          in their squad's Stamina pool, or if they take acid or fire damage
          while their squad's Stamina pool is at 0 Stamina.
~~~