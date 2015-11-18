# mobile-area-select
手机端地区三级联动菜单插件，模拟原生效果

## html 结构

> 选择地区确定后会自动赋值给next(':hidden')对象

    <input type="text" id="area" value="" data-value="" readonly="readonly"/>
   	<input type="hidden" id="hd_area" value=""/>

## 调用方法 	
	

    <script>
	$("#area").mobileAreaSelect({
    	data:"address.json",//json数据路径或者json对象
    	separator:' ',//设置地址名称间隔符号，默认为空格字符
    	isMaskClose:true,//是否给mask填加关闭弹层事件
		onChange:function(){
		    //点击确定后的回调函数
			console.log("点击确定了");
		}
	});
	</script>
