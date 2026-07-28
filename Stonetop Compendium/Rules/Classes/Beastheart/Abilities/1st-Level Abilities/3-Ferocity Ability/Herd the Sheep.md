```ds-feature
type: feature
feature_type: ability
name: Herd the Sheep
flavor: Your companion circles your foe, luring them out of position with fake openings and unpredictable attacks.
keywords:
  - Companion
  - Melee
  - Strike
  - Weapon
cost: 3 Ferocity
usage: Main action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 5 + M damage; slide 1; `I < WEAK` weakened (save ends)
    tier2: 8 + M damage; slide 2; `I < AVERAGE` weakened (save ends)
    tier3: 11 + M damage; slide 4; `I < STRONG` weakened (save ends)

  - name: Spend 1 Ferocity
    effect: You and your companion can shift up to a number of squares equal to the number of squares the target was force moved.
```

