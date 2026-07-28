---
tags:
  - Category/Region
obsidianUIMode: preview
MyContainer:
image: "The Island of Screams.jpg"
---
<%*

// 1) Rename if title starts with "NewRegion"
let title;
if (tp.file.title.startsWith("NewRegion")) {
  title = await tp.system.prompt("Enter Region Name");
  if (!title) {
    new Notice("No title entered. Aborting.");
    return;
  }
  await tp.file.rename(title);
} else {
  title = tp.file.title;
}

// 2) Gather all continent files under 1. World/Continents/
const continentFiles = tp.app.vault.getMarkdownFiles()
  .filter(f => f.path.startsWith("1. World/Continents/"));

if (continentFiles.length === 0) {
  new Notice("No continent notes found.");
  return;
}

const placeholderLabel = "🌀 No Continent Selected";
const placeholderPath = "__placeholder__";

// 3) Prompt user to choose container
const continentChoices = [placeholderLabel, ...continentFiles.map(f => f.basename)];
const continentValues  = [placeholderPath, ...continentFiles.map(f => f.path)];
const chosenPath       = await tp.system.suggester(continentChoices, continentValues, true);
if (!chosenPath) return;

// 4) Build the wiki-link or fallback
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

> [!NOTE] Parent Continent: `INPUT[suggester(optionQuery(#Category/Continent)):MyContainer]`

> [!column|no-i no-t]
>> [!info|no-title] Map
>> ```leaflet  
>> id: ZalkorsFerry ### Must be unique with no spaces  
>> image: [[The Island of Screams.jpg]] ### Link to the map image file. Do not add a ! in front of the image  
>> bounds: [[0,0], [5888, 5882]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
>> height: 500px ### Size of the leaflet embed in px on your screen  
>> width: 95% ### Size of the leaflet embed in your note  
>> lat: 2944 ### To center the map, make this half of the map height.  
>> long: 2941 ### To center the map, make this half of the map width.  
>> minZoom: -5 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
>> maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
>> defaultZoom: -3.5 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
>> zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out.  
>> unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
>> scale: 0.09328358208955223 ### Real units/px (resolution) of your map  
>> recenter: false  
>> darkmode: false ### marker
>> ```
>
>> [!note|no-title] Town Name
>> ~~~meta-bind
>> INPUT[select(
>> option(1, ℹ️General Info),
>> option(2, 🌐Region Details),
>> option(3, 📝GM Notes),
>> class(tabbed)
>> )]
>> ~~~
>>>[!tabbed-box-maxh]
>>> >[!div-m|no-title]
>>> > ![[#General Info|no-h clean]]
>>>
>>> >[!div-m|no-title]
>>> > ![[#Region Details|no-h clean]]
>>>
>>> > [!div-m|no-title]
>>> > ![[#GM Notes|no-h clean]]
>>> 

> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🏡Hubs),
> option(2, 🍎Points of Interest),
> option(3, ⚔️Groups),
> option(4, 💭Quests),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box]
> > >[!div-m|no-title]
> > > ![[#Hubs|no-h clean]]
> >
> > > [!div-m|no-title]
> > > ![[#Points of Interest|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Groups|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Quests|no-h clean]]

---
# General Info

This is the region description. 

# Region Details

**Dominant Races:**  
**Climate:** 
**Seasons:**

# GM Notes

Make notes of what you need to track in the region here. 

# Hubs

`BUTTON[button_hub]` **Hubs** Places where people live - Cities, Towns, Villages, Hamlets, Encampment, Keeps, Fortresses, Strongholds.

```base
properties:
  file.name:
    displayName: Hub Name
views:
  - type: cards
    name: Hubs - Cards
    filters:
      and:
        - file.folder == "1. World/Hubs"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: Hubs - Table
    filters:
      and:
        - file.folder == "1. World/Hubs"
        - list(MyContainer).contains(this)
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

# Points of Interest

`BUTTON[button_pointofinterest]`  Places that can be explored. 

```base
properties:
  file.name:
    displayName: Hub Name
views:
  - type: cards
    name: POIs - Cards
    filters:
      and:
        - file.folder == "1. World/Points of Interest"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: POIs - Table
    filters:
      and:
        - file.folder == "1. World/Points of Interest"
        - list(MyContainer).contains(this)
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

# Groups

`BUTTON[button_group]` Groups of people and power - religious, cults, guilds, military

```base
properties:
  file.name:
    displayName: Hub Name
views:
  - type: cards
    name: Groups - Cards
    filters:
      and:
        - file.folder == "1. World/Groups"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: Groups - Table
    filters:
      and:
        - file.folder == "1. World/Groups"
        - list(MyContainer).contains(this)
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

# Quests

`BUTTON[button_quest]` **P - Philosophy** (Religion and Education) - Houses of Worship, Schools, Universities, Laboratories, Arboretums

```base
properties:
  file.name:
    displayName: Hub Name
views:
  - type: cards
    name: Quests - Cards
    filters:
      and:
        - file.folder == "1. World/Quests"
        - list(MyContainer).contains(this)
    order:
      - file.name
    image: note.image
  - type: table
    name: Quests - Table
    filters:
      and:
        - file.folder == "1. World/Quests"
        - list(MyContainer).contains(this)
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

