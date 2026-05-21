#### Little China
```zoommap
image: vault_maps/little_china.png
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
    "h": 3859
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
      "id": "marker_2ewn5z",
      "x": 0.7179081093890114,
      "y": 0.29572607594689065,
      "layer": "default",
      "link": "Bridgetown",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_vn8bhu",
      "x": 0.33199074092676456,
      "y": 0.49623245438085956,
      "layer": "default",
      "link": "Chrome Cross",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_8wlx8w",
      "x": 0.4269305013990648,
      "y": 0.6400568587925749,
      "layer": "default",
      "link": "Rovine del Forlorn Hope",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_5kcnaz",
      "x": 0.5138663259545004,
      "y": 0.2558870380465352,
      "layer": "default",
      "link": "Guăngbō Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_q0qocg",
      "x": 0.627722095780684,
      "y": 0.33023863952335775,
      "layer": "default",
      "link": "Guānyīn Temple",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fndp4y",
      "x": 0.3585256159137253,
      "y": 0.3437149171827489,
      "layer": "default",
      "link": "The Hong Kong Market",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_auuwxx",
      "x": 0.5445087921748288,
      "y": 0.47131289713230023,
      "layer": "default",
      "link": "Hydrosubsidium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tp9d4z",
      "x": 0.33342330031131673,
      "y": 0.38223649075343263,
      "layer": "default",
      "link": "Ling Husan's New China Pharmacy",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3qfub0",
      "x": 0.40380879707466383,
      "y": 0.40721898654730126,
      "layer": "default",
      "link": "Rovine della Ling Po Import",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wez9lj",
      "x": 0.39047613196272185,
      "y": 0.3036124510161391,
      "layer": "default",
      "link": "Madam Yap's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qeh3fq",
      "x": 0.45475681328237777,
      "y": 0.3470023948947058,
      "layer": "default",
      "link": "Madame Lin's Massage Parlor",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_91enx3",
      "x": 0.32663490642106624,
      "y": 0.5762997432531864,
      "layer": "default",
      "link": "The Parisian",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_14wnrp",
      "x": 0.3024063436219921,
      "y": 0.33299916841754873,
      "layer": "default",
      "link": "Prosperity Gardens Tenements",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_d0ndr2",
      "x": 0.6211834204940884,
      "y": 0.45724677825246235,
      "layer": "default",
      "link": "Richard Night Aquarium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qlk6ye",
      "x": 0.2398076779810855,
      "y": 0.41872515853915027,
      "layer": "default",
      "link": "La perdita",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/little_china.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/little_china.png",
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
ZOOMMAP-DATA id=map-0
{
  "size": {
    "w": 4073,
    "h": 3859
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
      "id": "marker_2ewn5z",
      "x": 0.7179081093890114,
      "y": 0.29572607594689065,
      "layer": "default",
      "link": "Bridgetown",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_vn8bhu",
      "x": 0.33199074092676456,
      "y": 0.49623245438085956,
      "layer": "default",
      "link": "Chrome Cross",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_8wlx8w",
      "x": 0.42693041399397264,
      "y": 0.6400568587925749,
      "layer": "default",
      "link": "Rovine del Forlorn Hope",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_5kcnaz",
      "x": 0.5138663259545004,
      "y": 0.2558870380465352,
      "layer": "default",
      "link": "Guăngbō Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_q0qocg",
      "x": 0.627722095780684,
      "y": 0.33023863952335775,
      "layer": "default",
      "link": "Guānyīn Temple",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fndp4y",
      "x": 0.3585256159137253,
      "y": 0.3437149171827489,
      "layer": "default",
      "link": "The Hong Kong Market",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_auuwxx",
      "x": 0.5445087921748288,
      "y": 0.47131289713230023,
      "layer": "default",
      "link": "Locations/Sedi corporative/Hydrosubsidium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tp9d4z",
      "x": 0.33342330031131673,
      "y": 0.38223649075343263,
      "layer": "default",
      "link": "Ling Husan's New China Pharmacy",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3qfub0",
      "x": 0.40380879707466383,
      "y": 0.40721898654730126,
      "layer": "default",
      "link": "Rovine della Ling Po Import",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wez9lj",
      "x": 0.38933051341902464,
      "y": 0.3024033024469556,
      "layer": "default",
      "link": "Madam Yap's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qeh3fq",
      "x": 0.45475681328237777,
      "y": 0.3470023948947058,
      "layer": "default",
      "link": "Madame Lin's Massage Parlor",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_91enx3",
      "x": 0.32663490642106624,
      "y": 0.5762997432531864,
      "layer": "default",
      "link": "The Parisian",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_14wnrp",
      "x": 0.3024063436219921,
      "y": 0.33299916841754873,
      "layer": "default",
      "link": "Prosperity Gardens Tenements",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_d0ndr2",
      "x": 0.6211834204940884,
      "y": 0.45724677825246235,
      "layer": "default",
      "link": "Richard Night Aquarium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qlk6ye",
      "x": 0.2398076779810855,
      "y": 0.41872515853915027,
      "layer": "default",
      "link": "La perdita",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/little_china.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/little_china.png",
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
