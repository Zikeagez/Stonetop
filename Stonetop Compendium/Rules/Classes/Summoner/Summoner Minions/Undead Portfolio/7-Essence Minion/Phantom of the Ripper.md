~~~ds-statblock
type: statblock
name: Phantom of the Ripper
level: .
roles:
  - Minion Ambusher
ancestry:
  - Undead
ev: 7 essence for two minions
speed: 6
size: 1M
stamina: 17|17
movement: Fly, hover
weaknesses:
immunities:
  - Corruption R
  - Poison R
stability: 1
free_strike: 8
might: 0
agility: 4
reason: 0
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: 🏹 Plunge of the Knife 2d10 + R - Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Melee
      - Strike
      - Weapon
    distance: Melee 1
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 8 damage; `I < WEAK` slowed (save ends)
        tier2: 13 damage; `I < AVERAGE` slowed (save ends)
        tier3: 17 damage; `I < STRONG` slowed (save ends)
        effect: The phantom deals an additional 3 damage if they have an edge.
  - type: feature
    feature_type: trait
    name: ⭐ Ripping Phase
    icon: ⭐️
    effects:
      - effect: The phantom can move through other creatures and objects at normal speed. The first time in a round that the phantom passes through a creature, that creature takes 3 corruption damage and has a bane on their next strike. The phantom doesn't take damage from being forced into objects.

~~~


