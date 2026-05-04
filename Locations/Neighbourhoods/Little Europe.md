
```zoommap
image: vault_maps/little_europe.png
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
    "h": 3516
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
      "id": "marker_kcxk0p",
      "x": 0.41149818210359024,
      "y": 0.34285455734008413,
      "layer": "default",
      "link": "101.1 Killzone",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ufuz4g",
      "x": 0.32158116322885005,
      "y": 0.2143728110001297,
      "layer": "default",
      "link": "Biotechnica Reference Forest RF-14",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2pt68s",
      "x": 0.2886145588502118,
      "y": 0.2824490854844986,
      "layer": "default",
      "link": "Bristol Business Park",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_su4p40",
      "x": 0.513647467000047,
      "y": 0.14795693345440397,
      "layer": "default",
      "link": "Camden's Court",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_f9akzs",
      "x": 0.6168472720114366,
      "y": 0.5431314048514723,
      "layer": "default",
      "link": "Chopper's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tu4tbe",
      "x": 0.459180903244036,
      "y": 0.4468283824101699,
      "layer": "default",
      "link": "Continental Brands Vertical Neighborhood",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/little_europe.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/little_europe.png",
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
  },
  "deleted": [
    {
      "id": "undo_0pmh15",
      "label": "Delete pin",
      "createdAt": "2026-05-04T10:47:02.384Z",
      "payload": {
        "kind": "marker",
        "marker": {
          "type": "pin",
          "id": "marker_xqnxjq",
          "x": 0.31855773144140703,
          "y": 0.21403554287196783,
          "layer": "default",
          "link": "Born This Way",
          "iconKey": "pinRed",
          "tooltip": "",
          "scaleLikeSticker": true
        },
        "index": 1
      }
    }
  ]
}
/ZOOMMAP-DATA
%%

