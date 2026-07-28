

~~~ds-statblock
type: statblock
name: Deinonychus
level:  
roles:
  - Companion
ancestry:
  - Animal
  - Companion
speed: 7
size: 1M
stability: 1
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
    name: 🗡️ Terrible Claws
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
        effect: _The deinonychus kicks their prey, then slashes them with wicked claws._
      - name: Effect
        effect: The target takes damage euqal to 3 + the deinonychus's Might score, and if they have `M < AVERAGE`, they are bleeding until the end of their next turn.
      - name: Spend 1 Ferocity
        effect: A target who has `M < STRONG`is bleeding (save ends).
  - type: feature
    feature_type: trait
    name: ⭐ Blood Frenzy
    icon: ⭐️
    effects:
      - effect: Whenever the deinonychus deals damage to a bleeding creature, they gain 1 surge.

~~~

> **Level 3 Deinonychus Advancement Feature**
> ⭐**Tear You to Ribbons**
>Whenever the deinonychus makes a strike against a creature while rampaging, the target is bleeding until the end of their next turn.


>**Level 6 Deinonychus Advancement Feature**
>⭐**Slake My Thirst in Blood**
>Whenever you use an ability that deals rolled damage to a bleeding creature while teh deinonychus is rampaging, you gain 2 surges. 

> **Level 10 Deinonychus Advancement Feature**
> ⭐**Reaping Scythe**
>The deinonychus's claws slash at creatures underfoot. When the deinonychus moves adjacent to an enemy or enters an enemy's space for the first time on a turn while rampaging, the deinonychus deals damage to that enemy equal to the deinonychus's Might score.


