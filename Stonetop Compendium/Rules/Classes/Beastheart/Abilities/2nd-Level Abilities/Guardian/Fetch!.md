```ds-feature
type: feature
feature_type: ability
name: Fetch!
cost: 5 Ferocity
flavor: Your companion blinks out of existence, returning with a visitor you were particularly hoping to meet.
keywords:
  - Companion
  - Magic
  - Melee
  - Strike
  - Weapon
usage: Main action
distance: 📐 Melee 1
target: 🎯 One creature or object
effects:
  - name: Effect
    effect: Your companion can teleport up to 5 squares before and after making the power roll. Instead of grabbing the target, your companion can pick up a target object that is smaller than they are. You can forgo dealing damage with this ability.
  - roll: Power Roll + Might
    tier1: 6 + M damage; `M < WEAK` grabbed 
    tier2: 8 + M damage; `M < AVERAGE` grabbed 
    tier3: 12 + M damage; `M < STRONG` grabbed

  - name: 
    effect: After making the power roll, your companion can teleport with a grabbed creature or held object, provided the creature or object can fit in the destination. You choose which squares adjacent to your companion the grabbed creautre or held object is teleported to.
```

