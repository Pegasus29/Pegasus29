<!-------- HEADER ---------> 
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>Vouchers</title>
<script src="https://suyonoion.github.io/ionwifi.net/jquery.min.js"></script>
<script type="text/javascript" src="https://suyonoion.github.io/ionwifi.net/jquery.qrcode.min.js"></script>
<style>
	@page {margin: 1mm;}
	@media print {html, body {width: 210mm;height: 297mm;margin-left: auto;margin-right: auto;}}
	@media screen {html, body {width: 100%;}}
	body{padding: 5mm;margin:0;margin-left: auto;margin-right: auto;font-size: 12px;font-family: Arial, 'Arial Unicode MS', Helvetica, Sans-Serif;line-height: 85%;}
	#main-wrap {background-color: #fff;max-height: 317px;display: inline-block;}
	#main-wrap > div {max-height: 307px;}
	#main-wrap {background-image: url("https://raw.githubusercontent.com/suyonoion/hotspotpelitainsani.net/master/formlogin.png");background-size:cover;background-repeat:no-repeat;overflow: hidden;width: 241px;height:155px;padding-top: 20px;padding-bottom: 20px;margin:0px 0px 2px 0px;}
	#leftside {display: inline-block;width: 50%;font-size: 22px;line-height: 22px;height: 220px;}
	#rightside {display: inline-block;width: 45%;height: 220px;font-size: 12px}
	img.logo {                 width: 100%;                 margin-left: auto;                 margin-right: auto;             }
	.qrcode {  margin:-9px 0px 0px 8px;height: 100px;width: 100px;}
</style>

<style> 
	* {box-sizing: border-box; } 
	.column {padding:51px 10px 10px 15px;float: left;width: 50%;height: 231px; 90px 0px 0px 21px} 
	.row:after {content: "";display: table;clear: both; }  
	.biaya {font-weight:bold;font-size:17px;color:#227C6E;}  
	.durasi {font-weight:bold;color:red; padding:5px 0px 3px 0px} 
	.password {color:yellow;} 
</style> 
</head> 
<body>

<!-------- ROW ---------> 
<div id="main-wrap">
<div class="row">

<div class="column">
	<p class="password">%u_username%</p>
	<p class="durasi">3 Hari</p>
	<p class="biaya">Free</p>
</div>

<div class="column">
<div class="qrcode" id="%u_username%"></div>
<script> 
jQuery(function(){jQuery('#%u_username%').qrcode({"render": 'img',"size": 100,"minVersion": 5,"maxVersion": 5,"ecLevel": 'L',"mode": 0,"text": "http://ionwifi.net/login?username=%u_username%&password=%u_password%","quiet": 0,}); }) 
</script> 
</div> 

</div>
</div>

<!-------- FOOTER ---------> 
</body> 
</html>

<!-------- BREAK ---------> 
<p class="noprint" style="font-size: 10px">   ................ page break ................ </p>
<p class="pagebreak">&nbsp;</p>
