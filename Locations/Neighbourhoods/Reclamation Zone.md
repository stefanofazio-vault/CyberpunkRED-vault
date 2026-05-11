#### Reclamation Zone
```zoommap
image: vault_maps/reclamation_zone.png
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
      "id": "marker_se61f0",
      "x": 0.626534552025144,
      "y": 0.23578619027364248,
      "layer": "default",
      "link": "Booster Bistro",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2l72b6",
      "x": 0.5133356278170562,
      "y": 0.2917434661373411,
      "layer": "default",
      "link": "Country Cars",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_xnsk9l",
      "x": 0.5606212543849919,
      "y": 0.39760858263623045,
      "layer": "default",
      "link": "Earl's Second Hand Shop",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_x1lxu9",
      "x": 0.55775545883542,
      "y": 0.25090977834491235,
      "layer": "default",
      "link": "Flashback",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_dvaut9",
      "x": 0.5821147210067805,
      "y": 0.2705704428375632,
      "layer": "default",
      "link": "Foundry Tech School",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_785840",
      "x": 0.6551925075208626,
      "y": 0.5004489815208658,
      "layer": "default",
      "link": "Freddie Douglas School",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_gqqaly",
      "x": 0.5563225610606338,
      "y": 0.29779290136584907,
      "layer": "default",
      "link": "Gordon's Garage",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_vw184z",
      "x": 0.5821147210067806,
      "y": 0.5322085164705326,
      "layer": "default",
      "link": "McGee Speedway",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_yj045h",
      "x": 0.6236687564755723,
      "y": 0.43995462923578615,
      "layer": "default",
      "link": "Herschel's Crematorium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_prgge3",
      "x": 0.5606212543849918,
      "y": 0.21310080816673754,
      "layer": "default",
      "link": "La Perrera",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2scja2",
      "x": 0.47894608122219423,
      "y": 0.4081950942861194,
      "layer": "default",
      "link": "Metal Mountain",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bggvwt",
      "x": 0.6265345520251441,
      "y": 0.306867054208611,
      "layer": "default",
      "link": "Mobile Mosque Prayer Center",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_l18tvw",
      "x": 0.41876437468118544,
      "y": 0.5306961576634055,
      "layer": "default",
      "link": "NCART Yards",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_dohgfz",
      "x": 0.5348290944388452,
      "y": 0.459615293728437,
      "layer": "default",
      "link": "Reclamation Zone Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_l1fti6",
      "x": 0.5591883566102057,
      "y": 0.3295524363155159,
      "layer": "default",
      "link": "Second City Solos Firing Range",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/reclamation_zone.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/reclamation_zone.png",
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
