#### Rancho Coronado
```zoommap
image: vault_maps/rancho_coronado.png
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
    "w": 652,
    "h": 614
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
      "id": "marker_x15qge",
      "x": 0.5933947462461983,
      "y": 0.4757565994262802,
      "layer": "default",
      "link": "106.9 Sangre y Arena",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zvt679",
      "x": 0.13079261966733005,
      "y": 0.5108780216275389,
      "layer": "default",
      "link": "Albino Alligators Car Wash",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_i689oi",
      "x": 0.33565312630240035,
      "y": 0.40895398495737956,
      "layer": "default",
      "link": "Bread and Roses",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_d5jhsi",
      "x": 0.13845485105231703,
      "y": 0.27825871988702017,
      "layer": "default",
      "link": "Coronado Heights",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_y8dfsh",
      "x": 0.8234178528677414,
      "y": 0.4180815064718737,
      "layer": "default",
      "link": "The Culms",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_41ztmd",
      "x": 0.2438425787878609,
      "y": 0.28493713826239675,
      "layer": "default",
      "link": "Digital Divinity Ruins",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_830tmy",
      "x": 0.4672020011249142,
      "y": 0.07831173720864266,
      "layer": "default",
      "link": "Eagle Rock Stadium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_x35g88",
      "x": 0.22471961486729244,
      "y": 0.4212565105224529,
      "layer": "default",
      "link": "The Henhouse",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_g1kk0t",
      "x": 0.526312666813231,
      "y": 0.3640423247213457,
      "layer": "default",
      "link": "The Island",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_o1cbl2",
      "x": 0.6835233277340161,
      "y": 0.18314573774624385,
      "layer": "default",
      "link": "Jack 'N' the Green",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_7gls2m",
      "x": 0.2622165449446066,
      "y": 0.17156911309263223,
      "layer": "default",
      "link": "Minimallism",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/rancho_coronado.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/rancho_coronado.png",
  "measurement": {
    "displayUnit": "km",
    "scales": {},
    "customUnitPxPerUnit": {},
    "travelTimePresetIds": [],
    "travelDaysEnabled": false
  },
  "pinSizeOverrides": {
    "pinRed": 28
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
