#### Kabuki
```zoommap
image: vault_maps/kabuki.png
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
    "h": 3418
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
      "id": "marker_8tdqyi",
      "x": 0.3730606478999825,
      "y": 0.8846718445565431,
      "layer": "default",
      "link": "100.0 G3 Gun-Gal Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_s6vmnh",
      "x": 0.5923816051668311,
      "y": 0.1450342968478928,
      "layer": "default",
      "link": "91.9 Royal Blue",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_lrfxec",
      "x": 0.3472581823391769,
      "y": 0.833426748872341,
      "layer": "default",
      "link": "Animelocaris",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_6twfmz",
      "x": 0.6038493676383004,
      "y": 0.3670963781461019,
      "layer": "default",
      "link": "Cyborg Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_nrvxwt",
      "x": 0.4017300540786556,
      "y": 0.3995516054127632,
      "layer": "default",
      "link": "Delphi X",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_j7c00x",
      "x": 0.5006395053950775,
      "y": 0.4542130408092455,
      "layer": "default",
      "link": "Hiroto Miyamoto Memorial Clinic",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_8riy39",
      "x": 0.4146312868590584,
      "y": 0.2663143566338378,
      "layer": "default",
      "link": "Houou",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hb9rru",
      "x": 0.5923816051668311,
      "y": 0.2014039021005151,
      "layer": "default",
      "link": "Kabuki Ceremonial Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_jk1he6",
      "x": 0.48200439137894,
      "y": 0.16211599540929353,
      "layer": "default",
      "link": "Kabuki Market",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_8osfuq",
      "x": 0.6024158973293667,
      "y": 0.43200683267942463,
      "layer": "default",
      "link": "Matsura Food Products",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_op43o9",
      "x": 0.4920386835414757,
      "y": 0.3705127178583821,
      "layer": "default",
      "link": "Murakami Suiun Imports",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_md6hpb",
      "x": 0.4045969946965229,
      "y": 0.48666826807590685,
      "layer": "default",
      "link": "Nakagawa Academy",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_78q0k5",
      "x": 0.3572924745017124,
      "y": 0.7070221795179757,
      "layer": "default",
      "link": "Nakagawa Garage Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_t16ooq",
      "x": 0.39742964315185464,
      "y": 0.6421117249846532,
      "layer": "default",
      "link": "Nakagawa Kabuki Theater",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mkk90x",
      "x": 0.36445982604638066,
      "y": 0.5754931005951904,
      "layer": "default",
      "link": "No-Tell Motel",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_amiib4",
      "x": 0.4891717429236083,
      "y": 0.2526489977847172,
      "layer": "default",
      "link": "Oasis",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_87dnip",
      "x": 0.5508109662077552,
      "y": 0.37222088771452216,
      "layer": "default",
      "link": "Rokumei-Kan",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_5m9vt3",
      "x": 0.5522444365166889,
      "y": 0.18944671310753464,
      "layer": "default",
      "link": "Sanroo Neuro-Land",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_pkqn03",
      "x": 0.42609904933052767,
      "y": 0.1791976939706942,
      "layer": "default",
      "link": "Segotari HQ - EXCEL-1",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mo419n",
      "x": 0.5938150754757647,
      "y": 0.2628980169215577,
      "layer": "default",
      "link": "Toranoko Gakuen",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hbcsgm",
      "x": 0.5995489567114994,
      "y": 0.3107267728934796,
      "layer": "default",
      "link": "Tyger Dojo - Tora-no-Ana",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_c02ys5",
      "x": 0.43469987118412956,
      "y": 0.5772012704513305,
      "layer": "default",
      "link": "Tyger Works Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2dm3tw",
      "x": 0.40746393531439024,
      "y": 0.34659833987242106,
      "layer": "default",
      "link": "Yum Seng",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_j0xgh2",
      "x": 0.49060521323254197,
      "y": 0.6728587823951744,
      "layer": "default",
      "link": "Tengen Towers",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/kabuki.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/kabuki.png",
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
