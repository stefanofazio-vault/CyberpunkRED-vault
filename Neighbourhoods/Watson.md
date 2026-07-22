#### Watson
```zoommap
image: vault_maps/watson.png
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
    "h": 3419
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
      "id": "marker_idmsmz",
      "x": 0.6663159107846434,
      "y": 0.6672094840655818,
      "layer": "default",
      "link": "Akagi-ryu Karate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_kk0sis",
      "x": 0.6936091738268845,
      "y": 0.24383035588690397,
      "layer": "default",
      "link": "Canadian Consulate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_oyf07l",
      "x": 0.6356627045087844,
      "y": 0.48906836925545605,
      "layer": "default",
      "link": "City Tot Daycare",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_sij3wm",
      "x": 0.5461295850092394,
      "y": 0.009430403817800073,
      "layer": "default",
      "link": "Ebunike Docks",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_24349m",
      "x": 0.47397748491958785,
      "y": 0.6031515085207588,
      "layer": "default",
      "link": "Faisal's Custom",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_lih8rl",
      "x": 0.36207459913992934,
      "y": 0.4381507009893562,
      "layer": "default",
      "link": "The Fork",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_mx5rcp",
      "x": 0.3162168056789417,
      "y": 0.5002039147038445,
      "layer": "default",
      "link": "Bodyweight Life Preservation Systems",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3sqm4b",
      "x": 0.29864554634263807,
      "y": 0.34299521212026485,
      "layer": "default",
      "link": "Cactus Water",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_sszd8d",
      "x": 0.27297548907249797,
      "y": 0.4000756474578391,
      "layer": "default",
      "link": "Gibson Battlegear",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ollxor",
      "x": 0.33142130539743736,
      "y": 0.38782794892233635,
      "layer": "default",
      "link": "Hammered Industries",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_v3yzjp",
      "x": 0.25141435181291844,
      "y": 0.3697150195630995,
      "layer": "default",
      "link": "Locations/Sedi corporative/Kendachi",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_usaz82",
      "x": 0.368555876632799,
      "y": 0.4786056277123938,
      "layer": "default",
      "link": "Locations/Sedi corporative/Kiroshi",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bbxob3",
      "x": 0.305002096417089,
      "y": 0.3982197318995743,
      "layer": "default",
      "link": "Makigai Automotive",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_yaxo2g",
      "x": 0.32698595991314683,
      "y": 0.4463890321605894,
      "layer": "default",
      "link": "Locations/Sedi corporative/Segotari",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_273cgi",
      "x": 0.2921243840651968,
      "y": 0.4475418744106323,
      "layer": "default",
      "link": "Locations/Sedi corporative/Towa",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_47uv4g",
      "x": 0.5130444564741125,
      "y": 0.7558336068520343,
      "layer": "default",
      "link": "FūdHouse",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_l1ikcg",
      "x": 0.47435219197464124,
      "y": 0.5301893270397983,
      "layer": "default",
      "link": "Gibson Battlegear Outlet",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_jg8ijn",
      "x": 0.5530450468674885,
      "y": 0.7097400269871786,
      "layer": "default",
      "link": "Hammered Up Liquor",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_twktnm",
      "x": 0.6391531479585882,
      "y": 0.14139994685922386,
      "layer": "default",
      "link": "HTown",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_03na5y",
      "x": 0.5980940363746762,
      "y": 0.7285189353089199,
      "layer": "default",
      "link": "Hunder Under Haven",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_699lto",
      "x": 0.7045741658520009,
      "y": 0.47726694904216355,
      "layer": "default",
      "link": "Petrochem & SovOil Joint Temporary Housing Solution",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_l0tlbv",
      "x": 0.6519259003510817,
      "y": 0.7672666885481627,
      "layer": "default",
      "link": "Megabuilding H10",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4d3pty",
      "x": 0.5992774599168966,
      "y": 0.5444416832080358,
      "layer": "default",
      "link": "Megabuilding H11",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zlp0b1",
      "x": 0.43871023882856197,
      "y": 0.6310612525593536,
      "layer": "default",
      "link": "Morgan's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ewwtot",
      "x": 0.4639461117333228,
      "y": 0.6925196021735619,
      "layer": "default",
      "link": "NCPD Precinct N°3",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_upj7kg",
      "x": 0.6716141146018242,
      "y": 0.6246788369463853,
      "layer": "default",
      "link": "NeoSoviet Consulate",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_y5em59",
      "x": 0.3649407057645765,
      "y": 0.5225459120676451,
      "layer": "default",
      "link": "The Obituary",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hwaudz",
      "x": 0.6141669048239305,
      "y": 0.04720794715097711,
      "layer": "default",
      "link": "Old Black Rum Pub",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ktfjij",
      "x": 0.5069377111030304,
      "y": 0.6390798830902924,
      "layer": "default",
      "link": "Oumei-ji Temple",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qpkakr",
      "x": 0.72015337262555,
      "y": 0.5239556014024997,
      "layer": "default",
      "link": "Petrochem Offices",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_eee1yt",
      "x": 0.7526141643355204,
      "y": 0.1387293623627848,
      "layer": "default",
      "link": "Petrochem Oil Refinery",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_txf82y",
      "x": 0.7215211758297808,
      "y": 0.10695904513319057,
      "layer": "default",
      "link": "SovOil Oil Refinery",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_s04hbr",
      "x": 0.6920513930961419,
      "y": 0.5373154009263167,
      "layer": "default",
      "link": "SovOil Offices",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_zt2zap",
      "x": 0.4815172836029935,
      "y": 0.7694910989199919,
      "layer": "default",
      "link": "The Pachinko Carnival",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ja1p7f",
      "x": 0.5729830658215997,
      "y": 0.8556643899490994,
      "layer": "default",
      "link": "Red Oktober",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4uroi7",
      "x": 0.6257564086074693,
      "y": 0.8860250699426394,
      "layer": "default",
      "link": "Redline",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_lpun30",
      "x": 0.6539178654472033,
      "y": 0.7138203008184723,
      "layer": "default",
      "link": "Sakura's",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_55bbx1",
      "x": 0.4454411460915349,
      "y": 0.5528287564537389,
      "layer": "default",
      "link": "SkidRow Limited",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ktu3ls",
      "x": 0.6881862425912849,
      "y": 0.41684989814684575,
      "layer": "default",
      "link": "Smash-Cut",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_5b54dh",
      "x": 0.6283727105287477,
      "y": 0.8323590336714546,
      "layer": "default",
      "link": "Snack & Shack",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_jz5sfl",
      "x": 0.6429528734220867,
      "y": 0.5646302808646317,
      "layer": "default",
      "link": "Trauma Team Tower",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_y6bbf1",
      "x": 0.6073763453173661,
      "y": 0.6249763210953253,
      "layer": "default",
      "link": "Trauma Team Corporate Living Center",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_j9ras8",
      "x": 0.5457550528874517,
      "y": 0.7913868700603826,
      "layer": "default",
      "link": "Turbo Neon Motors",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qzke61",
      "x": 0.6421443318681854,
      "y": 0.524919012415144,
      "layer": "default",
      "link": "UnoMas Mexican Bar & Grill",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_w9xdp2",
      "x": 0.4071830659574431,
      "y": 0.5506754088453343,
      "layer": "default",
      "link": "Vargtimmen",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_9gi5l5",
      "x": 0.6080601594528485,
      "y": 0.5848187743236274,
      "layer": "default",
      "link": "Watson Central Cubelife",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ajbw9d",
      "x": 0.7121139645354067,
      "y": 0.3721659034192443,
      "layer": "default",
      "link": "Whammer Arena",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_j246fg",
      "x": 0.6695388423774982,
      "y": 0.5799487898374174,
      "layer": "default",
      "link": "Watson Residence",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    }
  ],
  "bases": [
    "vault_maps/watson.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/watson.png",
  "measurement": {
    "displayUnit": "km",
    "scales": {},
    "customUnitPxPerUnit": {},
    "travelTimePresetIds": [],
    "travelDaysEnabled": false
  },
  "pinSizeOverrides": {
    "pinRed": 130
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
    "h": 3419
  },
  "layers": [
    {
      "id": "default",
      "name": "Default",
      "visible": true,
      "locked": false
    }
  ],
  "markers": [],
  "bases": [
    "vault_maps/watson.png"
  ],
  "overlays": [],
  "activeBase": "vault_maps/watson.png",
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
