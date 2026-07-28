

~~~ds-statblock
type: statblock
name: Spider
level: .  
roles:
  - Companion
ancestry:
  - Animal
  - Companion
speed: 5
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
    name: 🏹 Web Shot
    icon: 🏹
    usage: Maneuver
    keywords:
      - Companion
      - Ranged
      - Weapon
    distance: 📐 Ranged 5
    target: 🎯One enemy
    effects:
      - name: Description
        effect: _The spider fires a ball of sticky silk._
      - name: Effect
        effect: If the target has `M < AVERAGE`, they are restrained until the end of their next turn.
      - name: Spend 1 Ferocity
        effect: If the target has `M < STRONG`, they are restrained (save ends).
  - type: feature
    feature_type: trait
    name: ⭐Come Into My Parlor
    icon: ⭐
    effects:
      - effect: Whenever the spider makes a strike against a restrained creature, the spider deals extra poison damage equal to twice their Intuition score.

~~~

> **Level 3 Spider Advancement Feature**
> ⭐**Dripping Fangs**
>Whenever the spider makes a strike against a creature while rampaging, the spider can deal extra poison damage equal to their Might score.

>**Level 6 Spider Advancement Feature**
>⭐**Web Slinger**
>Once on each of your turns while the spider is rampaging, you can shoot a web to a ceiling, wall, or sturdy object above you within 5 squares as a free maneuver. You can then fly in a straight line to any space within 5 squares of that object.

> **Level 10  Spider  Advancement Feature**
> ⭐**Life Drinker**
>Whenever you or the spider deals damage with a maneuver while the spider is rampaging, the attacker regains Stamina equal to the damage dealt.


