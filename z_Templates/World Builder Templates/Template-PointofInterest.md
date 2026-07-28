---
tags:
  - Category/Planet
obsidianUIMode: preview
MyContainer:
image: "Template_Planet_Placeholder.png"
---
<%*

// 1) Rename if the file starts with "NewPlanet"
let title;
if (tp.file.title.startsWith("NewPlanet")) {
title = await tp.system.prompt("Enter Planet Name");
if (!title) {
  new Notice("No name entered. Aborting.");
  return;
}
await tp.file.rename(title);
} else {
title = tp.file.title;
}

// 2) Get all Star System notes from folder
const systemFiles = tp.app.vault.getMarkdownFiles()
.filter(f => f.path.startsWith("1. World/Star Systems/"));

const placeholderLabel = "🌀 No Star System Selected";
const placeholderPath = "__placeholder__";

// Combine options
const systemChoices = [placeholderLabel, ...systemFiles.map(f => f.basename)];
const systemValues = [placeholderPath, ...systemFiles.map(f => f.path)];

// 3) Prompt user to pick a Star System
const chosenPath = await tp.system.suggester(systemChoices, systemValues, true);
if (!chosenPath) return;

// 4) Build the wiki-link or set fallback
let wikiLink = null;
if (chosenPath !== placeholderPath) {
const chosenAlias = chosenPath.split("/").pop().replace(/\.md$/, '');
wikiLink = `[[${chosenPath}|${chosenAlias}]]`;
}

// 5) Write to frontmatter
setTimeout(() => {
const newFile = tp.file.find_tfile(tp.file.path(true));
if (!newFile) {
  new Notice("Could not find file after rename.");
  return;
}
app.fileManager.processFrontMatter(newFile, fm => {
  fm["MyContainer"] = wikiLink ?? "None";
});
}, 200);

%>



> [!NOTE] Parent Star System: `INPUT[suggester(optionQuery(#Category/StarSystem)):MyContainer]`

> [!column|no-i no-t]
>> [!info|no-title] Map
>> ![[Template_Planet_Placeholder.png]]
>
>> [!note|no-title] Town Name
>> ~~~meta-bind
>> INPUT[select(
>> option(1, ℹ️General Info),
>> option(2, 🌐Planet Details),
>> option(3, 📝GM Notes),
>> class(tabbed)
>> )]
>> ~~~
>>>[!tabbed-box-maxh]
>>> >[!div-m|no-title]
>>> > ![[#General Info|no-h clean]]
>>>
>>> >[!div-m|no-title]
>>> > ![[#Planet Details|no-h clean]]
>>>
>>> > [!div-m|no-title]
>>> > ![[#GM Notes|no-h clean]]
>>> 

> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🗺️Continents),
> option(2, 👽Sapient Species),
> option(3, ⚔️Capital Cities),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box]
> > >[!div-m|no-title]
> > > ![[#Continents|no-h clean]]
> >
> > > [!div-m|no-title]
> > > ![[#Sapient Species|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Capital Cities|no-h clean]]
> > 

---
# General Info

This is the planet description. 

# Planet Details

**Dominant Races:**  
**Climate:** 
**Seasons:**

# GM Notes

Make notes of what you need to track in the region here. 

# Continents

`BUTTON[button_continent]` **Continents**  Large continuous landmasses that contain regions.

```base
properties:
  file.name:
    displayName: Continent(s)
views:
  - type: cards
    name: Continents - Cards
    filters:
      and:
        - file.folder == "1. World/Continents"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: Continents - Table
    filters:
      and:
        - file.folder == "1. World/Continents"
        - list(MyContainer).contains(this)
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC
    columnSize:
      file.name: 182

```

# Sapient Species

`BUTTON[button_species]`  Intelligent species that live on this planet. 

```base
properties:
  file.name:
    displayName: Sapient Species(s)
views:
  - type: cards
    name: Sapient Species - Cards
    filters:
      and:
        - file.folder == "1. World/Sapient Species"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: Sapient Species - Table
    filters:
      and:
        - file.folder == "1. World/Sapient Species"
        - list(MyContainer).contains(this)
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC
    columnSize:
      file.name: 182

```

# Capital Cities

`BUTTON[button_hub]` Groups of people and power - religious, cults, guilds, military

```base
filters:
  and:
    - formula.LinkedToThisPlanet
    - MyContainer.contains(this)
formulas:
  LinkedToThisPlanet: |
    list(MyContainer)
      .filter(
        file(value)
        && list(file(value).properties.MyContainer)
             .filter(
               file(value)
               && list(file(value).properties.MyContainer)
                    .contains(this)
             ).length > 0
      ).length > 0
properties:
  file:
    displayName: Hub
  MyCategory:
    displayName: Type
  MyContainer:
    displayName: Region(s)
views:
  - type: cards
    name: Capital Cities (Cards)
    filters:
      and:
        - file.inFolder("1. World/Hubs")
        - list(MyCategory).contains("City +1500")
    order:
      - file
      - MyCategory
      - MyContainer
    image: note.image
  - type: table
    name: Capital Cities (List)
    filters:
      and:
        - file.inFolder("1. World/Hubs")
        - formula.LinkedToThisPlanet
        - list(MyCategory).contains("City +1500")
    order:
      - file
      - MyCategory
      - MyContainer

```
