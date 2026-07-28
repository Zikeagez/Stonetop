---
agility: 4
ancestry:
- Abyssal
- Demon
- Soulraker
ev: 9 for four minions
file_basename: Soulraker Scout
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 0
item_id: soulraker-scout
item_index: '23'
item_name: Soulraker Scout
level: 7
might: 2
presence: -1
reason: 1
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster.demons.statblock:soulraker-scout
scdc:
- 1.1.1:2.35.1:23
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '12'
type: monster/demons/statblock
---

~~~ds-statblock
type: statblock
name: Soulraker Scout
level: 7
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Demon
  - Soulraker
ev: 9 for four minions
stamina: "12"
weaknesses:
  - Holy 5
speed: 7
movement: Fly
size: 1M
stability: 0
free_strike: 3
with_captain: Gain an edge on strikes
might: 2
agility: 4
reason: 1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Soul Stinger
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature per minion
    effects:
      - roll: Power Roll + 4
        tier1: 3 poison damage
        tier2: 6 poison damage; the scout can shift 1 square
        tier3: 7 poison damage; the scout shifts up to 3 squares
  - type: feature
    feature_type: trait
    name: Abyssal Buzzing
    icon: ⭐️
    effects:
      - effect: Any enemy who starts their turn with two or more soulraker minions
          adjacent to them takes 3 sonic damage.
~~~