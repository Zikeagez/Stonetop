

~~~ds-statblock
type: statblock
name: Lightbender
level: .  
roles:
  - Companion
ancestry:
  - Beast
  - Companion
speed: 7
size: 1L
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
        effect: Hide
  - type: feature
    feature_type: ability
    name: 🗡️ Sparking Tail Whip
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
        effect: _The lightbender swings their tail, sending gouts of sparks in their foe's face._
      - name: Effect
        effect: The target takes damage equal to 3 + the lightbender's Might score, and if they have `M < AVERAGE`, they are dazzled until the end of their next turn. A dazzled creature has line of effect only within 1 square.
      - name: Spend 1 Ferocity
        effect: A dazzled creature also takes a bane on strikes.
  - type: feature
    feature_type: trait
    name: ⭐Avoidance
    icon: ⭐
    effects:
      - effect: Any effect on the lightbender that would be ended by a saving throw instead ends automatically at the end of their next turn.

~~~

> **Level 3 Lightbender Advancement Feature**
> ⭐**Hit and Run**
>Whenever the lightbender makes a strike against a creature while rampaging, the lightbender can teleport up to 5 squares and use the Hide maneuver.

>**Level 6 Lightbender Advancement Feature**
>⭐**Lightbearer**
>While the lightbender is rampaging, you can use a free maneuver to glow with blinding light that lasts until the rampage ends or you use this ability again. While glowing, your skin sheds light for 10 squares and strikes against you take a bane.

> **Level 10  Lightbender Advancement Feature**
> ⭐**Everywhere and Nowhere**
>While the lightbender is rampaging, your grip on spatial reality is weakened, and once on each of your turns, you or the lightbender can teleport up to 3 spaces as a free maneuver. Additionally, strikes made against you and the lightbender have a double bane until the lightbender's rampage ends.


