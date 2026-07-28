
`BUTTON[rules]`

`BUTTON[actiontable]`   &nbsp&nbsp   `BUTTON[skillactions]` &nbsp&nbsp `BUTTON[weapontraits]` &nbsp&nbsp `BUTTON[conditions]` &nbsp&nbsp`BUTTON[charcreation]`    &nbsp&nbsp   `BUTTON[levelup]`   &nbsp&nbsp   `BUTTON[buyinggear]`  

## **Playing the Game**

> [!infobox]
>  # Session Journals
>  #### `BUTTON[sessionjournal]`
>  ```dataview 
TABLE WITHOUT ID link(file.name) AS "Session Date", Adventure,  OneLiner AS "Description"
from "0. Session Journals"
where (type="Session Journal")
SORT file.name DESC
LIMIT 10



```meta-bind-button
label: Magus Features
icon: ""
style: default
class: button-74
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: actionable
hidden: false
actions:
  - type: open
    link: 2. Mechanics/Classes/Magus
    newTab: true
```
<br>

> [!example]- General Table
> |                                                                                        |                                                                      |                                                                                                              |
|:--------------------------------------------------------------------------------------:|:--------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------:|
|        [[PF2e Journals/GM Screen/Bonuses and Penalties\|Bonuses and Penalties]]        |      [[PF2e Journals/GM Screen/Size and Reach\|Size and Reach]]      |                                 [[PF2e Journals/GM Screen/Falling\|Falling]]                                 |
| [[PF2e Journals/GM Screen/Death, Dying and Unconscious\|Death, Dying and Unconscious]] |   [[PF2e Journals/GM Screen/Terrain and Cover\|Terrain and Cover]]   |                            [[PF2e Journals/GM Screen/Treat Wounds\|Treat Wounds]]                            |
|                [[PF2e Journals/GM Screen/Counteracting\|Counteracting]]                |               [[PF2e Journals/GM Screen/Light\|Light]]               |                            [[PF2e Journals/GM Screen/Travel Speed\|Travel Speed]]                            |
|                       [[PF2e Journals/GM Screen/Senses\|Senses]]                       | [[PF2e Journals/GM Screen/Detecting Creatures\|Detecting Creatures]] | [[PF2e Journals/GM Screen/Detecting and Stealth with Other Senses\|Detecting and Stealth with Other Senses]] |
|       [[PF2e Journals/GM Screen/Exploration Activities\|Exploration Activities]]       |         [[PF2e Journals/GM Screen/Hero Points\|Hero Points]]         |                                  [[PF2e Journals/GM Screen/Traits\|Traits]]                                  |
|          [[PF2e Journals/GM Screen/Bulk and Encumbered\|Bulk and Encumbered]]          |        [[PF2e Journals/GM Screen/Summon Trait\|Summon Trait]]        |                               [[PF2e Journals/GM Screen/Attitudes\|Attitudes]]                               |

> [!example]- Exploration Activities
>| General Exploration Activities                                            | Description                                                                            |
| --------------------------------------------------- | ------------------------------------------------------------------------------- |
| [[Avoid Notice]]                                    | Travel stealthitly at half speed and use Stealth for initiative                 |
| [[Defend]]                                          | Move at half speed with your shield raised.                                     |
| [[2. Mechanics/Actions/Detect Magic\|Detect Magic]] | Cast [[Spells/Detect Magic\|Detect Magic]] regularly while moving at half speed |
| [[Follow the Expert]]                               | Match the tactic of an expert to gain a bonus to a skill check                  |
| [[2. Mechanics/Actions/Hustle]]                                          | Move at double speed for Con (min. 1) x 10 minutes                              |
| [[Investigate]]                                     | Seek out information about your surroundings at half speed.                     |
| [[Refocus]]                                         | Perform deeds to restore 1 focus point to your focus pool                       |
| [[Repeat a Spell]]                                  | Cast the same spell (usually a cantrip) repeatedly at half speed.               |
| [[2. Mechanics/Actions/Scout\|Scout]]               | Scout ahead and behind to watch for danger at half speed.                       |
| [[2. Mechanics/Actions/Search]]                                          | Seek meticulously for hidden features at half speed (or slower)                 | 
>
>| Skill Exploration Activities                                               | Description                                                                                 |
| -------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| [[Borrow an Arcane Spell]]                                                 | Prepare a spell from someone else's spellbook (Arcana)                                      |
| [[Coerce]]                                                                 | Threaten a creature so it does waht you want (Intimidation)                                 |
| [[Cover Tracks]]                                                           | Obscure your passing (Survival)                                                             |
| [[Decipher Writing]]                                                       | Understand archaic, esoteric, or obscure texts (Arcana, Occultism, Religion, Society)       |
| [[Gather Information]]                                                     | Canvass the area to learn about an individual/topic (Diplomacy)                             |
| [[Identify Alchemy]]                                                       | Identify an alchemical item using alchemist's tools (Crafting)                              |
| [[Identify Magic]]                                                         | Learn about a magic item, location, or ongoing effect (Arcana, Nature, Occultism, Religion) | 
| [[Impersonate]]                                                            | Create a disguise, usually with a disguise kit (Deception)                                  |
| [[Learn a Spell]]                                                          | Gain access to a new spell (Arcana, Nature, Occultism, Religion)                            |
| [[Make an Impression]]                                                     | Make a good impression on someone (Diplomacy)                                               |
| [[Repair]]                                                                 | Fix a damaged item using a repair kit (Crafting)                                            |
| [[Sense Direction]]                                                        | Get a sense of where you are and where is north (Survival)                                  |
| [[Squeeze]]                                                                | Squeeze through very tight spaces (Acrobatics)                                              |
| [[2. Mechanics/Actions/Skill Actions/Survival/Track]]                                                                  | Find and follow creatures' tracks (Survival)                                                |
| [[2. Mechanics/Actions/Skill Actions/Medicine/Treat Wounds\|Treat Wounds]] | Treat a living creature's woudns (Medicine)                                                 |

> [!example]- Downtime Activities
> | Downtime Activities                             | Traveler                                                                 |
| ----------------------------------------------- | ------------------------------------------------------------------------ |
| [[Crafting (Int)\|Craft]]                       | Create items from raw materials (Crafting)                               |
| [[Create Forgery]]                              | Forge a document (Deception)                                             |
| [[Earn Income]]                                 | Earn money (Crafting, Lore, Performance)                                 |
| Long Term Rest                                  | Spend an entire day resting to recovery Con (min. 1) x twice your level. |
| [[2. Mechanics/Actions/Retraining\|Retraining]] | Alter some of your character choices (feats, skills, class features)     |
| [[Subsist]]                                     | Find food/shelter in the wilderness (survival) or a settlement (Society) |
| [[Treat Disease]]                               | Spend time caring for a diseased creature to cure them (Medicine)        |



## Wardens of Iron
![[Party View.base]]



## The  Rough-Hewn Rangers

```dataview
TABLE WITHOUT ID link(file.name) AS "Character Name",Player, Class, Race, level, Role
from "0. The Party/The Rough-hewn Rangers"
where (Role = "Player")
sort ASC
```

# Recently Modified Notes
```dataview
TABLE WITHOUT ID
	link(file.path, file.folder + " / " + file.name) AS "Note",
	file.mtime AS "Last modified"
FROM "/"
WHERE file.mtime >= date(today) - dur(30 days)
AND file.name != this.file.name
	AND !contains(file.path, "z_Assets")
	AND !contains(file.path, "Inline Scripts")
	AND !contains(file.path, "z_Templates")
	AND !contains(file.path, "BRAT")
SORT file.mtime DESC
LIMIT 10
```







