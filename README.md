# SMART-ROAD-SIGN
<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Template</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
/* Always set the map height explicitly to define the size of the div
 * element that contains the map. */
#map {
  height: 100%;
  width: 100%;
}
/* Optional: Makes the sample page fill the window. */
html, body {
  height: 100%;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
}
/* Style the header */
header {
  background-color: #666;
  text-align: center;
  font-size: 35px;
  color: white;
  width: 100%;
  height: 5%;
}
/* Responsive layout - makes the two columns/boxes stack on top of each other instead of next to each other, on small screens */
</style>
</head>

<body>
  <header>
    <h5>GIS SMART ROAD SIGN</h5>
  </header>
    <div id="map"></div>
    <script>
      function initMap() {
        var map = new google.maps.Map(document.getElementById('map'), {
          zoom: 11,
          center: {lat: -1.2833, lng:	36.8167}
        });
        //added markers
        var locations = [
    {
      title: 'PEPSized Coffee',
      position:{lat: -1.2441032, lng:	36.8670072},
      icon: {
        url: "images/W17.png",
        scaledSize: new google.maps.Size(50, 50)
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2445234, lng: 36.8677181},
      icon: {
        url: "images/W30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.245054, lng: 36.8674831},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2451611, lng: 36.8677753},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2447317, lng: 36.868365},
      icon: {
        url: "images/W17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2450246, lng: 36.8682517},
      icon: {
        url: "images/W30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2465042, lng: 36.8690838},
      icon: {
        url: "images/8.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2470486, lng: 36.8698022},
      icon: {
        url: "images/9.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2470228, lng: 36.8703597},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.247163, lng: 36.8706004},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2471084, lng: 36.8740863},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2471335, lng: 36.8742765},
      icon: {
        url: "images/13.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2471831, lng: 36.8744416},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2472018, lng: 36.8751673},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.247502, lng: 36.8757834},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2474841, lng: 36.8758097},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2486004, lng: 36.8776239},
      icon: {
        url: "images/w12.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.248811, lng: 36.8778126},
      icon: {
        url: "images/W17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2490857, lng: 36.8777687},
      icon: {
        url: "images/20.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2492838, lng: 36.8780521},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2496965, lng: 36.878313},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2502178, lng: 36.878542},
      icon: {
        url: "images/23.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2513693, lng: 36.8788272},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.252211, lng:	36.8789579},
      icon: {
        url: "images/26,30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2525946, lng:	36.8789958},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2528285, lng:	36.8788562},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2514031, lng: 36.8788212},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.252211, lng: 36.8789579},
      icon: {
        url: "images/26,30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:-1.2525946, lng:	36.8789958},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2528285, lng: 36.8788562},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2530952, lng:	36.8790027},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.255737, lng: 36.8790809},
      icon: {
        url: "images/26,30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2560904, lng:	36.8791239},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2566341, lng:	36.8791296},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2573032, lng:	36.8789913},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.257451, lng:	36.879028},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2575582, lng:	36.8790531},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2601159, lng:	36.8790821},
      icon: {
        url: "images/36.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {	lat: -1.261465, lng: 36.8791981},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2619012, lng:	36.879089},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2623973, lng:	36.8796912},
      icon: {
        url: "images/39.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2626445, lng:	36.8791629},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2640099, lng:	36.8794262},
      icon: {
        url: "images/142.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.264656, lng:	36.8795918},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2648902, lng:	36.8796642},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2654424, lng:	36.8797985},
      icon: {
        url: "images/44.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2664403, lng: 36.8800479},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2666106, lng:	36.8800635},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2685464, lng:	36.8804257},
      icon: {
        url: "images/w30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.268855, lng:	36.8807191},
      icon: {
        url: "images/w30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2692756, lng:	36.8811893},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2694898, lng:	36.8816843},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2694969, lng:	36.8815211},
      icon: {
        url: "images/w30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2698191, lng:	36.8809397},
      icon: {
        url: "images/w25.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2706856, lng:	36.881168},
      icon: {
        url: "images/54.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2709185, lng: 	36.8812257},
      icon: {
        url: "images/w25.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.271315, lng:	36.8812522},
      icon: {
        url: "images/56.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2717744, lng:	36.8813393},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2764475, lng:	36.8824011},
      icon: {
        url: "images/58.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2784606, lng:	36.8838342},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2784532, lng:	36.8836323},
      icon: {
        url: "images/w30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2785299, lng:	36.8833307},
      icon: {
        url: "images/61.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2789282, lng:	36.8827102},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2814468, lng:	36.8831456},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2818266, lng:	36.8832532},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2844373, lng:	36.8839275},
      icon: {
        url: "images/65.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2862535, lng:	36.8842375},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2888181, lng:	36.8849348},
      icon: {
        url: "images/67.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2892574, lng:	36.8850478},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2895305, lng:	36.8851119},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.291007, lng:	36.88545},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2928913, lng:	36.8860139},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2932217, lng:	36.8860432},
      icon: {
        url: "images/72.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.294351, lng:	36.8874007},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2947297, lng: 	36.887656},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2951955, lng:	36.8863962},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2954701, lng:	36.8864031},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2956683, lng:	36.8864733},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2964113, lng:	36.886814},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2973557, lng:	36.8869625},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2993967, lng:	36.8873777},
      icon: {
        url: "images/82.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2997693, lng:	36.8872532},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.2998453, lat:	36.8873449},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3003815, lng:	36.887442},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3003947, lng:	36.8873789},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3012424, lng:	36.887782},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3029755, lng:	36.8880591},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3045065, lng:	36.8887194},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3047972, lng:	36.8886767},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3047689, lng:	36.8887476},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position:  {lat:	-1.3059204, lng:	36.8890},
      icon: {
        url: "images/92.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3067774, lng:	36.889575},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3069845, lng: 36.8896961},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3074913, lng:	36.8899499},
      icon: {
        url: "images/95.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.308119, lng:	36.8902952},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3083442, lng:	36.8902689},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.310389, lng:	36.8916212},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3103382, lng:	36.8917024},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3133815, lng:	36.8936279},
      icon: {
        url: "images/100.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3139588, lng: 36.8940077},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3148914, lng:	36.8944121},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3148452, lng:	36.8944863},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:	-1.3155686, lng:	36.8948847},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3158492, lng:	36.8950828},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3193115, lng:	36.8972372},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3193906, lng:	36.8972769},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3216103, lng:	36.8987007},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3216726, lng:	36.8987401},
      icon: {
        url: "images/109.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3222007, lng:	36.8990711},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3234172, lng:	36.8999929},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3229706, lng:	36.9009394},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3237944, lng:	36.900277},
      icon: {
        url: "images/113.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3234425, lng:	36.9009529},
      icon: {
        url: "images/w12.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3235315, lng:	36.9008045},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2450873, lng:	36.8662148},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2448828, lng:	36.8663602},
      icon: {
        url: "images/W30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2450117, lng:	36.867072},
      icon: {
        url: "images/W30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2455707, lng:	36.8674719},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.246153, lng:	36.8682287},
      icon: {
        url: "images/W30.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2475512, lng:	36.8734615},
      icon: {
        url: "images/121.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.247574, lng:	36.8740875},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2474965, lng:	36.8744508},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2494444, lng:	36.877871},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.24983, lng:	36.8781125},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2503308, lng:	36.8782508},
      icon: {
        url: "images/W17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2505758, lng:	36.8783363},
      icon: {
        url: "images/w12.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2528631, lng:	36.8786137},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2534912, lng:	36.8786026},
      icon: {
        url: "images/130.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2556498, lng:	36.8786779},
      icon: {
        url: "images/131.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2561039, lng:	36.8786615},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.257331, lng:	36.8788326},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.258865, lng:	36.8788018},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2590363, lng:	36.8788265},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2620344, lng:	36.8789532},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2625058, lng:	36.8783591},
      icon: {
        url: "images/138.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2625184, lng:	36.8782087},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2628081, lng:	36.8790288},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2631977, lng:	36.8789642},
      icon: {
        url: "images/140.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2642063, lng:	36.8791448},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2650662, lng:	36.8794422},
      icon: {
        url: "images/41.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2659421, lng:	36.8796641},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2664701, lng:	36.879788},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2672598, lng:	36.8799829},
      icon: {
        url: "images/145.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2679871, lng:	36.8800558},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2713752, lng:	36.8808863},
      icon: {
        url: "images/147.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2715127, lng:	36.8804536},
      icon: {
        url: "images/W17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2714127, lng:	36.8810181},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2718583, lng:	36.8811204},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.27213, lng:	36.8811136},
      icon: {
        url: "images/151.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2723692, lng:	36.8811589},
      icon: {
        url: "images/W17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2726274, lng:	36.8812228},
      icon: {
        url: "images/w12.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2742926, lng:	36.8816043},
      icon: {
        url: "images/154.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.278116, lng:	36.8823522},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2809802, lng:	36.8827172},
      icon: {
        url: "images/156.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2858028, lng:	36.8839095},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.286311, lng:	36.8841092},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2910691, lng:	36.8853158},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2920149, lng:	36.8854639},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2931045, lng:	36.8856476},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2960992, lng:	36.8862038},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.296732, lng:	36.8863571},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.29816, lng:	36.8866463},
      icon: {
        url: "images/166.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2986752, lng:	36.8864831},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.2998884, lng:	36.8871194},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3004513, lng:	36.8872335},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3004767, lng:	36.8871199},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat:-1.3017355, lng:	36.8873212},
      icon: {
        url: "images/180.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.303098, lng:	36.8879307},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3031318, lng:	36.8878652},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3048785, lng:	36.8885434},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3049109, lng:	36.8884622},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.306135, lng:	36.8890259},
      icon: {
        url: "images/entry.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3067949, lng:	36.8893259},
      icon: {
        url: "images/92.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3082908, lng:	36.8897183},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3090134, lng:	36.8902046},
      icon: {
        url: "images/179.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3100981, lng:	36.8908787},
      icon: {
        url: "images/1800.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3104348, lng:	36.8910508},
      icon: {
        url: "images/141.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3104936, lng:	36.8915033},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3106499, lng: 36.8912533},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3120649, lng:	36.8920646},
      icon: {
        url: "images/184.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3138109, lng:	36.8934838},
      icon: {
        url: "images/xxx.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3140459, lng:	36.8936472},
      icon: {
        url: "images/exit.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3149928, lng:	36.8943005},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.317885, lng:	36.895695},
      icon: {
        url: "images/188.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.318306, lng:	36.8960561},
      icon: {
        url: "images/xxx.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3183445, lng:	36.8962937},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3187225, lng:	36.8962418},
      icon: {
        url: "images/// xxx.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3210257, lng:	36.8976795},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3212894, lng:	36.8981702},
      icon: {
        url: "images/xxx.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3227745, lng:	36.8991713},
      icon: {
        url: "images/p15.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3238712, lng:	36.8996523},
      icon: {
        url: "images/r2.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3239524, lng:	36.899376},
      icon: {
        url: "images/196.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3241371, lng:	36.8999578},
      icon: {
        url: "images/w37.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3245133, lng:	36.9001216},
      icon: {
        url: "images/w12.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    {
      title: 'PEPSized Office',
      position: {lat: -1.3245932, lng:	36.9001923},
      icon: {
        url: "images/w17.png",
        scaledSize: new google.maps.Size(50, 50),
      }
    },
    ];
    locations.forEach( function( element ) {
    var marker = new google.maps.Marker({
      position: element.position,
      map: map,
      title: element.title,
      icon: element.icon,
    });
    });
      }
    </script>
    <script async defer
     src="https://maps.googleapis.com/maps/api/js?key=AIzaSyBQ8UuCXFfZ6FA7vCeXEhcvw4SM4UaxTiY &callback=initMap">
     </script>


</body>
</html>
