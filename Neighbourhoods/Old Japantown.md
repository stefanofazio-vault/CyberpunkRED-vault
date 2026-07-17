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
      "y": 0.4975339231638497,
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
    },
    {
      "type": "pin",
      "id": "marker_7jdxue",
      "x": 0.37307219819599363,
      "y": 0.3341680803511323,
      "layer": "default",
      "link": "Kaifū Corner",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4jyenm",
      "x": 0.5135566378624966,
      "y": 0.32727468562350215,
      "layer": "default",
      "link": "Kid Camp",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_0h1vfz",
      "x": 0.27415968455325185,
      "y": 0.5271831327247759,
      "layer": "default",
      "link": "Kakoi-chō",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tjcpzs",
      "x": 0.6640756803623211,
      "y": 0.4772060209494574,
      "layer": "default",
      "link": "Lovely Drone Heroes Cafè",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_x4ih0i",
      "x": 0.4934874321958533,
      "y": 0.43239895521986166,
      "layer": "default",
      "link": "Miyasaka Clinic",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hebzn7",
      "x": 0.5164236672434457,
      "y": 0.397931981581711,
      "layer": "default",
      "link": "Mrs. Suzuki's Bodega",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_q1p2el",
      "x": 0.21108503817237295,
      "y": 0.5444166195438512,
      "layer": "default",
      "link": "Neo Galaxy Cards and Comics",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_klej4p",
      "x": 0.3874073451007389,
      "y": 0.47203597490373483,
      "layer": "default",
      "link": "Oni-Yama Jail",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_1xsfyi",
      "x": 0.3802397716483663,
      "y": 0.22904381075477284,
      "layer": "default",
      "link": "The Precipice",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_dlcykc",
      "x": 0.6956130035527606,
      "y": 0.5220130866790533,
      "layer": "default",
      "link": "Sanroo Complex",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fvsa4m",
      "x": 0.6053015780528658,
      "y": 0.7322616258717721,
      "layer": "default",
      "link": "Segotari Factory",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_jgnomw",
      "x": 0.6096021221242894,
      "y": 0.4427390473113068,
      "layer": "default",
      "link": "Segotari Station Japantown",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_76vi4g",
      "x": 0.38310680102931527,
      "y": 0.5582034089991115,
      "layer": "default",
      "link": "Tartarus",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_pd9a1b",
      "x": 0.51785718193392,
      "y": 0.6305840536392276,
      "layer": "default",
      "link": "Tsukuyomi",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3k5162",
      "x": 0.5565620785767322,
      "y": 0.5375232248162211,
      "layer": "default",
      "link": "Unnamed Cube Hotel",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_slpg7n",
      "x": 0.31429809588653834,
      "y": 0.21181032393569757,
      "layer": "default",
      "link": "White Side",
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
