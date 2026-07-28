~~~ds-statblock
type: statblock
name: Pixie Hydrain
level: .
roles:
  - Minion Artillery
ancestry:
  - Fey
ev: 3 essence for two minions
speed: 5
size: 1T
stamina: 5|5
movement: Fly, hover
immunities:
  - Acid R
stability: 0
free_strike: 5
might: -3
agility: 0
reason: 1
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Acid
  - type: feature
    feature_type: ability
    name: 🏹 Burning/Healing Rain 2d10 + `R` | Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Ranged
      - Strike
    distance: Ranged 5
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 5 acid damage; `M < WEAK` weakened (EoT)
        tier2: 7 acid damage; `M < AVERAGE` weakened (EoT)
        tier3: 9 acid damage; `M < STRONG` weakened (Save Ends)
        effect: After the hydrain's squad uses this ability, you or one ally within distance can spend a Recovery or end a condition.
  - type: feature
    feature_type: trait
    name: ⭐ Miniscule
    icon: ⭐️
    effects:
      - effect: The soakreed has cover while occupying a larger creature's space.


~~~


