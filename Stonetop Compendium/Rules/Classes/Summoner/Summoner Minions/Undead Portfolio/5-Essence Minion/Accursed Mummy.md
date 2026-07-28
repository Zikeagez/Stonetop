~~~ds-statblock
type: statblock
name: Accursed Mummy
level: .
roles:
  - Minion Hexer
ancestry:
  - Mummy
  - Undead
ev: 5 essence for three minions
speed: 5
size: 1M
stamina: 4|4|4
movement: 
weaknesses: 
  - Fire 1 
stability: 2
free_strike: 3
might: 2
agility: -1
reason: 1
intuition: 3
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Poison
  - type: feature
    feature_type: ability
    name: 🗡️ Fetid Binding 2d10 + R -  Signature Ability
    icon: 🗡️
    usage: Main action
    keywords:
      - Melee
      - Strike
      - Weapon
    distance: Melee R
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 3 poison damage; pull R
        tier2: 4 poison damage; pull R + 1
        tier3: 6 poison damage; pull R + 2
        effect: A target pulled adjacent to the mummy is `M < STRONG` weakened (EoT).
  - type: feature
    feature_type: trait
    name: ⭐ Mummy Dust
    icon: ⭐
    effects:
      - name: 
        effect: Whenever the mummy takes damage, each enemy adjacent to the mummy takes 2 poison damage.

~~~

