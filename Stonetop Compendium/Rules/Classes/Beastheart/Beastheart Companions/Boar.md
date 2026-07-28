

~~~ds-statblock
type: statblock
name: Boar
level:  
roles:
  - Companion
ancestry:
  - Animal
  - Companion
speed: 5
size: 1M
stability: 2
free_strike: 1+M
might: 2
agility: 1
reason: -1
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: trait
    name: Skills
    icon: 🗡
    effects:
      - name: 
        effect: Search
  - type: feature
    feature_type: ability
    name: 🗡️ Gore
    icon: 🗡️
    usage: Maneuver
    keywords:
      - Companion
      - Melee
      - Weapon
    distance: 📐 Melee 1
    target: 🎯One creature or object
    effects:
      - name: Description
        effect: _With an enraged snort, the boar lunges forward to rip open foes with their tusks._
      - name: Effect
        effect: The boar moves up to their speed in a straight line. When this movement ends, they can deal damage equal to 3 + their Might score to an adjacent target. If the boar moved closer to the target as part of this movement, the boar deals extra damage equal to their Might score.
      - name: Spend 1 Ferocity
        effect: The target is bleeding until the end of their next turn.
  - type: feature
    feature_type: trait
    name: ⭐️ Spiteful Endurance
    icon: ⭐️
    effects:
      - effect: While the boar is winded, they have damage immunity equal to their Might score and ignore the effects of bleeding.


~~~

> **Level 3 Boar Advancement Feature**
> ⭐**Greased Pig**
> While the boar is rampaging, they have a +2 bonus to speed and a double edge on the Escape Grab maneuver.


>**Level 6 Boar Advancement Feature**
>⭐**Wild Rush**
>While the boar is rampaging, you can use their Gore maneuver, and you and the boar can shift instead of move when using the Charge action or the Gore maneuver.

> **Level 10 Boar Advancement Feature**
> ⭐**Immortal Rage**
>Whenever you or the boar use an ability that deals damage while the boar is rampaging, you gain 10 temporary stamina.


