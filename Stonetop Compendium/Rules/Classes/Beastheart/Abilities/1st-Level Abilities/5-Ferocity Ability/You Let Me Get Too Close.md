```ds-feature
type: feature
feature_type: ability
name: You Let Me Get Too Close
cost: 5 Ferocity
flavor: The wilderness has no concept of fair play.
keywords:
  - Beastheart
  - Charge
  - Melee
  - Strike
  - Weapon
usage: Main action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 8 + M damage; `M < WEAK` grabbed
    tier2: 12 + M damage; `M < AVERAGE` grabbed
    tier3: 16 + M damage; `M < STRONG` grabbed

  - name: Effect
    effect: If you grab the target while your companion is adjacent to them, your companion can make a melee free strike against the target.
```

