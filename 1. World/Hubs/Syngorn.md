---
tags:
  - Category/Hub
MyContainer: "[[1. World/Regions/Verdant Expanse.md|Verdant Expanse]]"
MyCategory: City +1500
obsidianUIMode: preview
image: Zelkor's Ferry.png
---

%% CODE BELOW IS TEMPLATER CODE. IT TRIGGERS THIS CODE WHEN THE NOTE IS CREATED USING THE META-BIND BUTTONS %% 



> [!NOTE|div-m] Parent Region: `INPUT[inlineListSuggester(optionQuery(#Category/Region)):MyContainer]`
%% DISPLAYS NOTES THAT MATCH THE TAGS ABOVE %% 

> [!column|no-i no-t]
>> [!info|no-title] Map
>> ```leaflet  
>> id: ZalkorsFerry ### Must be unique with no spaces  
>> image: [[Map - Syngorn.webp]] ### Link to the map image file. Do not add a ! in front of the image  
>> bounds: [[0,0], [746, 1118]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
>> height: 500px ### Size of the leaflet embed in px on your screen  
>> width: 95% ### Size of the leaflet embed in your note  
>> lat: 373 ### To center the map, make this half of the map height.  
>> long: 559 ### To center the map, make this half of the map width.  
>> minZoom: -3 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
>> maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
>> defaultZoom: -.5 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
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


_Syngorn is an ancient elven sanctuary_ and the largest elven city within the continent of Tal'Dorei.




For non-elves there are some options for inns, but he recommends the Oaken Cup which is in the Tarn Ward west of the Spellbinder's Hall.

Business is usually conducted after sunset.


Spellbinder's Guildhall -  Pinnacle of Elven Magic


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




