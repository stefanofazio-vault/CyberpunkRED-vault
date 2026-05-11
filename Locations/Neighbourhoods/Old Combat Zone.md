#### Old Combat Zone
```zoommap
image: vault_maps/old_combat_zone.png
# markers is optional; defaults to <image>.markers.json
# markers: Assets/Map.jpg.markers.json

# Map view limits
minZoom: 0.3
maxZoom: 8

# Size & interactivity
height: 560px
width: 100%
resizable: true
resizeHandle: native     # left | right | both | native
render: canvas           # or: dom

# Responsive display (fit into width, no wheel/pinch/dblclick pan/zoom)
responsive: true        # true → always fit; disables pan/zoom gestures

# Storage (optional)
# storage: note          # default is json; use "note" to store markers inline
# id: map-1              # optional stable id for inline storage (per code block)

# Alignment / wrapping (optional)
align: right             # left | center | right
wrap: true               # wrap text; useful with left/right alignment
```
%%
ZOOMMAP-DATA id=map-1
{
  "size": {
    "w": 4073,
    "h": 3454
  },
  "layers": [
    {
      "id": "default",
      "name": "Default",
      "visible": true,
      "locked": false
    }
  ],
  "markers": [
    {
      "type": "pin",
      "id": "marker_r3vjmw",
      "x": 0.5964026905211718,
      "y": 0.16097949613100299,
      "layer": "default",
      "link": "Alice's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_i5wuyg",
      "x": 0.5166522978819177,
      "y": 0.6527258008221515,
      "layer": "default",
      "link": "Always Hot",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_afwpps",
      "x": 0.3107893602164219,
      "y": 0.6567646698439364,
      "layer": "default",
      "link": "The Arena",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mzrv3k",
      "x": 0.5931619239137259,
      "y": 0.24099136963650078,
      "layer": "default",
      "link": "Bladeware",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_f862ab",
      "x": 0.45440757273377547,
      "y": 0.2063109765153778,
      "layer": "default",
      "link": "Farnsworth Building",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_0t83ub",
      "x": 0.5074297751403026,
      "y": 0.3264375481664964,
      "layer": "default",
      "link": "Flasher's Corner",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fwlxuv",
      "x": 0.5562777805919081,
      "y": 0.16156842695442522,
      "layer": "default",
      "link": "From The Ashes",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_m3ddhe",
      "x": 0.7609518015863737,
      "y": 0.24672014007270973,
      "layer": "default",
      "link": "NC Ionic Semiconductor Building",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bfqk68",
      "x": 0.423130658864353,
      "y": 0.6739576336986423,
      "layer": "default",
      "link": "Jesse James' Kosher Deli",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/old_combat_zone.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/old_combat_zone.png",
  "measurement": {
    "displayUnit": "km",
    "scales": {},
    "customUnitPxPerUnit": {},
    "travelTimePresetIds": [],
    "travelDaysEnabled": false
  },
  "pinSizeOverrides": {
    "pinRed": 168
  },
  "grids": [],
  "panClamp": true,
  "drawLayers": [],
  "drawings": [],
  "textLayers": [],
  "secondScreen": {
    "showGrids": true
  }
}
/ZOOMMAP-DATA
%%
