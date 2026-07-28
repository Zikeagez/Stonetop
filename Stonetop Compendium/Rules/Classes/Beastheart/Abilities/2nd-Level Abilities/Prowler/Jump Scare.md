```ds-feature
type: feature
feature_type: ability
name: Jump Scare
cost: 5 Ferocity
flavor: Surprised to see me?
keywords:
  - Area
  - Companion
  - Magic
usage: Main action
distance: 📐 2 burst
target: 🎯 Each enemy in the area
effects:
  - name: Special
    effect: This ability targets only enemies with line of effect to your companion
  - name: Effect
    effect: Your companion shifts up to a number of squares equal to their Intuition score. During this movement, they are invisible. They then make a power roll.
  - roll: Power Roll + Intuition
    tier1: 4 damage; `P < WEAK` frightened (save ends) 
    tier2: 6 damage; `P < AVERAGE` frightened (save ends)
    tier3: 10 damage; `P < WEAK` frightened (save ends)
```

