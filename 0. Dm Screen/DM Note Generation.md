---
obsidianUIMode: preview
---

```base
formulas:
  Untitled: ""
  TestForm: ""
  Untitled 2: char_age.
properties:
  property.char_race:
    displayName: Race
  property.char_gender:
    displayName: Gender
  property.char_status:
    displayName: Status
  property.char_class:
    displayName: Class
  property.char_age:
    displayName: Age
  property.char_items:
    displayName: Inventory
  file.name:
    displayName: Character Name
  property.Player:
    displayName: Player Name
  property.level:
    displayName: Level
  note.char_status:
    displayName: Character Status
  note.char_race:
    displayName: Race
  note.char_gender:
    displayName: Gender
  note.char_items:
    displayName: Items
  note.char_age:
    displayName: Age
  note.level:
    displayName: Level
  note.char_class:
    displayName: Class
views:
  - type: table
    name: Party View - Tables
    filters:
      and:
        - tags.contains("Category/Player")
        - file.folder != "z_Templates/1_Story World Templates"
    order:
      - file.name
      - Player
      - level
      - hp
      - ac
      - char_class
    image: note.image
  - type: cards
    name: Party Members
    filters:
      and:
        - tags == ["Category/Player"]
        - file.folder != "z_Templates/World Builder Templates"
    order:
      - file.name
      - Player
      - level
      - char_race
      - char_gender
      - char_status
      - char_class
      - char_age
      - ac
      - hp
      - pasperc
    image: note.image

```


`BUTTON[button_journal]` `BUTTON[button_player]`
%% These are Inline Buttons. Inline allows the buttons to be placed on the same line next to each other. Button's are defined within the Meta Bind Plugin. See Button Templates. %%
`BUTTON[button_galaxy]` `BUTTON[button_starsystem]` `BUTTON[button_planet]`

`BUTTON[button_continent]` `BUTTON[button_region]` `BUTTON[button_pointofinterest]`

`BUTTON[button_hub]` `BUTTON[button_place]` `BUTTON[button_person]`

`BUTTON[button_species]` `BUTTON[button_item]`

`BUTTON[button_group]` `BUTTON[button_quest]` 

## Known Languages

%% This will scan the player notes for any known languages and list the unique languages that the party know here. This is handy to determine quickly if the party can understand someone. %%

```dataviewjs
dv.list(dv.pages()
		.where(p => p.Status && p.Status.includes("Active") && p.Role && p.Role.includes("Player"))
		.PlayerKnownLanguages.distinct())
```
