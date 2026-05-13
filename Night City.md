```zoommap
image: vault_maps/night_city.png
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
    "w": 5100,
    "h": 6600
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
      "id": "marker_ae1evj",
      "x": 0.44258295283950677,
      "y": 0.4586131693204507,
      "layer": "default",
      "link": "Zona calda",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ci5m03",
      "x": 0.7020332204625772,
      "y": 0.3975385275472456,
      "layer": "default",
      "link": "Executive Zone",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ml6lt5",
      "x": 0.6524913599076293,
      "y": 0.36744375303958227,
      "layer": "default",
      "link": "Charter Hill",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_7g6gs1",
      "x": 0.6275773238671748,
      "y": 0.2966325506831156,
      "layer": "default",
      "link": "New Westbrook",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_gdi0ul",
      "x": 0.3761454360054624,
      "y": 0.2136506729216312,
      "layer": "default",
      "link": "NorCal MIlitary Zone",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bwka2l",
      "x": 0.31343067904405525,
      "y": 0.4190031665084671,
      "layer": "default",
      "link": "Little Europe",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wpuw9n",
      "x": 0.5316436773994971,
      "y": 0.43316539347359545,
      "layer": "default",
      "link": "Upper Marina",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ebay0q",
      "x": 0.28107094847266173,
      "y": 0.44754891895225274,
      "layer": "default",
      "link": "Downtown",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4famcm",
      "x": 0.5617124048707172,
      "y": 0.4957890573106783,
      "layer": "default",
      "link": "Little China",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wey8ct",
      "x": 0.308848760236541,
      "y": 0.4940187704986841,
      "layer": "default",
      "link": "Quartiere universitario",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_n5j95z",
      "x": 0.3996276278806208,
      "y": 0.5438078971555748,
      "layer": "default",
      "link": "Glen",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_k3dp96",
      "x": 0.5233389987193454,
      "y": 0.5384970367195921,
      "layer": "default",
      "link": "Old Japantown",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_q9p1hu",
      "x": 0.31457613689772573,
      "y": 0.5466846090043885,
      "layer": "default",
      "link": "South Night City",
      "iconKey": "pinRed",
      "tooltip": ""
    },
    {
      "type": "pin",
      "id": "marker_h0znyt",
      "x": 0.2701889677735435,
      "y": 0.584082362070482,
      "layer": "default",
      "link": "Porto di Night City",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ejeglv",
      "x": 0.31600716047187116,
      "y": 0.611743689614964,
      "layer": "default",
      "link": "Reclamation Zone",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_q61yo4",
      "x": 0.4989977353021425,
      "y": 0.5778858085488717,
      "layer": "default",
      "link": "Old Combat Zone",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_7u0icm",
      "x": 0.4030641762272969,
      "y": 0.28180646194281295,
      "layer": "default",
      "link": "Watson",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_je5qr1",
      "x": 0.47064715091501164,
      "y": 0.30260723912885995,
      "layer": "default",
      "link": "Kabuki",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_cnwuxi",
      "x": 0.657359577633937,
      "y": 0.5349564968610163,
      "layer": "default",
      "link": "Heywood Docks",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ksbhcn",
      "x": 0.7272335554218252,
      "y": 0.5677066847039646,
      "layer": "default",
      "link": "Heywood",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ebvb0p",
      "x": 0.5920675186535631,
      "y": 0.5887287604035407,
      "layer": "default",
      "link": "Heywood Industrial Zone",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hc8x6t",
      "x": 0.6802691716715087,
      "y": 0.6938391410117593,
      "layer": "default",
      "link": "Santo Domingo",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fqfoy7",
      "x": 0.35638600400294135,
      "y": 0.6889708417270839,
      "layer": "default",
      "link": "Pacifica",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3zwpgx",
      "x": 0.42310990714861135,
      "y": 0.7845659919206438,
      "layer": "default",
      "link": "Rancho Coronado",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/night_city.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/night_city.png",
  "measurement": {
    "displayUnit": "km",
    "scales": {},
    "customUnitPxPerUnit": {},
    "travelTimePresetIds": [],
    "travelDaysEnabled": false
  },
  "pinSizeOverrides": {
    "pinRed": 248
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

