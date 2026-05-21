#### Quartiere Universitario
```zoommap
image: vault_maps/university_district.png
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
    "h": 3280
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
      "id": "marker_jmb93g",
      "x": 0.4318964647225739,
      "y": 0.4644913627639155,
      "layer": "default",
      "link": "94.4 NCU Radio",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/university_district.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/university_district.png",
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
    "h": 3280
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
      "id": "marker_jmb93g",
      "x": 0.4371297877773689,
      "y": 0.4758642485736047,
      "layer": "default",
      "link": "94.4 NCU Radio",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2ye577",
      "x": 0.2256968963188441,
      "y": 0.5839956262808582,
      "layer": "default",
      "link": "Biograph Theater",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_75q0dw",
      "x": 0.7684833629478688,
      "y": 0.5246485578354566,
      "layer": "default",
      "link": "Biotechnica Campus",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_m89gh1",
      "x": 0.7160773501589859,
      "y": 0.46714984861028114,
      "layer": "default",
      "link": "Biotechnica Habitation Sphere Alpha",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_pxvo0j",
      "x": 0.2713300072326981,
      "y": 0.643191547073333,
      "layer": "default",
      "link": "Campus Chapel",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_m5q60d",
      "x": 0.22415757993457522,
      "y": 0.6435015720132862,
      "layer": "default",
      "link": "Carriage Street Books - Afterwords Cafè",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_xna0jx",
      "x": 0.19929282200383147,
      "y": 0.5469291291025754,
      "layer": "default",
      "link": "Fashion Cuts",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_sz91sa",
      "x": 0.2107589117464288,
      "y": 0.6134006922441949,
      "layer": "default",
      "link": "Food Truck Plaza",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_33mxnt",
      "x": 0.20222458164642307,
      "y": 0.5103294574422333,
      "layer": "default",
      "link": "Kosmos Hospital",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_sujtsl",
      "x": 0.42936220944113207,
      "y": 0.6079062768753005,
      "layer": "default",
      "link": "Night City Symphony Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_frmf4g",
      "x": 0.29656934876401403,
      "y": 0.6407174307340303,
      "layer": "default",
      "link": "Night City University",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_r8zcvm",
      "x": 0.3313420266350681,
      "y": 0.6421870619227564,
      "layer": "default",
      "link": "Administration Building",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3h84s5",
      "x": 0.31744376784840045,
      "y": 0.5384955599844488,
      "layer": "default",
      "link": "Blaine Building",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_pqh311",
      "x": 0.3178184389276277,
      "y": 0.5880188396094554,
      "layer": "default",
      "link": "Brooks Library",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wg1aq7",
      "x": 0.2732627606355572,
      "y": 0.5795852704913287,
      "layer": "default",
      "link": "The Cells",
      "iconKey": "pinRed",
      "tooltip": ""
    },
    {
      "type": "pin",
      "id": "marker_95w1a0",
      "x": 0.31765100478201924,
      "y": 0.5642087286902663,
      "layer": "default",
      "link": "Howard Wong Building",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_0me43b",
      "x": 0.31595085712271964,
      "y": 0.5068439037462723,
      "layer": "default",
      "link": "Michaels Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bofe7c",
      "x": 0.3484161105116875,
      "y": 0.5831446913769072,
      "layer": "default",
      "link": "Knute Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_kgtn9k",
      "x": 0.34972452875404125,
      "y": 0.5490190274276479,
      "layer": "default",
      "link": "Hoggagia Science Labs",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_i7bquh",
      "x": 0.2622962614914811,
      "y": 0.5131135987214893,
      "layer": "default",
      "link": "Lombardy Groceries",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_gopn8d",
      "x": 0.2907115155914037,
      "y": 0.5131135987214893,
      "layer": "default",
      "link": "NCU Clinic",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_r9u2hw",
      "x": 0.3484161979903425,
      "y": 0.5123382648010566,
      "layer": "default",
      "link": "Schumacher Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_6phwmn",
      "x": 0.3175147130375794,
      "y": 0.6131858256249842,
      "layer": "default",
      "link": "Science Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_5x446j",
      "x": 0.35090802747710087,
      "y": 0.6147152023347247,
      "layer": "default",
      "link": "M. Thompson Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tpntnb",
      "x": 0.8317307804042235,
      "y": 0.5873245966552719,
      "layer": "default",
      "link": "Parkside Living",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_67rle6",
      "x": 0.5388482195538284,
      "y": 0.5590773488326973,
      "layer": "default",
      "link": "PrincessLand!",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_f0f1eu",
      "x": 0.6044031489709244,
      "y": 0.6315084733813607,
      "layer": "default",
      "link": "Retail Resale",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_llpch1",
      "x": 0.16863548997708358,
      "y": 0.6250836573079472,
      "layer": "default",
      "link": "Stems & Seeds",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_7tnuxf",
      "x": 0.38923102656002406,
      "y": 0.5242573876151446,
      "layer": "default",
      "link": "Tumble And Dry",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_etbsvk",
      "x": 0.3884223738735015,
      "y": 0.6414117823164338,
      "layer": "default",
      "link": "University Crèche",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tp3kef",
      "x": 0.1682608188978564,
      "y": 0.5008103122072808,
      "layer": "default",
      "link": "University Cubes",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_urfwda",
      "x": 0.5388482195538284,
      "y": 0.6368477676520586,
      "layer": "default",
      "link": "Yewtree",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/university_district.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/university_district.png",
  "measurement": {
    "displayUnit": "km",
    "scales": {},
    "customUnitPxPerUnit": {},
    "travelTimePresetIds": [],
    "travelDaysEnabled": false
  },
  "pinSizeOverrides": {
    "pinRed": 120
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
      "id": "undo_na39eh",
      "label": "Delete pin",
      "createdAt": "2026-05-21T13:15:21.761Z",
      "payload": {
        "kind": "marker",
        "marker": {
          "type": "pin",
          "id": "marker_ql076o",
          "x": 0.38814401679339394,
          "y": 0.7226252811977261,
          "layer": "default",
          "link": "Night City University",
          "iconKey": "pinRed",
          "tooltip": "",
          "scaleLikeSticker": true
        },
        "index": 11
      }
    }
  ]
}
/ZOOMMAP-DATA
%%
