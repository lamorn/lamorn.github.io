<head>

<title>Yun Demo</title>

<style type="text/css">

body {
	font: 1em/150% Arial, Helvetica, sans-serif;
}
a {
	color: #669;
	text-decoration: none;
}
a:hover {
	text-decoration: underline;
}
h1 {
	font: bold 30px/100% SimSun,"Times New Roman",Serif;
}
 
/************************************************************************************
STRUCTURE 

*************************************************************************************/
#pagewrap {
	padding: 0px;
	width: 680px;
	margin: 0px auto;
}
#header {
	height: 120px;
}
#content {
	width: 680px;
	float: right;
    font-family: SimSun,"Times New Roman",Serif;
}

#sidebar {
	width: 680px;
	float: right;
}
#footer {
	
	clear: both;
	
}

 
/************************************************************************************
MEDIA QUERIES
*************************************************************************************/
/* for 980px or less */
@media screen and (max-width: 980px) {
	
	#pagewrap {
		width: 94%;
	}
	#content {
		width: 65%;
	}
	#sidebar {
		width: 30%;
	}
 
}
 
/* for 700px or less */
@media screen and (max-width: 700px) {
 
	#content {
		width: auto;
		float: none;
	}
	#sidebar {
		width: auto;
		float: none;
	}
 
}

/* border guideline (you can ignore these) */
#content {
	background: #fff;
}
#sidebar {
	background: #fff;
}
#header, #content, #sidebar {
	margin-bottom: 1px;
}
#pagewrap, #header, #content, #sidebar, #footer {
	border: solid 0px #ccc;
}
 <!-- 注释:边框 -->



</style>
</head>
 
<body>


<div id="pagewrap">
 
	<div id="header">
		<h1 style="text-align:center">实践是检验真理的唯一标准</h1>
		
		<p style="font-family:Times New Roman; font-size:16px;">
<a style=" color: #000;" href="#" >首页</a>&emsp;
<a style=" color: #000;" href="#" >实验</a>&emsp;
<a style=" color: #000;" href="#" >交流</a>&emsp;
<a style=" color: #000;" href="#" >工具 </a>&emsp;
</p>
 <!-- 内容 -->
	<div id="content">
<!-- 标题 -->
		<h2 style="font-family:Times New Roman; font-size:20px;">原文内容</h2>
<!-- 目录 -->
<table border="0" width=100% >
  <tr>
    <td>
    <a style=" color: #000;" href="#" >
    检验真理的标准只能是社会实践</a></td>
    <td align="right">
   <time>1978-05-11</time>
   </td>
</tr>
  <tr>
    <td>
    <a style=" color: #000;" href="#" >
    任何理论都要不断接受实践的检验</a></td>
    <td align="right">
   <time>1978-05-11</time>
   </td>
</tr>

	</div>
<!-- 底部 -->	
	<div id="footer">
	<hr style="height:0px;border:none;border-top:3px double #ccc;" /> 

<a style="text-decoration: none; color: #ccc;font-size:1px; " href="#" title="注释">©2021</a>
<a style="text-decoration: none; color: #ccc;font-size:1px; " href="#">lamorn.</a>
<a style="text-decoration: none; color: #ccc;font-size:1px; " href="#" title="注释">Blog README.</a>

	</div>
 
</div>
