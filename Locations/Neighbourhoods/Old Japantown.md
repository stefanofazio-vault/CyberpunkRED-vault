#### Old Japantown
```zoommap
image: vault_maps/old_japantown.png
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
ZOOMMAP-DATA id=map-0
{
  "size": {
    "w": 4073,
    "h": 3388
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
      "id": "marker_4uudfa",
      "x": 0.3100005683209578,
      "y": 0.370094470270114,
      "layer": "default",
      "link": "Basement",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/old_japantown.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/old_japantown.png",
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
%%
ZOOMMAP-DATA id=map-1
{
  "size": {
    "w": 4073,
    "h": 3388
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
      "id": "marker_4uudfa",
      "x": 0.3100005683209578,
      "y": 0.36871675474256527,
      "layer": "default",
      "link": "Basement",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_brel7e",
      "x": 0.26344314320893475,
      "y": 0.3711277831940149,
      "layer": "default",
      "link": "Bodukkan",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_igdh7y",
      "x": 0.4617059961830203,
      "y": 0.49099087356750754,
      "layer": "default",
      "link": "Crisis Medical Center",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_38xic5",
      "x": 0.35512537118585547,
      "y": 0.4138376477822481,
      "layer": "default",
      "link": "Cutting Edge",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hx140j",
      "x": 0.4230274688202707,
      "y": 0.4992572718457572,
      "layer": "default",
      "link": "Dine'n'Dash",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ywcvp5",
      "x": 0.30183505868727306,
      "y": 0.2764083953718765,
      "layer": "default",
      "link": "Gazebo",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ae49kp",
      "x": 0.5147096967971915,
      "y": 0.23163195749232018,
      "layer": "default",
      "link": "Grateful Crane",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_sj2602",
      "x": 0.4376393413910897,
      "y": 0.25712011520380096,
      "layer": "default",
      "link": "Highcourt Plaza Hotel",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_yn9vfz",
      "x": 0.505541526460491,
      "y": 0.4996017270058837,
      "layer": "default",
      "link": "Honest Hiro's Used Cars",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2yk4gn",
      "x": 0.39953403779716257,
      "y": 0.44070346846479896,
      "layer": "default",
      "link": "Imperial Bank",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/old_japantown.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/old_japantown.png",
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
