#### Porto di Night City
```zoommap
image: vault_maps/port_night_city.png
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
    "h": 3867
  },
  "layers": [
    {
      "id": "default",
      "name": "Default",
      "visible": true,
      "locked": false
    }
  ],
  "markers": [],
  "bases": [
    "vault_maps/port_night_city.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/port_night_city.png",
  "measurement": {
    "displayUnit": "km",
    "scales": {},
    "customUnitPxPerUnit": {},
    "travelTimePresetIds": [],
    "travelDaysEnabled": false
  },
  "pinSizeOverrides": {},
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
    "h": 3867
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
      "id": "marker_atmvi7",
      "x": 0.060927915896841975,
      "y": 0.5448381354825508,
      "layer": "default",
      "link": "Floatsam",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_5nfnd6",
      "x": 0.438500560046738,
      "y": 0.6858210351762626,
      "layer": "default",
      "link": "Dock 14 Studio Apartment",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bmyujw",
      "x": 0.44510430558330166,
      "y": 0.7221656096357456,
      "layer": "default",
      "link": "Dock Cargo Community",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_shhp1m",
      "x": 0.44541383156375125,
      "y": 0.4603409875596796,
      "layer": "default",
      "link": "Rusty's Dive Shack",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ju0oi4",
      "x": 0.623442683112235,
      "y": 0.47037156111921447,
      "layer": "default",
      "link": "The Amber Room",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_v2rdv3",
      "x": 0.42132641484110345,
      "y": 0.6370680971288408,
      "layer": "default",
      "link": "Dock 13",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_dh530f",
      "x": 0.42299208431216684,
      "y": 0.5496276984403415,
      "layer": "default",
      "link": "Harbor Patrol HQ",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ib82dl",
      "x": 0.3206559751115583,
      "y": 0.23164891113812144,
      "layer": "default",
      "link": "Porto",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2kmdzq",
      "x": 0.5133684244003869,
      "y": 0.6497394828447134,
      "layer": "default",
      "link": "Maritime Supply",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mz42cn",
      "x": 0.3962074197237256,
      "y": 0.3309718593951486,
      "layer": "default",
      "link": "Medical Technologies",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wws0ws",
      "x": 0.4856504602878442,
      "y": 0.5681285791408348,
      "layer": "default",
      "link": "Mestnyy Bank",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_oicaqb",
      "x": 0.5379061402188865,
      "y": 0.4243281377867572,
      "layer": "default",
      "link": "Naiad's Embrace",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_6pub8v",
      "x": 0.3753429204133297,
      "y": 0.37197453179574674,
      "layer": "default",
      "link": "Reclaimed Studios",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4aaifh",
      "x": 0.4744394992253345,
      "y": 0.7583786730312618,
      "layer": "default",
      "link": "Reclamation Plant",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_s198g9",
      "x": 0.5668072979945489,
      "y": 0.5318468131866918,
      "layer": "default",
      "link": "The Yard",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/port_night_city.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/port_night_city.png",
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
