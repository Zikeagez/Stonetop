

~~~ds-statblock
type: statblock
name: Wolf
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
    name: 🗡️ Clamping Jaws
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
        effect: _With an unnerving growl, the wolf sinks powerful teeth into their quarry._
      - name: Effect
        effect: The target takes damage equal to 3 + the wolf's Might score, and if they have `M < AVERAGE`, they are grabbed by the wolf.
      - name: Spend 1 Ferocity
        effect: If the target has `M < STRONG`, they are grabbed by the wolf.
  - type: feature
    feature_type: trait
    name: ⭐Retriever
    icon: ⭐
    effects:
      - effect: The wolf can move at full speed while they have a creature grabbed, no matter the grabbed creature's size.

~~~

> **Level 3 Wolf Advancement Feature**
> ⭐**My, What Big Teeth You Have**
>Whenever the wolf makes a strike against a creature while rampaging, they can grab the target.

>**Level 6 Wolf Advancement Feature**
>⭐**Call of the Wild**
>While the wolf is rampaging, you and the wolf gain a +2 bonus to speed, and creatures within 5 squares can't be hidden or have concealment from you or the wolf.

> **Level 10  Wolf  Advancement Feature**
> ⭐**Dire Wolf**
>While the wolf is rampaging, you and the wolf are surrounded by an aura of dread, and enemies who start their turn adjacent to you or the wolf who have `P < STRONG` are frightened until the end of their next turn.


