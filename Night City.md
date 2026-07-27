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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_4famcm",
      "x": 0.5617124048707172,
      "y": 0.49313361020998076,
      "layer": "default",
      "link": "Little China",
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_n5j95z",
      "x": 0.40093512288856187,
      "y": 0.5448183017611273,
      "layer": "default",
      "link": "Glen",
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": ""
    },
    {
      "type": "pin",
      "id": "marker_h0znyt",
      "x": 0.2701889677735435,
      "y": 0.584082362070482,
      "layer": "default",
      "link": "Porto di Night City",
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": "",
      "scaleLikeSticker": true,
      "tooltipLabelAlways": true,
      "tooltipLabelPosition": "below"
    },
    {
      "type": "pin",
      "id": "marker_je5qr1",
      "x": 0.47064715091501164,
      "y": 0.30260723912885995,
      "layer": "default",
      "link": "Kabuki",
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ksbhcn",
      "x": 0.7272335554218252,
      "y": 0.5677066847039646,
      "layer": "default",
      "link": "North Heywood",
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hc8x6t",
      "x": 0.6815766666794496,
      "y": 0.6938391410117593,
      "layer": "default",
      "link": "Santo Domingo",
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
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
      "iconKey": "pinBlue",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_jnbcdg",
      "x": 0.1528677245181202,
      "y": 0.3372411920923575,
      "layer": "default",
      "link": "107.3 Morro Rock Radio",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qp0tk0",
      "x": 0.8731540542829506,
      "y": 0.588239190422566,
      "layer": "default",
      "link": "Edgewood Farm",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_obk5wo",
      "x": 0.9447531017149599,
      "y": 0.6356356351793029,
      "layer": "default",
      "link": "Ingall Farm",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_c9pags",
      "x": 0.7776887159743925,
      "y": 0.8134181945962344,
      "layer": "default",
      "link": "Poppy Farm",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_hqma82",
      "x": 0.5235120975907602,
      "y": 0.9509968940957428,
      "layer": "default",
      "link": "Jackson Plains Regional Airport",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_qsrqmp",
      "x": 0.8726766690326165,
      "y": 0.7444445356197673,
      "layer": "default",
      "link": "Laguna Bend",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_fg4l9f",
      "x": 0.8089536916204905,
      "y": 0.607419101486779,
      "layer": "default",
      "link": "Municipal Landfill",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_ubboel",
      "x": 0.1788819868176295,
      "y": 0.3857441338134964,
      "layer": "default",
      "link": "Night City Spaceport",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3kdipl",
      "x": 0.947617238414602,
      "y": 0.5177901121105276,
      "layer": "default",
      "link": "NorCal Marshal Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_nohddp",
      "x": 0.5781660662642543,
      "y": 0.11187774361742349,
      "layer": "default",
      "link": "Militech Ballistics and Explosive Range",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_vl3owx",
      "x": 0.5984524921703838,
      "y": 0.8929040306111354,
      "layer": "default",
      "link": "Night Corp Solar Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_b4lv8v",
      "x": 0.35048100802928434,
      "y": 0.05378489701713515,
      "layer": "default",
      "link": "Northern Oil Fields",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_6266ui",
      "x": 0.8325813772730535,
      "y": 0.5705346986939236,
      "layer": "default",
      "link": "Petrochem CHOOH2 Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_j34d6x",
      "x": 0.9531063821828148,
      "y": 0.7213917669899136,
      "layer": "default",
      "link": "Pol-Bud Cement Factory",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_3g2w40",
      "x": 0.8929631823399271,
      "y": 0.4908645534523098,
      "layer": "default",
      "link": "Pol-Bud Miasto",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_86bioa",
      "x": 0.8349679539199999,
      "y": 0.46246357545852074,
      "layer": "default",
      "link": "Pol-Bud Mine",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_bxpsh7",
      "x": 0.828285259624771,
      "y": 0.8901377037785351,
      "layer": "default",
      "link": "Sheriff's Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_1t7c0z",
      "x": 0.4471398094636775,
      "y": 0.870957860251598,
      "layer": "default",
      "link": "SovOil CHOOH2 Station",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_i4ansd",
      "x": 0.9476172384146021,
      "y": 0.5683217047651197,
      "layer": "default",
      "link": "Sunshine Motel",
      "iconKey": "pinRed",
      "tooltip": "",
      "scaleLikeSticker": true
    },
    {
      "type": "pin",
      "id": "marker_msuwss",
      "x": 0.8392638967659203,
      "y": 0.5342036288048644,
      "layer": "default",
      "link": "Union Railroad Station",
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
    "pinBlue": 248,
    "pinRed": 220
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

