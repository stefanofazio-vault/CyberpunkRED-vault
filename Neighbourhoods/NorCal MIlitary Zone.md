#### NorCal Military Zone
```zoommap
image: vault_maps/norcal.png
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
    "h": 3734
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
      "id": "marker_9tdywz",
      "x": 0.7579634009249774,
      "y": 0.19500324446064263,
      "layer": "default",
      "link": "157th Tactical Air Squadron Airfield",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/norcal.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/norcal.png",
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
    "h": 3734
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
      "id": "marker_9tdywz",
      "x": 0.7409610640602143,
      "y": 0.1664713059099546,
      "layer": "default",
      "link": "157th Tactical Air Squadron Airfield",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_b3c9ds",
      "x": 0.34373190610397747,
      "y": 0.21036471400339352,
      "layer": "default",
      "link": "COG Treatment Facility",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_z8r0lo",
      "x": 0.481894125284903,
      "y": 0.12998321350496847,
      "layer": "default",
      "link": "Estero Bay Military COG Academy",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_yinhvp",
      "x": 0.5904040402191649,
      "y": 0.11136626655626373,
      "layer": "default",
      "link": "Fire & Emergency Response Center",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_z451n3",
      "x": 0.6906922589824568,
      "y": 0.5307302835943798,
      "layer": "default",
      "link": "Main Gate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_m15gny",
      "x": 0.5535882043307363,
      "y": 0.20513179911947924,
      "layer": "default",
      "link": "Mess Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3hpsj4",
      "x": 0.6590482339291077,
      "y": 0.4734528434361504,
      "layer": "default",
      "link": "Military Police Headquarters",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4o3jr3",
      "x": 0.7451344348825294,
      "y": 0.44735937721616975,
      "layer": "default",
      "link": "Militech Corporate Housing",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fxsflp",
      "x": 0.5833654666066729,
      "y": 0.4735177994172657,
      "layer": "default",
      "link": "Militech Offices",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_6tkvx8",
      "x": 0.8098551738287033,
      "y": 0.32913438858346644,
      "layer": "default",
      "link": "Motor Pool",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_smznmm",
      "x": 0.7158564800573622,
      "y": 0.3169046367029145,
      "layer": "default",
      "link": "The Oaks",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_pbajj9",
      "x": 0.6462789049587132,
      "y": 0.24080293414083506,
      "layer": "default",
      "link": "Parade Ground",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ciu3fc",
      "x": 0.6075964811816464,
      "y": 0.36392356254846064,
      "layer": "default",
      "link": "The Potentilla",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_k6eplm",
      "x": 0.594327494982934,
      "y": 0.2632261966613389,
      "layer": "default",
      "link": "Post Exchange",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_p3f70k",
      "x": 0.43604808242168386,
      "y": 0.25527624271713256,
      "layer": "default",
      "link": "Rec Center",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_627yyl",
      "x": 0.13599211182440293,
      "y": 0.41936592470275963,
      "layer": "default",
      "link": "Task Force 384 Docks",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tt4or7",
      "x": 0.5427506967618124,
      "y": 0.36636828248087594,
      "layer": "default",
      "link": "USO Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/norcal.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/norcal.png",
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
