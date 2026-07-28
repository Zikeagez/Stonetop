```ds-feature
type: feature
feature_type: ability
name: Bring the Thunder
flavor: Your companion unleashes a shattering roar, screech, or howl that terrifies your foes - or at least gets their attention.
keywords:
  - Area
  - Companion
  - Magic
cost: 3 Ferocity
usage: Main action
distance: 📐 2 Burst
target: 🎯 Each enemy in the area
effects:
  - roll: Power Roll + Intuition
    tier1: 3 sonic damage; push 1; `P < WEAK` taunted (save ends)
    tier2: 5 sonic damage; push 2; `P < AVERAGE` taunted (save ends)
    tier3: 7 sonic damage; push 3; `P < STRONG` frightened (save ends)

  - name: Spend 1 Ferocity
    effect: This ability also affects a 2 burst originating from you. An enemy in both areas is only affected once.
```

