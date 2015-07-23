# RT_9_Tonenchuk
<!DOCTYPE html>
<html>
<head>
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.8.3/jquery.min.js">
</script>
<script type="text/javascript">

var i=0;
$(document).ready(function () 
{
$("#but1").click(function () 
   {
	
      while (i<6)
          {
              i++;
              $("#div1").fadeIn();
              $("#div2").fadeIn();
              $("#div2").delay(1000).fadeOut(2000);
           }
   });
$("#but2").click(function () 
   {
                $("#div1").fadeIn();                
                $("#div2").stop($("#but1").click());
                $("#div2").hide();
                $("#div2").fadeIn();
   });
});
</script>
</head>

<div id="div1" style="width:80px;height:80px;display:none;background-color:red;"></div><br>
<div id="div2" style="width:80px;height:80px;display:none;background-color:blue;"></div><br>
<p></p>
<button id="but1">Click me</button>
<button id="but2">Click me for stop it</button>

</body>

</html>
