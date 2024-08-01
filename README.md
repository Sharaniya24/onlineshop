<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>jQuery Slider Menu</title>
<script type="text/javascript" src="jquery-1.2.6.min.js"></script>

<style type="text/css">
body {
margin: 0;
font-size:16px;
color: #000000;
font-family:Arial, Helvetica, sans-serif;
}
#sliderWrap {
margin: 0 auto;
width: 300px;
}
#slider {

position: absolute;
background-image:url(slider.png);
background-repeat:no-repeat;
background-position: bottom;
width: 300px;
height: 159px;
margin-top: -141px;
}
#slider img {
border: 0;
}
#sliderContent {
margin: 30px 0 0 30px;
position: absolute;
text-align:top_left;
color:#333333;
font-weight:simple;
padding: 10px;
}
#header {
margin: 0 auto;
width: 600px;
background-color: #F0F0F0;
height: 200px;
padding: 10px;
}
#openCloseWrap {
position:absolute;
margin: 143px 0 0 120px;
font-size:12px;
font-weight:bold;
}
</style>

</head>
<body>


	<script type="text/javascript">
	$(document).ready(function() {
		$(".topMenuAction").click( function() {
			if ($("#openCloseIdentifier").is(":hidden")) {
				$("#slider").animate({ 
					marginTop: "-141px"
					}, 500 );
				$("#topMenuImage").html('<img src="open.png" alt="open" />');
				$("#openCloseIdentifier").show();
			} else {
				$("#slider").animate({ 
					marginTop: "0px"
					}, 500 );
				$("#topMenuImage").html('<img src="close.png" alt="close" />');
				$("#openCloseIdentifier").hide();
			}
		});  
	});
	</script>
	
	
	
	<div id="sliderWrap">
		<div id="openCloseIdentifier"></div>
		<div id="slider">
			<div id="sliderContent">
			<span style="text-shadow: 0px 0px 4px purple;"><blink>Developed By:<br>kuroshinibalakumar<br>
			    Contact:0752713422<br></span>
				
			</div>
			<div id="openCloseWrap">
				<a href="#" class="topMenuAction" id="topMenuImage">
					<img src="open.png" alt="open" />
				</a>
			</div>
		</div>
	</div>
	
	
	
	


</body>
</html>

