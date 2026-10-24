
```zoommap
image: z_Assets/Maps/Map - The Setting.webp
# markers is optional; defaults to <image>.markers.json
# markers: Assets/Map.jpg.markers.json

# Map view limits
minZoom: 0.3
maxZoom: 8

# Size & interactivity
height: 760px
width: 100%
resizable: true
resizeHandle: native    
render: canvas           

# Image interpolation: auto | pixelated | crisp-edges
imageRendering: pixelated

# Responsive display (fit into width, no wheel/pinch/dblclick pan/zoom)
responsive: false        # true → always fit; disables pan/zoom gestures


# Alignment / wrapping (optional)
align: right             # left | center | right
wrap: true               # wrap text; useful with left/right alignment
```
