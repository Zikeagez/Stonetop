---
tags:
  - Category/Hub
MyContainer:
MyCategory: Hamlet <80
obsidianUIMode: preview
image: "Zelkor's Ferry.png"
---

%% CODE BELOW IS TEMPLATER CODE. IT TRIGGERS THIS CODE WHEN THE NOTE IS CREATED USING THE META-BIND BUTTONS %% 
<%*

// 1) Rename if title starts with "NewHub"
let title;
if (tp.file.title.startsWith("NewHub")) {
  title = await tp.system.prompt("Enter Hub Name");
  if (!title) {
    new Notice("No name entered. Aborting.");
    return;
  }
  await tp.file.rename(title);
} else {
  title = tp.file.title;
}

// 2) Gather all region files under 1. World/Regions
const regionFiles = tp.app.vault.getMarkdownFiles()
  .filter(f => f.path.startsWith("1. World/Regions/"));

const placeholderLabel = "🌀 No Region Selected";
const placeholderPath = "__placeholder__";

// 3) Suggester for picking region (with placeholder)
const regionChoices = [placeholderLabel, ...regionFiles.map(f => f.basename)];
const regionValues  = [placeholderPath, ...regionFiles.map(f => f.path)];
const chosenPath    = await tp.system.suggester(regionChoices, regionValues, true);
if (!chosenPath) return;

// 4) Build the wiki-link or fallback
let wikiLink = null;
if (chosenPath !== placeholderPath) {
  const chosenAlias = chosenPath.split("/").pop().replace(/\.md$/, "");
  wikiLink = `[[${chosenPath}|${chosenAlias}]]`;
}

// 5) Prompt for Hub type (MyCategory)
const categoryOptions = [
  "City +1500",
  "Town +200",
  "Village +80",
  "Hamlet <80",
  "Encampment",
  "Keep",
  "Fortress",
  "Stronghold"
];
const chosenCat = await tp.system.suggester(categoryOptions, categoryOptions, true);
if (!chosenCat) return;

// 6) Write both properties into frontmatter
setTimeout(() => {
  const newFile = tp.file.find_tfile(tp.file.path(true));
  if (!newFile) return;
  app.fileManager.processFrontMatter(newFile, fm => {
    fm["MyContainer"] = wikiLink ?? "None";
    fm["MyCategory"]  = chosenCat;
  });
}, 100);

%>


> [!NOTE|div-m] Parent Region: `INPUT[inlineListSuggester(optionQuery(#Category/Region)):MyContainer]`
%% DISPLAYS NOTES THAT MATCH THE TAGS ABOVE %% 

> [!column|no-i no-t]
>> [!info|no-title] Map
>> ```leaflet  
>> id: ZalkorsFerry ### Must be unique with no spaces  
>> image: [[Zelkor's Ferry.png]] ### Link to the map image file. Do not add a ! in front of the image  
>> bounds: [[0,0], [5000, 4025]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
>> height: 500px ### Size of the leaflet embed in px on your screen  
>> width: 95% ### Size of the leaflet embed in your note  
>> lat: 2500 ### To center the map, make this half of the map height.  
>> long: 2012.5 ### To center the map, make this half of the map width.  
>> minZoom: -3 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
>> maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
>> defaultZoom: -3 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
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
>> option(1, ℹ️General),
>> option(2, 🏃‍♂️‍➡️NPCs),
>> option(3, 📝GM Notes),
>> option(4, 🐎Travel),
>> class(tabbed)
>> )]
>> ~~~
>>>[!tabbed-box-maxh]
>>> >[!div-m|no-title]
>>> > ![[#General|no-h clean]]
>>>
>>> >[!div-m|no-title]
>>> > ![[#NPCs|no-h clean]]
>>>
>>> > [!div-m|no-title]
>>> > ![[#GM Notes|no-h clean]]
>>> 
>>> > [!div-m|no-title]
>>> > ![[#Travel|no-h clean]]
>>> 

> [!NOTE|no-title]
> ~~~meta-bind
> INPUT[select(
> option(1, 🛒Commerce),
> option(2, 🍎Agriculture),
> option(3, ⚔️Military),
> option(4, 💭Philosophy),
> option(5, ⚙️Industrial),
> option(6, 🏠Nesting),
> option(7, 👑Government),
> class(tabbed)
> )]
> ~~~
> >[!tabbed-box]
> > >[!div-m|no-title]
> > > ![[#Commerce|no-h clean]]
> >
> > > [!div-m|no-title]
> > > ![[#Agriculture|no-h2 clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Military|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Philosophy|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Industrial|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Nesting|no-h clean]]
> > 
> > > [!div-m|no-title]
> > > ![[#Government|no-h clean]]

---
# General

Select Settlement: `INPUT[suggester(optionQuery(#Category/Region)):MyContainer]`
%% DISPLAYS NOTES THAT MATCH THE TAGS ABOVE %% 

Select Category: `INPUT[template-hub-category][:MyCategory]`
%% MODIFY OPTIONS IN SETTINGS > COMMUNITY PLUGINS > META-BIND > EDIT TEMPLATES > template-hub-category %%

This is the town description. 

# NPCs

`BUTTON[button_person]` List important NPCs here. 

```base
formulas:
  LinkedViaPlace: |
    list(MyContainer)                                          
      .filter( file(value)                                     
               && list(file(value).properties.MyContainer)     
                    .contains(this) )                          
      .length > 0
  PlacesForThis: |
    list(MyContainer)
      .filter( file(value)
               && list(file(value).properties.MyContainer).contains(this) )
      .map( link(value, file(value).name) )
properties:
  file.name:
    displayName: Person
  PlacesForThis:
    displayName: Places (for this note)
  note.char_race:
    displayName: Race
  note.char_gender:
    displayName: Gender
  note.char_age:
    displayName: Age
views:
  - type: cards
    name: People linked via Places → this note
    filters:
      and:
        - file.inFolder("1. World/People")
        - formula.LinkedViaPlace
    order:
      - file.name
      - char_age
      - char_gender
      - char_race
    image: note.image
    cardSize: 100
  - type: table
    name: View

```

# GM Notes

Make notes of what you need to track in the town here. 

# Travel

%% For every other hub/location that you would like to see travel time to, add a line in the table and replicate the format provided. Change the Town name and link it to that towns note and then change the 88 in the formula to match the distance in miles to that place. Use a Leaflet map to measure the distance. %%

`VIEW[{Travel Calculator#HoursPerDay}][math]` hrs per day
[[Travel Calculator]]  / [[Exhaustion]] Level: `VIEW[{Travel Calculator#ExhaustionLevel}][math]`

| Destination |  Travel Days  |
| ---|---|
| [[Next Town A]] | 🕓: `VIEW[round((88* {Travel Calculator#TravelCalc}) / 60 / {Travel Calculator#HoursPerDay}, 1)]`      |
| [[Next Town B ]] | 🕓: `VIEW[round((88* {Travel Calculator#TravelCalc}) / 60 / {Travel Calculator#HoursPerDay}, 1)]`

# CAMPING 

C - Commerce (Economics and Entertainment) - Shops, Malls, Theatres, Markets, Carnivals, Electronics
A - Agriculture (Resource Production and Collection) - Farms, Mines, Fisheries, Lumber Yards, Oil Rigs, Power Plants
M - Military (Protection and Transportation) - Forts, Bases, Armories, Walls, Seaports, Airports, Spaceports
P - Philosophy (Religion and Education) - Houses of Worship, Schools, Universities, Laboratories, Arboretums
I - Industrial (Resource Utilization and Processing) - Factories, Metalworks, Bakeries, Artisans, Jewelers
N - Nesting (Housing and Civil Engineering) - Residential Areas, Inns/Hotels
G - Government (Legislation and Judicial) - Town Halls, Courthouses, Tourist Stops, Monuments/Landmarks

## Commerce

`BUTTON[button_place]` `BUTTON[button_person]` **C - Commerce** (Economics and Entertainment) - Shops, Malls, Theatres, Markets, Carnivals, Electronics

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Commerce"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Commerce"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```


## Agriculture

`BUTTON[button_place]` `BUTTON[button_person]` **A - Agriculture** (Resource Production and Collection) - Farms, Mines, Fisheries, Lumber Yards, Oil Rigs, Power Plants

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Agriculture"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Agriculture"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

## Military

`BUTTON[button_place]` `BUTTON[button_person]` **M - Military** (Protection and Transportation) - Forts, Bases, Armories, Walls, Seaports, Airports, Spaceports

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Military"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Military"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

## Philosophy

`BUTTON[button_place]` `BUTTON[button_person]` **P - Philosophy** (Religion and Education) - Houses of Worship, Schools, Universities, Laboratories, Arboretums

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Philosophy"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Philosophy"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

## Industrial

`BUTTON[button_place]` `BUTTON[button_person]` **I - Industrial** (Resource Utilization and Processing) - Factories, Metalworks, Bakeries, Artisans, Jewelers

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Industrial"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Industrial"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

## Nesting

`BUTTON[button_place]` `BUTTON[button_person]` **N - Nesting** (Housing and Civil Engineering) - Residential Areas, Bridges, Parks, Inns/Hotels

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Nesting"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Nesting"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```

## Government

`BUTTON[button_place]` `BUTTON[button_person]` **G - Government** (Legislation and Judicial) - Town Halls, Courthouses, Tourist Stops, Monuments/Landmarks

```base
properties:
  file.name:
    displayName: Places Name
  note.MyCategory:
    displayName: Type of Place
views:
  - type: cards
    name: Region - Cards
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Government"
    order:
      - file.name
      - MyCategory
    image: note.image
  - type: table
    name: Region - Table
    filters:
      and:
        - file.folder == "1. World/Places"
        - list(MyContainer).contains(this)
        - MyCategory == "Government"
    order:
      - file.name
      - MyContainer
    sort:
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 182

```




