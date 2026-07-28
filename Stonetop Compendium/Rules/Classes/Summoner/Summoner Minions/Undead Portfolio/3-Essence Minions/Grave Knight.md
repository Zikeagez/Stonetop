~~~ds-statblock
type: statblock
name: Grave Knight
level: .
roles:
  - Minion Brute
ancestry:
  - Undead
ev: 3 essence for two minions
speed: 5
size: 1M
stamina: 6|6
movement:
immunities:
  - Corruption R, poison R
stability: 1
free_strike: 5
might: 2
agility: 1
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: 🗡️ Knight Strike 2d10 + R - Signature Ability
    icon: 🗡️
    usage: Main action
    keywords:
      - Melee
      - Strike
      - Weapon
    distance: Melee 1
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 5 corruption damage; `M < WEAK` bleeding (EoT)
        tier2: 7 corruption damage; `M < AVERAGE` bleeding (EoT)
        tier3: 9 corruption damage; `M < STRONG` bleeding (Save Ends)
  - type: feature
    feature_type: trait
    name: ⭐ To the Grave
    icon: ⭐️
    effects:
      - effect: When the grave knight is reduced to 0 Stamina, they can make a melee strike before being destroyed.

~~~


