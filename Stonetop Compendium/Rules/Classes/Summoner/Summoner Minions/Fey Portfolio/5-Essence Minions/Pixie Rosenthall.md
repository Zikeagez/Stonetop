~~~ds-statblock
type: statblock
name: Pixie Rosenthall
level: .
roles:
  - Minion Harrier
ancestry:
  - Fey
  - Swarm
ev: 5 essence for three minions
speed: 6
size: 2
stamina: 5|5|5
movement: Fly, hover
weaknesses: 
stability: 1
free_strike: 3
might: 0
agility: 2
reason: 4
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: 🗡️ Stickerbush Symphony 2d10 + R -  Signature Ability
    icon: 🗡️
    usage: Main action
    keywords:
      - Melee
      - Strike
      - Weapon
    distance: Melee 2
    target: 🎯 One creature or object per minion
    effects:
      - roll: Power Roll + Reason
        tier1: 3 damage; pull 2; `A < WEAK` bleeding (EoT)
        tier2: 6 damage; pull 3; `A < AVERAGE` bleeding (EoT)
        tier3: 8 damage; pull 4; `A < STRONG` bleeding (EoT)
        effect: A target can't shift while bleeding from this ability.
  - type: feature
    feature_type: trait
    name: ⭐ Swarm
    icon: ⭐
    effects:
      - name: 
        effect: The rosenthall can move through squares as if they were size 1T, and can occupy other creatures' spaces. At the start of the rosenthall's turn, they deal 2 damage to each enemy whose space they share.

~~~

