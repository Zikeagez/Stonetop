---
agility: 0
ancestry:
- Horror
- Voiceless Talker
ev: 8 for four minions
file_basename: Voiceless Talker Graywarper
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 3
intuition: 1
item_id: voiceless-talker-graywarper
item_index: '01'
item_name: Voiceless Talker Graywarper
level: 6
might: -1
presence: 1
reason: 3
roles:
- Minion Controller
scc:
- mcdm.monsters.v1:monster.voiceless-talkers.statblock:voiceless-talker-graywarper
scdc:
- 1.1.1:2.46.1:01
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '9'
type: monster/voiceless-talkers/statblock
---

~~~ds-statblock
type: statblock
name: Voiceless Talker Graywarper
level: 6
roles:
  - Minion Controller
ancestry:
  - Horror
  - Voiceless Talker
ev: 8 for four minions
stamina: "9"
speed: 5
size: 1M
stability: 0
free_strike: 3
with_captain: +2 bonus to Stamina
might: -1
agility: 0
reason: 3
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Phase Chant
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 8
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 3 psychic damage
        tier2: 5 psychic damage; slide 2
        tier3: 7 psychic damage; slide 4
  - type: feature
    feature_type: trait
    name: Psionic Conductor
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the
          graywarper uses a psionic ability, they can do so as if they were in
          the graywarper's space.
~~~