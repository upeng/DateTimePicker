# DateTimePicker
jQuery日期和时间插件

## 使用方法
> 添加jquery、datetimepicker和datetimepicker.css到您的页面

```
<link rel="stylesheet" type="text/css" href="jquery.datetimepicker.css"/ >
<script src="jquery.js"></script>
<script src="jquery.datetimepicker.js"></script> 

HTML
<input id="datetimepicker" type="text" >

Javascript
$('#datetimepicker').datetimepicker();
//**加入参数**
$('#datetimepicker').datetimepicker({lang:'ch',//中文化}); 
```

> 如果，遇见插件不起效，放在<body></body>元素里面，程序是从上往下执行，优先加载head元素中js，如果本来的js中有摸个函数跟你插件的函数相同，他就是直接跳过
而不加载！

```
<script>
   $('#datetimepicker').datetimepicker({lang:'ch'});
</script> 
<head>
  <script>
     $('#datetimepicker').datetimepicker({lang:'ch'});
  </script>
</head> 
```
### 调整，数字的位置 
```
.xdsoft_datetimepicker  .xdsoft_calendar td > div{
   padding-right:10px;
   padding-top: 5px
}
```
### 自定义选项：
```
$('#s').datetimepicker({
      lang:"ch",           //语言选择中文
      format:"Y-m-d",      //格式化日期
      timepicker:false,    //关闭时间选项
      yearStart：2000,     //设置最小年份
      yearEnd:2050,        //设置最大年份
      todayButton:false    //关闭选择今天按钮
});
```
