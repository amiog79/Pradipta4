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
    font-size: 60px;

}

span{

  background: pink;  
  
}

span:hover{

    background: black;
    color: yellow;
}

h1{

    font-size: 40px;
    background: red;
    color: white;
}


</style>

</head>
<body>

<h1>MADE BY PRADIPTA GHOSH</h1>

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

<iframe width="1000" height="600" src="https://www.youtube.com/embed/UOhDLO5TMhQ">
</iframe>

<!--END NO-1 VIDEO-->

<!--YOUTUBE VIDEO 2-->
<iframe width="1000" height="600" src="https://www.youtube.com/embed/bQNX4EdFlz4">
</iframe>

<!--END NO-2 VIDEO-->

<center style="font-size:16px;background:red"><u><a style="color:white;">Privacy Policy</a></u> <u><a style="color:white">Terms & Conditions</a></u></center>
<center style= "color:black;font-size:16px;background:#17D4FE">Copyright © By Pradipta Ghosh.com 2019</center>

</body>
</html>



<!--ONLINE USERS-->


<html>
<head>
  <title>Currently Active Demo</title>
  <style type="text/css">
    .currently-active {
      position: fixed;
      margin: 10px;
      padding: 5px;
      bottom: 0;
      left: 0;
      border: solid 1px #AFAFAF;
      border-radius: 6px;
      font-family: "Arial";
    }

    div{
      background: yellow;
      font-size: 26px;
      
    }


  </style>
</head>
<body>
  <div class="currently-active">
    <span>Currently Active: </span><span id="active"></span>
  </div>
</body>
<script src="https://cdn.pubnub.com/sdk/javascript/pubnub.4.20.2.js"></script>
<script type="text/javascript">
var active = document.getElementById('active');
function setCurrentlyActiveUsers(numberOfUsers) {
  active.innerText = numberOfUsers.toString();
}
setCurrentlyActiveUsers(1);
var pubnub = new PubNub({
    publishKey : '__YOUR_PUB_KEY__',
    subscribeKey : '__YOUR_SUB_KEY__',
    heartbeatInterval: 30
});
pubnub.addListener({
  presence: function(presenceEvent) {
    setCurrentlyActiveUsers(presenceEvent.occupancy);
  }
});
pubnub.subscribe({ 
  channels: ['myWebPage1'],
  withPresence: true
});
</script>
</html>


<!--END ONLINE USERS-->
