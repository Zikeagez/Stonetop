```ds-feature
type: feature
feature_type: ability
name: I Feed On Your Pain!
cost: 5 Ferocity
flavor: Invigorated by the smell of blood, you strike a savage blow.
keywords:
  - Beastheart
  - Melee
  - Range
  - Strike
  - Weapon
usage: Main action
distance: 📐 Melee 1 or ranged 5
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 8 + M damage 
    tier2: 12 + M damage 
    tier3: 16 + M damage; `M < STRONG` bleeding (save ends)

  - name: Effect
    effect: If the target is killed by this damage, or is winded or bleeding after taking this damage, you gain 2 surges.
```

