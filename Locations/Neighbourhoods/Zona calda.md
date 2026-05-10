```zoommap
image: vault_maps/zona_calda.png
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
    "h": 4004
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
      "id": "marker_kkwn44",
      "x": 0.6949838383674327,
      "y": 0.4610441157742031,
      "layer": "default",
      "link": "Ashcroft Hotel",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2cvet3",
      "x": 0.3652781561196939,
      "y": 0.5304166616270458,
      "layer": "default",
      "link": "Il cratere",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_shm5bp",
      "x": 0.7090583253974586,
      "y": 0.3506851779650224,
      "layer": "default",
      "link": "Crisis Center",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_jx56uu",
      "x": 0.2823226658473394,
      "y": 0.470101203888358,
      "layer": "default",
      "link": "Dark Zone One",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_8ovu3e",
      "x": 0.5616441080279372,
      "y": 0.6923426161964641,
      "layer": "default",
      "link": "La discarica",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_81z0zp",
      "x": 0.5975794075296107,
      "y": 0.2639543990198708,
      "layer": "default",
      "link": "Eurasiabank Plaza",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_i2usgz",
      "x": 0.33519728858015085,
      "y": 0.641090116248046,
      "layer": "default",
      "link": "The N54",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_prbb33",
      "x": 0.35394357087514977,
      "y": 0.12407250223937037,
      "layer": "default",
      "link": "Totentanz",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_9ndujk",
      "x": 0.11734497773570172,
      "y": 0.271239867693943,
      "layer": "default",
      "link": "Toggle's Temple",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_b64k16",
      "x": 0.7550205516030253,
      "y": 0.5210997958775664,
      "layer": "default",
      "link": "Safe Child",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_k06fdo",
      "x": 0.759317805904694,
      "y": 0.3539139000333682,
      "layer": "default",
      "link": "Graceland Medical",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/zona_calda.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/zona_calda.png",
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
