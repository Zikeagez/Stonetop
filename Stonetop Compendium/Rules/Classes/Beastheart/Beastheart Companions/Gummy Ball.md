

~~~ds-statblock
type: statblock
name: Gummy Ball
level: .  
roles:
  - Companion
ancestry:
  - Ooze
  - Companion
speed: 5
size: 1L
stability: 2
free_strike: 1+M
immunities:
  - Acid 3
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
    name: 🗡️ Absorb
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
        effect: _With a sickening squelch, the ball oozes around their hapless prey._
      - name: Effect
        effect: The target takes acid damage equal to 3 + the ball's Might score, and if they have A < AVERAGE, the ball moves into the target's space. If the target completely fits within the ball's space, the target is grabbed by the ball.
      - name: Spend 1 Ferocity
        effect: A target grabbed this way takes acid damage equal to the ball's Might score at the end of each of the ball's turns.
  - type: feature
    feature_type: trait
    name: ⭐Gelatinous
    icon: ⭐
    effects:
      - effect: The ball can occupy another creature's space. While occupying a creature's space, the ball has line of effect to that creature. If the creature completely fits within the ball's space, the creature has line of effect only to the ball and creatures outside the ball don't have line of effect to the creature. The ball's space is difficult terrain.

~~~

> **Level 3 Gummy Ball Advancement Feature**
> ⭐**Suck It Up**
>Whenever the ball makes a strike while rampaging, one target is pulled up to 3 squares into the ball's space. If the target ends this movement and completely fits within the ball's space, the target is grabbed by the ball.

>**Level 6 Gummy Ball Advancement Feature**
>⭐**Taffy Pull**
>While the ball is rampaging, your arms and legs become viscous and stretchy, and you gain +2 bonus to speed and melee distance.

> **Level 10 Gummy Ball Advancement Feature**
> ⭐**Runaway Expansion**
>While the ball is rampaging, you and the ball have acid immunity 10, and whenever a creature is reduced to 0 Stamina while inside the ball, the ball's size increases by 1 (to a maximum of 5). The ball's size can't increase this way more than once a turn, and the ball shrinks back to their original size when their rampage ends.


