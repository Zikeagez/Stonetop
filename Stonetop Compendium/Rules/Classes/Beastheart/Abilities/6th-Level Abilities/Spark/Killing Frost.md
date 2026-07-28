```ds-feature
type: feature
feature_type: ability
name: Killing Frost
cost: 9 Ferocity
flavor: Black frost freezes boots to the floor and creeps up trapped victims until they're completely encased in ice.
keywords:
  - Area
  - Companion
  - Magic
usage: Main Action
distance: 📐 5 cube within 1
target: 🎯 Each enemy in the area
effects:
  - roll: Power Roll + Might
    tier1: 5 cold damage; `I < WEAK` restrained (save ends)
    tier2: 7 cold damage; `I < AVERAGE` restrained (save ends)
    tier3: 12 cold damage; `I < STRONG` restrained (save ends)

  - name: Effect
    effect: While restrained this way, a creature takes 5 cold damage at the start of each of your turns. A creature killed by this ability becomes an ice statue and their space is difficult terrain.
```

