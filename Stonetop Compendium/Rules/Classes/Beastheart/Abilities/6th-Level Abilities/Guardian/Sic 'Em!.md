```ds-feature
type: feature
feature_type: ability
name: Sic 'Em!
cost: 9 Ferocity
flavor: Your companion rushes forward to protect you from a dangerous foe.
keywords:
  - Charge
  - Companion
  - Melee
  - Strike
  - Weapon
usage: Main Action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 11 + M damage; taunted (save ends); `M < WEAK` prone
    tier2: 16 + M damage; taunted (save ends); `M < AVERAGE` prone
    tier3: 21 + M damage; taunted (save ends); `M < STRONG` prone and can't stand (EoT)

  - name: Spend 2 Ferocity
    effect: Your companion can use this ability as a triggered action against an enemy who damages you.
```

