

~~~ds-statblock
type: statblock
name: Bear
level:  
roles:
  - Companion
ancestry:
  - Animal
  - Companion
speed: 5
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
        effect: Intimidate
  - type: feature
    feature_type: ability
    name: 🗡️ Backhand
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
        effect: _The bear casually swats the pesky foe into next week._
      - name: Effect
        effect: The target takes damage equal to 4 + the bear's Might score and is pushed up to 2 squares.
      - name: Spend 1 Ferocity
        effect: The target is force moved up to a number of additional squares equal to the bear's Might score.
  - type: feature
    feature_type: trait
    name: ⭐ Strong like a bear
    icon: ⭐️
    effects:
      - effect: You gain a +1 bonus to your stability.


~~~

> **Level 3 Bear Advancement Feature**
> ⭐**Foes Thresher**
> Whenever the bear targets a creature with a strike that doesn't impose forced movement while rampaging, the bear can push the target up to a number of squares equal to the bear's Might score.


>**Level 6 Bear Advancement Feature**
>⭐**Ursine Form**
>While the bear is rampaging, you have damage immunity 5 and your size increases to the bear's size (to a maximum of 2). If you don't have enough unoccupied space to grow, you grow as soon as there is sufficient space.

> **Level 10 Bear Advancement Feature**
> ⭐**Twin Colossi**
> While the bear is rampaging, you gain a +1 bonus to distance with melee weapon abilities, your size increases to match the bear's size (to a maximum of 3), and your strikes deal an extra 5 damage.


