

~~~ds-statblock
type: statblock
name: Sporeling
level: .  
roles:
  - Companion
ancestry:
  - Beast
  - Companion
speed: 5
size: 1S
stability: 0
immunities:
  - Poison 3
free_strike: 1+M
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
        effect: Track
  - type: feature
    feature_type: ability
    name: 🗡️ Spore Puff
    icon: 🗡️
    usage: Maneuver
    keywords:
      - Companion
      - Melee
    distance: 📐 Melee 1
    target: 🎯One enemy
    effects:
      - name: Description
        effect: _The sporeling breathes a cloud of disorienting fumes._
      - name: Effect
        effect: The target takes poison damage equal to 3 + the sporeling's Might score, and the sporeling is invisible to the target until the end of the sporeling's next turn or they deal damage to the target.
      - name: Spend 1 Ferocity
        effect: If the target has `M < STRONG`, they are dazed until the end of their next turn.
  - type: feature
    feature_type: trait
    name: ⭐Skulker
    icon: ⭐
    effects:
      - effect: The sporeling can end their movement in an ally's space. While occupying an ally's space, the sporeling has cover.

~~~

> **Level 3 Sporeling Advancement Feature**
> ⭐**Slowing Spores**
>Whenever the sporeling makes a strike against a creature while rampaging, the sporeling can cause the target to be slowed until the end of the target's next turn.

>**Level 6 Sporeling Advancement Feature**
>⭐**Plant Walk**
>Once on each of your turns while the sporeling is rampaging, you can teleport to a space within 15 squares as a free maneuver, provided the space or an adjacent space contains the sporeling or plants or fungus of size 1S or larger. You then gain an edge on the next strike you make before the end of your next turn.

> **Level 10  Sporeling  Advancement Feature**
> ⭐**Trailing Mycelia**
>While the sporeling is rampaging, you and thes poreling sprout rootlike, gripping mycelia along your limbs, and whenever you or the sporeling makes a strike against a creature who has `M < STRONG`, the creature is grabbed by the attacker. Additionally, you and the sporeling can't be force moved or knocked prone until the sporeling's rampage ends.


