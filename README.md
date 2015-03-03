# tinger
选项卡
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>选项卡</title>
<style type="text/css">
	*{margin:0; padding:0; font-size:12px; font-family:"微软雅黑",Arial; list-style:none; border:0;}
	#tab{width:480px; margin:10px auto; height:400px; overflow:hidden;}
	#tab ul{ height:80px;}
	#tab ul li{width:80px; height:80px;float:left; cursor: pointer; color:#fff; text-align:center; opacity:0.4;filter:alpha(opacity=40); background:#C3F;}
	#tab ul span{display:block; width:80px; height:60px; float:left;}
	#tab ul .li1{ background:url(imges/tu1.png) no-repeat #99C;}
	#tab ul .li2{ background:url(imges/tu2.png) no-repeat #3F9;}
	#tab ul .li3{ background:url(imges/tu3.png) no-repeat #39F;}
	#tab ul .li4{ background:url(imges/tu4.png) no-repeat #99C;}
	#tab ul .li5{ background:url(imges/tu5.png) no-repeat #3F9;}
	#tab ul .li6{ background:url(imges/tu6.png) no-repeat #39F;}
	#tab ul .li_current{ opacity:1;filter:alpha(opacity=100);}
	#tab ul .li_currentl{opacity:0.4;filter:alpha(opacity=40);}
	#tab div{display:none; clear:both; height:200px;}
	#tab .div_current{display:block;}
	
</style>
</head>

<body>
<div id="tab">
	<ul>
    	<li class="li_current"><span class="li1"></span>自如转换</li>
        <li><span class="li2"></span>多任务处理</li>
        <li><span class="li3"></span>触控打字</li>
        <li><span class="li4"></span>首款window8</li>
        <li><span class="li5"></span>灵活高效</li>
        <li><span class="li6"></span>持续8小时</li>
    </ul>
    <div class="div_current"><a href="#"><img src="imges/tu13.jpg" width="482" height="320" /></a></div>
    <div><a href="#"><img src="imges/tu14.jpg" width="480" height="320" /></a></div>
    <div><a href="#"><img src="imges/tu15.jpg" width="482" height="320" /></a></div>
    <div><a href="#"><img src="imges/tu16.jpg" width="482" height="320" /></a></div>
    <div><a href="#"><img src="imges/tu17.jpg" width="482" height="320" /></a></div>
    <div><a href="#"><img src="imges/tu18.jpg" width="482" height="320" /></a></div>


</div>
</body>
</html>
<script type="text/javascript">
	var aLis= document.getElementById("tab").getElementsByTagName("li");
	var aDivs = document.getElementById("tab").getElementsByTagName("div");
	
	for(var i=0; i<aLis.length; i++){
		aLis[i].index = i;
		aLis[i].onmouseover = function(){
			sum(this.index);
		};;
	};
	function sum(nIndex){
		for(var i=0; i<aLis.length; i++){
			//var aLi = aLis.item(i);
			//var aDiv = aDivs.item(i);
			aLis[i].className=null;
			aDivs[i].className = null;
		};
		aLis[nIndex].className="li_current";
		aDivs[nIndex].className="div_current";
		
	};
</script>
































