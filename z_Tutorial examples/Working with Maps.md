# Plugins
Obsidian Leaflet (have This already)

# Templates 
![[Insert Map (Leaflet)]]
![[Instert Map DUNGEON (Leaflet)]]

# Example

## Region
```leaflet
id: exampleregion1
image: [[elturgard.jpg]]
height: 500px
lat: 50
long: 50
minZoom: 1
maxZoom: 10
defaultZoom: 100
unit: meters
scale: 1
marker: default, 39.983334, -82.983330, [[Note]]
darkMode: false
```

## Dungeon


```leaflet
### Tutorial: https://youtu.be/54EyMzJP5DU
### id must be unique
id: exampledungeon
image: [[Map - Cult Ritual Site.png]]
height: 800px
width: 85%
### This sets where the map starts by default. Set it to the middle (half) of your bounds.
lat: 50
long: 50
### 0 is no zoom. Negative zoom steps away from the map. Positive zoom steps towards the map.
minZoom: 0
### Max zoom is 18
maxZoom: 18
### Hover mouse over the Reset Zoom icon to see your current zoom level.
defaultZoom: 17.5
### How far it zooms in or out with each step. Can be in decimals.
zoomDelta: 0.5
### This is a string so can be any text. Change it to match your maps measurement scale.
unit: feet
scale: 1
darkMode: false
```
