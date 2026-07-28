~~~ds-statblock
type: statblock
name: Light of the Sun
level: .
roles:
  - Minion Support
ancestry:
  - Elemental (Air, Green, Fire, Void)
ev: 7 essence for two minions
speed: 6
size: 2
stamina: 17|17
movement: Fly
weaknesses:
stability: 0
free_strike: 7
might: 0
agility: 2
reason: 4
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Free Strike Damage Type - Fire
  - type: feature
    feature_type: ability
    name: 🏹 Solar Blade 2d10 + R - Signature Ability
    icon: 🏹
    usage: Main action
    keywords:
      - Magic
      - Melee
      - Strike
    distance: Melee 1
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 7 fire damage; `I < WEAK` dazed (EoT)
        tier2: 11 fire damage; `I < AVERAGE` dazed (EoT)
        tier3: 16 fire damage; `I < STRONG` dazed (save ends)
        effect: A target dazed by this ability has their stability reduced to 0 until the condition ends.
  - type: feature
    feature_type: trait
    name: ⭐ Soulsight
    cost: 2 Essence
    icon: ⭐️
    effects:
      - effect: When the light is reduced to 0 Stamina, the area within 1 square of the light becomes wreathed in sentient flames until the end of the encounter. An enemy that enters this area or starts their turn there takes 3 fire damage and is slowed (EoT). You or any ally that enters this area or starts their turn there gains 5 temporary Stamina and their speed increases by 2 until the end of their turn.

~~~


