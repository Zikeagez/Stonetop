

~~~ds-statblock
type: statblock
name: Panther
level: .  
roles:
  - Companion
ancestry:
  - Animal
  - Companion
speed: 7
size: 1M
stability: 1
free_strike: 1+M
movement: Climb
might: 2
agility: 2
reason: -1
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: trait
    name: Skills
    icon: 🗡
    effects:
      - name: 
        effect: Sneak
  - type: feature
    feature_type: ability
    name: 🗡️ Pounce
    icon: 🗡️
    usage: Maneuver
    keywords:
      - Companion
      - Melee
      - Weapon
    distance: 📐 Melee 1
    target: 🎯One enemy
    effects:
      - name: Description
        effect: _The panther bunches up, then uncoils into a deadly leap._
      - name: Effect
        effect: The target takes damage equal to 3 + the panther's Might score, and if they have `M < AVERAGE`, they are knocked prone.
      - name: Spend 1 Ferocity
        effect: The panther can jump up to a number of squares equal to their speed before using this ability. If they jump at least 1 square in this way, a target who has `M < STRONG` is knocked prone.
  - type: feature
    feature_type: trait
    name: ⭐Mighty Spring
    icon: ⭐
    effects:
      - effect: Whenever the panther takes the Advance move action or the Charge action, they can jump up to a number of squares equal to their speed in any direction, including vertically, as part of this movement.

~~~

> **Level 3 Panther Advancement Feature**
> ⭐**Cat and Mouse**
>Whenever the panther makes a strike against a creature while rampaging, the panther can knock the target prone.

>**Level 6 Panther Advancement Feature**
>⭐**Single Bound**
>While the panther is rampaging, you can jump up to a number of squares equal to your speed as a free maneuver once on each of your turns.

> **Level 10  Panther Advancement Feature**
> ⭐**Panther Spirit**
>While the panther is rampaging, you and the panther are invisible and can move through objects and terrain, which are difficult terrain for you both. A creature who ends their turn inside a solid object from moving this way is teleported to the last unoccupied space they previously occupied.


