---
agility: 2
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Rogue
file_dpath: Monsters/Humans/Statblocks
free_strike: 2
intuition: 0
item_id: human-rogue
item_index: '01'
item_name: Human Rogue
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster.humans.statblock:human-rogue
scdc:
- 1.1.1:2.20.1:01
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster/humans/statblock
---

~~~ds-statblock
type: statblock
name: Human Rogue
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Human
  - Humanoid
ev: 3 for four minions
stamina: "4"
immunities:
  - Corruption 1
  - psychic 1
speed: 7
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Concealed Dagger
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
      - name: Effect
        effect: If the rogue is disguised or hidden when they use this ability, it deals
          an extra 3 damage.
  - type: feature
    feature_type: trait
    name: Supernatural Insight
    icon: ⭐️
    effects:
      - effect: The rogue ignores concealment if it's granted by a supernatural effect.
~~~