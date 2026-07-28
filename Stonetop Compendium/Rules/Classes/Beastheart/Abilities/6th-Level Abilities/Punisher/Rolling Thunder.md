```ds-feature
type: feature
feature_type: ability
name: Rolling Thunder
cost: 9 Ferocity
flavor: The rumble of your companion's dash is a rolling thunderclap, their impact an earthquake.
keywords:
  - Companion
  - Magic
  - Melee
  - Strike
usage: Main Action
distance: 📐 Self
target: 🎯 Self
effects:
  - name: Effect
    effect: Your companion shifts up to their speed and makes one power roll that targets each enemy they come adjacent to during the shift. If your companion targets only one enemy with this ability, the power roll gains an edge.

  - roll: Power Roll + Might
    tier1: 9 sonic damage; `M < WEAK` prone
    tier2: 13 sonic damage; `M < AVERAGE` prone
    tier3: 18 sonic damage; `M < STRONG` prone

  - name: Spend 2 Ferocity
    effect: You can move up to your speed. The power roll also targets each enemy you come adjacent to during the move.


```

