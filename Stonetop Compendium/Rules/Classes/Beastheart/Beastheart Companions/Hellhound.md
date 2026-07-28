

~~~ds-statblock
type: statblock
name: Helllhound
level: .  
roles:
  - Companion
ancestry:
  - Infernal
  - Companion
speed: 7
size: 1M
stability: 1
free_strike: 1+M
immunities:
  - Fire 3
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
        effect: Intimidate
  - type: feature
    feature_type: ability
    name: 🗡️ Fire Breath
    icon: 🗡️
    usage: Maneuver
    keywords:
      - Companion
      - Magic
      - Melee
      - Ranged
    distance: 📐 Melee 1 or Ranged 2
    target: 🎯One enemy
    effects:
      - name: Description
        effect: _The hellhound exhales infernal flames._
      - name: Effect
        effect: The target takes fire damage equal to 3 + the hellhound's Might score.
      - name: Spend 1 Ferocity
        effect: This ability gains a bonus to either its damage or distance equal to the hellhound's Intuition score.
  - type: feature
    feature_type: trait
    name: ⭐Hellish Pact
    icon: ⭐
    effects:
      - effect: You have fire immunity equal to the hellhound's fire immunity

~~~

> **Level 3 Hellhound Advancement Feature**
> ⭐**Infernal Apparition**
>Whenever the hellhound makes a strike against a creature while rampaging, they can cause a target who has `P < AVERAGE` to be frightened until the end of the target's next turn.

>**Level 6 Hellhound Advancement Feature**
>⭐**Slavering Jaws**
>While the hellhound is rampaging, your mouth foams with acidic ichor, and whenever you make a strike against a creature, you deal extra acid damage equal to your Might score.

> **Level 10  Hellhound Advancement Feature**
> ⭐**Wreathed in Flames**
>While the hellhound is rampaging, you and the hellhound are surrounded by an aura of flames, and each enemy who starts their turn adjacent to you or the hellhound takes fire damage equal to the hellhound's Might score.


