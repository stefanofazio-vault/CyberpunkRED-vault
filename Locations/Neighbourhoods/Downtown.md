```zoommap
image: vault_maps/downtown.png
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
    "h": 3445
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
      "id": "marker_0yfnsv",
      "x": 0.5758393546847993,
      "y": 0.47906920542357695,
      "layer": "default",
      "link": "Acacia Way",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_66jvdq",
      "x": 0.3511035335155764,
      "y": 0.3388112588475824,
      "layer": "default",
      "link": "Bella Vista Market",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_rdo4yz",
      "x": 0.6276780198762765,
      "y": 0.3984056022271084,
      "layer": "default",
      "link": "Cafè Bouchon",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_labgbm",
      "x": 0.5046873366469866,
      "y": 0.5628964653308993,
      "layer": "default",
      "link": "Clocktower Residence",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_w0cf1h",
      "x": 0.594593455415763,
      "y": 0.29041574421137223,
      "layer": "default",
      "link": "Continental Brands Offices",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_50ibf5",
      "x": 0.6350929647203111,
      "y": 0.29026817894010903,
      "layer": "default",
      "link": "Continental Plaza",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_gd9qpu",
      "x": 0.4739694039878071,
      "y": 0.47619395764163186,
      "layer": "default",
      "link": "Cortex Complex",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_suafsc",
      "x": 0.5074286691149225,
      "y": 0.6560807801456355,
      "layer": "default",
      "link": "Delirium",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_e80int",
      "x": 0.4257460229591039,
      "y": 0.5698914935084207,
      "layer": "default",
      "link": "The Eldritch Mirage",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_i85xz6",
      "x": 0.40281738594999444,
      "y": 0.42750320905345507,
      "layer": "default",
      "link": "Europa Meatworks",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_gf1lzo",
      "x": 0.27671084451645,
      "y": 0.5628964136261791,
      "layer": "default",
      "link": "Folio",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zttgfm",
      "x": 0.6117899769051659,
      "y": 0.6294154150591238,
      "layer": "default",
      "link": "Gilded Phoenix Arcade",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_56nzmt",
      "x": 0.3392647767398444,
      "y": 0.5413844062907273,
      "layer": "default",
      "link": "Goosetopia",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_iplk18",
      "x": 0.47720998748397925,
      "y": 0.3739478735761683,
      "layer": "default",
      "link": "Guns & Dolls",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zla2r0",
      "x": 0.29066652011425614,
      "y": 0.3093478928310061,
      "layer": "default",
      "link": "Jade Blossom Spa",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_uq79e2",
      "x": 0.38655464231228204,
      "y": 0.5368920416818636,
      "layer": "default",
      "link": "Moleharty's Books and Antiques",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mngbms",
      "x": 0.45864026327150204,
      "y": 0.4304489303689432,
      "layer": "default",
      "link": "Munch Munch Munch",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_k55hol",
      "x": 0.46238027272619336,
      "y": 0.2901205102594057,
      "layer": "default",
      "link": "New Libertine Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ar5e1g",
      "x": 0.4239382934125754,
      "y": 0.47663680856958157,
      "layer": "default",
      "link": "Locations/Servizi pubblici/Night City Firestation #2",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_0mrlta",
      "x": 0.5484869057439924,
      "y": 0.35450245219976184,
      "layer": "default",
      "link": "The Nightingale Theater",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_9pwipa",
      "x": 0.6114152762385641,
      "y": 0.6804613136494154,
      "layer": "default",
      "link": "Studio Blocks A thru D",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_48mc2b",
      "x": 0.34967050463564964,
      "y": 0.43317650947018477,
      "layer": "default",
      "link": "West Hill Church Of God",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_x5iksc",
      "x": 0.35116878251120776,
      "y": 0.3849990853435008,
      "layer": "default",
      "link": "West Hill Park",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/downtown.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/downtown.png",
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
