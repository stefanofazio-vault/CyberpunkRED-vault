#### Executive Zone
```zoommap
image: vault_maps/executive_zone.png
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
    "h": 3425
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
      "id": "marker_25vh0b",
      "x": 0.590661232085808,
      "y": 0.3984136740095877,
      "layer": "default",
      "link": "The Estates - Artyom Sokolov",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_maw6yt",
      "x": 0.5348971372122013,
      "y": 0.48673431262986305,
      "layer": "default",
      "link": "The Estates - Denny",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hbcaa9",
      "x": 0.4503694172395816,
      "y": 0.48474668545043176,
      "layer": "default",
      "link": "The Estates - Eran Malour",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ei4pd2",
      "x": 0.45495530044522214,
      "y": 0.3630712204815157,
      "layer": "default",
      "link": "The Estates - Kerry Eurodyne",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zz8ph7",
      "x": 0.439566220472558,
      "y": 0.6974594590209088,
      "layer": "default",
      "link": "The Estates - Franklin M'bolu",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_d9ggzv",
      "x": 0.4963295358256846,
      "y": 0.4433873144680203,
      "layer": "default",
      "link": "The Estates - Heather Stein",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_z5f3zz",
      "x": 0.5013125182064845,
      "y": 0.6804176024570896,
      "layer": "default",
      "link": "The Estates - Jami Sharkeater Tealov",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_7g8if5",
      "x": 0.5553344497825526,
      "y": 0.6821217881134715,
      "layer": "default",
      "link": "The Estates - William Joseph Billy Joe Brentwood",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3a3fda",
      "x": 0.4973878838475853,
      "y": 0.4892518454383492,
      "layer": "default",
      "link": "The Estates - Karen Davies",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wpdeyn",
      "x": 0.5686661361873534,
      "y": 0.7765944599820095,
      "layer": "default",
      "link": "The Estates - Michiko Sanderson",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_t2247j",
      "x": 0.40791409247476446,
      "y": 0.4441297232279339,
      "layer": "default",
      "link": "The Estates - Mister Kernaghan",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hwyt0e",
      "x": 0.38224399240373336,
      "y": 0.6535960252033082,
      "layer": "default",
      "link": "The Estates - UR",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/executive_zone.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/executive_zone.png",
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
