#### Heywood Docks
```zoommap
image: vault_maps/heywood_docks.png
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
    "h": 4059
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
      "id": "marker_g5z1wv",
      "x": 0.5999007295285577,
      "y": 0.17141582739518274,
      "layer": "default",
      "link": "The Cylinders",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_9r9j89",
      "x": 0.6454866449481789,
      "y": 0.41563110899633765,
      "layer": "default",
      "link": "Decker, Tanaka & Rogers",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_uockak",
      "x": 0.2735728427490425,
      "y": 0.5725470674536712,
      "layer": "default",
      "link": "Dockside Billhooks Track",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_xqvabo",
      "x": 0.3029036394045789,
      "y": 0.6318519011731728,
      "layer": "default",
      "link": "Greenbox Storage Units",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zqferg",
      "x": 0.6750071519725456,
      "y": 0.3758877399165483,
      "layer": "default",
      "link": "HF&S Construction",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_29f6or",
      "x": 0.6159061649685048,
      "y": 0.318771530072535,
      "layer": "default",
      "link": "LoadStar Continental Shipping",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_7q2sr6",
      "x": 0.45261746734081154,
      "y": 0.5353622613993366,
      "layer": "default",
      "link": "Rail Yard",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_lf9rr8",
      "x": 0.33672139226741404,
      "y": 0.5027455941536806,
      "layer": "default",
      "link": "Shipping Yard",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_9tug4v",
      "x": 0.5393077622690076,
      "y": 0.3477024471601972,
      "layer": "default",
      "link": "SK Securities",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wv6yuh",
      "x": 0.6298553847979059,
      "y": 0.2347821403168581,
      "layer": "default",
      "link": "Warehouse 13",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/heywood_docks.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/heywood_docks.png",
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
