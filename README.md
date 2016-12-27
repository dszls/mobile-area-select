# mobile-area-select
手机端省市区三级联动菜单、下拉菜单插件,模拟原生效果

## html 结构

> 可以绑定Input对象或其它DOM对象，选择确定后会自动赋值或通过onChange回调方法再做其它操作，

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

## 属性列表 
*   data：默认值"json/address.json",数据访问路径或数组对象
*   code：默认值"code",数据节点参数名称
*   name：默认值"name",数据节点显示文本名称
*   childName：默认值"",二三级节点名称
*   value：默认值[],选中的数据
*   level：默认值3,几级菜单
*   separator：默认值" ",地址名称间隔符号
*   isMaskClose：默认值true,是否给mask填加关闭弹层事件
*   isDefault：默认值false ,显示配置的value对应的文本
*   onChange：回调函数

