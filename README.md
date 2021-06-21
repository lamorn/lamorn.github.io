<html>
<head>
<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0"/>
<!-- 自适应代码 -->
<body bgcolor="#CCFFCC">

    <style type="text/css">
        .res
        {
            color: Red;
        }
		.result{
			background: yellow;
		}
		

.MODS {
float: left;
margin: 5px;
padding: 15px;
width: 300px;
height: 300px;
border: 1px solid black;
} 
	
    </style>
    <script src="https://code.jquery.com/jquery-3.3.1.min.js" type="text/javascript"></script>
    <script type="text/javascript">
        var oldKey = "";
        var index = -1;
        var pos = new Array();//用于记录每个关键词的位置，以方便跳转
        var oldCount = 0;//记录搜索到的所有关键词总数
		
		function previous(){
			index--;
            index = index < 0 ? oldCount - 1 : index;
			search();
		}
		function next(){
			index++;
            //index = index == oldCount ? 0 : index;
			if(index==oldCount){
				index = 0 ;
			}
			search();
		}
 
        function search() {
            $(".result").removeClass("res");//去除原本的res样式
            var key = $("#key").val(); //取key值
            if (!key) {
				console.log("key为空则退出");
				$(".result").each(function () {//恢复原始数据
                    $(this).replaceWith($(this).html());
                });
                oldKey = "";
                return; //key为空则退出
            }
            if (oldKey != key) {
				console.log("进入重置方法");
                //重置
                index = 0;
                $(".result").each(function () {
                    $(this).replaceWith($(this).html());
                });
                pos = new Array();
				var regExp = new RegExp(key+'(?!([^<]+)?>)', 'ig');//正则表达式匹配
                $("body").html($("body").html().replace(regExp, "<span id='result" + index + "' class='result'>" + key + "</span>")); // 高亮操作
                $("#key").val(key);
                oldKey = key;
                $(".result").each(function () {
                    pos.push($(this).offset().top);
                });
                oldCount = $(".result").length;
				console.log("oldCount值：",oldCount);
            }
 
            $(".result:eq(" + index + ")").addClass("res");//当前位置关键词改为红色字体
 
            $("body").scrollTop(pos[index]);//跳转到指定位置
        }
    </script>
    <title>标题不会显示在文档区</title>
    
</head>

<font face="Times New Roman" color="#FF6666">
    
    <br>
<h1>This is a heading</h1>
<body>

   <div style="position: fixed; right: 20px; top: 0;">
        <input id="key" type="text" style="width: 100px;"/>
        <input type="button" value="下一个" onclick="next()" />
        <input type="button" value="上一个" onclick="previous()" />
    </div>
  <!-- 内容案例    
  <div style="height: 100px;">
    </div>
    -->
<center>   
   
<!-- 开头 -->  
<div class="MODS">  

<summary>0核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    


<!-- 开头 -->  
<div class="MODS">  
    
<summary>1核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>2核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>3核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>4核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>5核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>6核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>7核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->    

<!-- 开头 -->  
<div class="MODS">  
    
<summary>8核心必备
&nbsp;&nbsp;&nbsp;&nbsp;<button type="button">
<a style="text-decoration:none" href="#">
<font size="3" color="#009966">备用下载</font></button></summary></a>

<!-- 文字描述 -->
<p>All pages and graphics on this web site are the property of W3School.</p>

<!-- 内容图片 -->
<p><img src="/i/eg_mouse.jpg" width="200" height="200" />
</p>

</div>
<!-- 结尾 -->   

</font>

<center>

</body>

<footer>

  <p>Posted by</p>

  <p>如有问题请联系我: <a href="mailto:lamorn@163.com">联系方式</a>.</p>
</footer>
</html>
