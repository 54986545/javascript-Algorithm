# javascript-Algorithm
javascript算法
<!doctype html>
<html>
<head>
<script type="text/javascript" src="jquery-2.1.1.js"></script>
<style>

#box{position: absolute;width: 200px;height: 200px;background: red;}
</style>

</head>
<body>

<input type="button" value="开始计时！" accesskey="h">
<input type="text" id="txt" accesskey="a">
<div id="111"><div id="333">2222</div></div>
<input type="button" value="停止计时！" onClick="stopCount()">
</body>
</html>
<script type="text/javascript">
var arry=[6,4,5,3,8,7,1,9,2];
for(var i=0;i<arry.length;i++)
{
  var min=i;
  for(var j=i+1;j<arry.length;j++){
	  if(arry[j]<arry[min]){
	  		min=j;
  	}
  }
  //最小数arry[min]
  
  
 // var minNumber=arry[min];
 // arry[min]=arry[i];
 // arry[i]=minNumber;
				 var temp = arry[i];
             //把最小数索引对应的值放到最左边
             arry[i] = arry[min];
             //把原来最左边对应的值放到最小数索引所在的位置
             arry[min] = temp;

  
}
alert(arry);
</script>
