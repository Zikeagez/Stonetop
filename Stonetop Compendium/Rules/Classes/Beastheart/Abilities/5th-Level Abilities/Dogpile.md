```ds-feature
type: feature
feature_type: ability
name: Dogpile
cost: 9 Ferocity
flavor: You and your allies surround your enemy like a pack of wolves, mobbing them and pulling them down.
keywords:
  - Beastheart
  - Melee
  - Strike
  - Weapon
usage: Main Action
distance: 📐 Melee 1
target: 🎯 One creature
effects:
  - roll: Power Roll + Might
    tier1: 10 + M damage; `M < WEAK` grabbed and prone
    tier2: 15 + M damage; `M < AVERAGE` grabbed and prone
    tier3: 20 + M damage; `M < STRONG` grabbed and prone

  - name: Effect
    effect: Each ally adjacent to the target can use a free triggered action to deal damage to the target equal to their highest characteristic score.
```

