```ds-feature
type: feature
feature_type: ability
name: Battle Frenzy
cost: 11 Ferocity
flavor: Your companion shatters the floodgates that keep their rampage dammed up, and it cascades into the unprepared minds of nearby creatures.
keywords:
  - Area
  - Companion
  - Magic
usage: Main Action
distance: 📐 5 burst
target: 🎯 Special
effects:
  - name: Special
    desc: This ability targets only creatures you choose within distance.

  - roll: Power Roll + Might
    tier1: If `P < WEAK` the target is battle-frenzied  
    tier2: If `P < AVERAGE` the target is battle-frenzied 
    tier3: If `P < STRONG` the target is battle-frenzied    
  - name: Effect
    effect: >-
      If a target resists the potency, they can choose to become battle-frenzied

      A battle-frenzied creature must use a free triggered action to make a melee free strike against themself or a creature adajcent to them. You choose each creature's target. After making this strike, they are no longer battle frenzied.
```

