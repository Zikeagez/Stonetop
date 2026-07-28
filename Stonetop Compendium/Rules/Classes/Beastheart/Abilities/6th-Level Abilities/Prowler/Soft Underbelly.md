```ds-feature
type: feature
feature_type: ability
name: Soft Underbelly
cost: 9 Ferocity
flavor: Your companion ducks under your enemy's guard and rakes open their soft vitals, leaving them vulnerable
keywords:
  - Companion
  - Melee
  - Strike
  - Weapon
usage: Main Action
distance: 📐 Melee 2
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 10 + M damage; `A < WEAK` bleeding (save ends)
    tier2: 15 + M damage; `A < AVERAGE` bleeding (save ends)
    tier3: 20 + M damage; `A < STRONG` bleeding (save ends)

  - name: Effect
    effect: While bleeding this way, the target has damage weakness 5.

```

