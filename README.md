
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

