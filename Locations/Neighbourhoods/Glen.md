#### Glen
```zoommap
image: vault_maps/glen.png
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
    "h": 3375
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
      "id": "marker_bizkl8",
      "x": 0.39979191334143743,
      "y": 0.6285056633884061,
      "layer": "default",
      "link": "1st Night City Bank",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_rbiroc",
      "x": 0.7306074211327493,
      "y": 0.37121308960756744,
      "layer": "default",
      "link": "96.1 Fever Dream",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fw4rke",
      "x": 0.6096021247406658,
      "y": 0.3286718275637543,
      "layer": "default",
      "link": "Air",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_858npz",
      "x": 0.42468449738055486,
      "y": 0.21954911607287667,
      "layer": "default",
      "link": "Archer & Li",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_glauzj",
      "x": 0.3329383106046712,
      "y": 0.26452938314321245,
      "layer": "default",
      "link": "Bear's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_86qqm9",
      "x": 0.4863264666206015,
      "y": 0.37179002000324374,
      "layer": "default",
      "link": "Beth El Congregation",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zka5lr",
      "x": 0.466256988263377,
      "y": 0.7420122181975456,
      "layer": "default",
      "link": "City Hall",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ei7m34",
      "x": 0.6855877160244737,
      "y": 0.2714494242309564,
      "layer": "default",
      "link": "Club Atlantis",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_la19n2",
      "x": 0.5881073925750975,
      "y": 0.42023030761745145,
      "layer": "default",
      "link": "Consulate Causeway",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_wakqij",
      "x": 0.5680379142178729,
      "y": 0.4704006055035952,
      "layer": "default",
      "link": "EEC Consulate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zxw2a9",
      "x": 0.6139110076058147,
      "y": 0.4409904308806833,
      "layer": "default",
      "link": "Japanese Consulate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_le6sac",
      "x": 0.5666043800494996,
      "y": 0.42542033843325944,
      "layer": "default",
      "link": "Mexican Consulate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_h25mzr",
      "x": 0.6282463492895466,
      "y": 0.4098502459858356,
      "layer": "default",
      "link": "Pacifica Confederation Offices",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_9wj2uy",
      "x": 0.5709049825546193,
      "y": 0.3752500405471157,
      "layer": "default",
      "link": "Organization Of American States Mission",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_cdsmfk",
      "x": 0.6139110076058147,
      "y": 0.3821700816348597,
      "layer": "default",
      "link": "United States Consulate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_d54x7n",
      "x": 0.529332491671797,
      "y": 0.4669405849597233,
      "layer": "default",
      "link": "Diplomatic Immunity",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bkgfw4",
      "x": 0.3960138140130912,
      "y": 0.7229821052062497,
      "layer": "default",
      "link": "DMV",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_rpxxrq",
      "x": 0.6110439392690683,
      "y": 0.5569011191003947,
      "layer": "default",
      "link": "EuroBank",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_0eo557",
      "x": 0.2741634097013708,
      "y": 0.2973995783099962,
      "layer": "default",
      "link": "First Baptist Church Of Night City",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_pxqtnw",
      "x": 0.26699573885950495,
      "y": 0.5430610369249067,
      "layer": "default",
      "link": "Glenlife Perfected",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_16r5o8",
      "x": 0.5838067900699779,
      "y": 0.7177920743904417,
      "layer": "default",
      "link": "Hall Of Justice",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_aohml7",
      "x": 0.3573083914670153,
      "y": 0.5361409958371627,
      "layer": "default",
      "link": "Kasim's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fi53ge",
      "x": 0.29566642222696854,
      "y": 0.4669405849597232,
      "layer": "default",
      "link": "Lazarus Regional HQ",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_lx4sri",
      "x": 0.6139110076058146,
      "y": 0.4755906363194032,
      "layer": "default",
      "link": "Le Jardin",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mofz29",
      "x": 0.5336330941769165,
      "y": 0.6036113964426664,
      "layer": "default",
      "link": "Merrill, Asukaga & Finch Offices",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_tygcse",
      "x": 0.2540939313441463,
      "y": 0.40466021517002754,
      "layer": "default",
      "link": "The Molly May",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3wrklo",
      "x": 0.7285937410756691,
      "y": 0.5032708006703789,
      "layer": "default",
      "link": "NCPD Precinct N°1",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_cl10h0",
      "x": 0.28419814887998307,
      "y": 0.1832189003622209,
      "layer": "default",
      "link": "Night City News Today",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_xhfx28",
      "x": 0.3329383106046713,
      "y": 0.39082013299453966,
      "layer": "default",
      "link": "Night City Plaza",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_2w6ycn",
      "x": 0.4218174290438085,
      "y": 0.2749094447748283,
      "layer": "default",
      "link": "Raven Microcybernetics HQ",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zukxci",
      "x": 0.6110439392690683,
      "y": 0.2212791263448127,
      "layer": "default",
      "link": "Seafoam",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_1qpuxy",
      "x": 0.702790126044952,
      "y": 0.323349732389036,
      "layer": "default",
      "link": "Souls Respite",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_q4ybsk",
      "x": 0.48345939828385526,
      "y": 0.508460831486187,
      "layer": "default",
      "link": "World Stock Exchange",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_47pqv5",
      "x": 0.6139110076058147,
      "y": 0.515380872573931,
      "layer": "default",
      "link": "Worthy Housing",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/glen.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/glen.png",
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
