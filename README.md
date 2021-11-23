# Pradipta4
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>

    <!-- Bootstrap -->
  <link rel="stylesheet" href="plugins/bootstrap/bootstrap.min.css">

<style>
    
body{

    background: lightgreen;
    text-align: center;
    font-size: 50px;

}


h1{

    font-size: 25px;
    background: red;
    color: white;
}

 div{
      background: darkgrey;
      font-size: 25px;
      
    }   
    
span{

    font-size: 30px;
     background: #17D4FE;
     color: black;
}    
   

</style>

</head>
<body>

    <div><h1 style="font-size:25px;"> MADE BY PRADIPTA GHOSH </h1></div>

<a class='yt-subscribe-button' rel="noopener nofollow" href='https://www.youtube.com/c/BONGOMALA?sub_confirmation=1' target='_blank'>
    <span><svg viewBox="0 0 24 24" width="16" style='margin:-2px 4px 0 0'>
        <path
            d="M23.495 6.205a3.007 3.007 0 0 0-2.088-2.088c-1.87-.501-9.396-.501-9.396-.501s-7.507-.01-9.396.501A3.007 3.007 0 0 0 .527 6.205a31.247 31.247 0 0 0-.522 5.805 31.247 31.247 0 0 0 .522 5.783 3.007 3.007 0 0 0 2.088 2.088c1.868.502 9.396.502 9.396.502s7.506 0 9.396-.502a3.007 3.007 0 0 0 2.088-2.088 31.247 31.247 0 0 0 .5-5.783 31.247 31.247 0 0 0-.5-5.805zM9.609 15.601V8.408l6.264 3.602z"
            fill='#fff'
        ></path>
    </svg>SUBSCRIBE</span>
    <span>CHANNEL</span>
</a>

<!--YOUTUBE VIDEO 1-->

<iframe src="https://www.youtube.com/embed/UOhDLO5TMhQ">
</iframe>

<!--END NO-1 VIDEO-->

<!--YOUTUBE VIDEO 2-->
<iframe src="https://www.youtube.com/embed/bQNX4EdFlz4">
</iframe>

<!--END NO-2 VIDEO-->
    
<!--GOOGLE MAP-->

<html lang="en-US">
<head>
  <meta charset="UTF-8">
  <title></title>
  <style type="text/css">
  #map_canvas {
    height: 300px;
    width: 300px;
  }
  </style>
</head>
<body>
<div id="map_canvas" width="300" height="300"></div>
<input type="text" id="query" value=""/>
<input type="submit" id="search" value="search"/>
<script src="http://maps.googleapis.com/maps/api/js?sensor=false" src="//maps.google.com/maps/api/js?sensor=false"></script>
<script type="text/javascript">
var geo = {};
window.onload = function() {
  var latlng = new google.maps.LatLng(39.102431, -94.583698),
      options  = {
        zoom               : 4,
        mapTypeId          : google.maps.MapTypeId.TERRAIN,
        center             : latlng,
        streetViewControl  : true,
        scaleControl       : true,
        scrollwheel        : true,
        mapTypeControl     : true,
        overviewMapControl : true,
        panControlOptions  : {
          position         : google.maps.ControlPosition.TOP_LEFT
        },
        zoomControlOptions : {
          position         : google.maps.ControlPosition.TOP_LEFT
        }
      };
      map    = new google.maps.Map(document.getElementById('map_canvas'), options),
      marker = new google.maps.Marker({
                     position  : latlng,
                     map       : map,
                     draggable : false
                   }),
      geocoder = new google.maps.Geocoder(),
      search = document.getElementById('search'), 
      query = document.getElementById('query');

  function codeAddress() {
    var address = query.value;
    geocoder.geocode( { 'address': address}, function(results, status) {
      console.log(results);
      if (status == google.maps.GeocoderStatus.OK) {
        map.setCenter(results[0].geometry.location);
        var marker = new google.maps.Marker({
            map: map,
            position: results[0].geometry.location
        });
      } else {
        alert("Geocode was not successful for the following reason: " + status);
      }
    });
  };

  search.onclick = function() {
   codeAddress(); 
  };
};
</script>
</body>
</html>



<!--END GOOGLE MAP-->
    
    

<center style="font-size:16px;background:red"><u><a style="color:white;">Privacy Policy</a></u> <u><a style="color:white">Terms & Conditions</a></u></center>
<center style= "color:black;font-size:16px;background:#17D4FE">Copyright © By Pradipta Ghosh.com 2019</center>

</body>
</html>


