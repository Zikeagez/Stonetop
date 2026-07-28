```ds-feature
type: feature
feature_type: ability
name: Foe Bowling
cost: 5 Ferocity
flavor: Your companion sends one enemy tumbling into another, taking them both out.
keywords:
  - Charge
  - Companion
  - Melee
  - Strike
  - Weapon
usage: Main action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 3 + M damage; push 2; `M < WEAK` prone
    tier2: 5 + M damage; push 3; `M < AVERAGE` prone
    tier3: 8 + M damage; push 3; `M < AVERAGE` prone
  - name: Effect
    effect: If the target is force moved at least 1 square, an enemy adjacent to the target at the end of this forced movement is also targeted by this ability's power roll, but they don't trigger this effect.
```

