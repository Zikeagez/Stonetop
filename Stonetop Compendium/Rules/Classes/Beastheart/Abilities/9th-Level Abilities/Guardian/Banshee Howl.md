```ds-feature
type: feature
feature_type: ability
name: Banshee Howl
cost: 11 Ferocity
flavor: Your companion's howl, screech, roar, or psychic emanation presages death to those who hear it.
keywords:
  - Area
  - Companion
  - Magic
usage: Main Action
distance: 📐 3 burst
target: 🎯 Each enemy in the area
effects:
  - roll: Power Roll + Intuition
    tier1: 5 sonic damage; `I < WEAK` frightened (save ends)
    tier2: 10 sonic damage; `I < AVERAGE` frightened (save ends)
    tier3: 15 sonic damage; `I < STRONG` frightened (save ends)

  - name: Effect
    effect: While frightened this way, a creature takes 10 psychic damgae at the start of each of your turns.

  - name: Spend 1 Ferocity
    effect: This ability also affects a 3 burst originating from you. An enemy in both areas is only affected once. 
```

