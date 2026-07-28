

~~~ds-statblock
type: statblock
name: Elemental Spark
level:  
roles:
  - Companion
ancestry:
  - Elemental
  - Companion
speed: 7
size: 1M
stability: 1
free_strike: 1+M
immunities:
  - Lightning 3
might: 2
agility: 1
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
        effect: Magic
  - type: feature
    feature_type: ability
    name: 🗡️ Static Shock
    icon: 🗡️
    usage: Maneuver
    keywords:
      - Companion
      - Magic
      - Melee
    distance: 📐 Melee 1
    target: 🎯One enemy
    effects:
      - name: Description
        effect: _An arc of lightning crackles from the spark._
      - name: Effect
        effect: The target takes lightning damage equal to 2 + the spark's Might score.
      - name: Spend 1 Ferocity
        effect: The distance increases to melee 5.
  - type: feature
    feature_type: trait
    name: ⭐Electric Surge
    icon: ⭐
    effects:
      - effect: The first time on a turn that you or the spark deal lightning damage, you gain 1 surge.

~~~

> **Level 3 Elemental Spark Advancement Feature**
> ⭐**Electroshock**
>Whenever the spark makes a strike agains a creature while rampaging, they can cause a target who has M < AVERAGE to be dazed until the end of teh target's next turn.


>**Level 6 Elemental Spark Advancement Feature**
>⭐**Conductive**
>While the spark is rampaging, lightning sings through your blood, and whenever you make a strike against a creature, you deal extra lightning damage equal to your might score.

> **Level 10 Elemental Spark Advancement Feature**
> ⭐**Lightning Speed**
>While the spark is rampaging, you and the spark can shift up to your speed as a free maneuver once on each of your turns.


