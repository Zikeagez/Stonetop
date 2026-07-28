```ds-feature
type: feature
feature_type: ability
name: Relentless
cost: 11 Ferocity
flavor: Your companion launches at your foe, shielding allies with their body.
keywords:
  - Charge
  - Companion
  - Melee
  - Strike
  - Weapon
usage: Main Action
distance: 📐 Melee 1
target: 🎯 One enemy
effects:
  - roll: Power Roll + Might
    tier1: 11 + M damage; `P < WEAK` taunted (save ends)
    tier2: 17 + M damage; `P < AVERAGE` taunted (save ends)
    tier3: 22 + M damage; `P < STRONG` taunted (save ends)

  - name: Effect
    effect: While the target is taunted this way, all creatures except your companion have immunity 10 to damage dealt by the target.
```

