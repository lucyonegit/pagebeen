# pagebeen
jquery分页插件

# 用法
### 一  引入js、css文件
```js
<link href="./pager/Pager.css" rel="stylesheet" type="text/css" />
<script src="jquery-1.3.2.min.js" type="text/javascript"></script>
<script src="jquery.pager.js" type="text/javascript"></script>
<script type="text/javascript" language="javascript">
    $(document).ready(function() {
        $("#pager").pager({ pagenumber: 1, pagecount: 5, buttonClickCallback: PageClick });
    });

    var PageClick = function(pageclickednumber) {
        $("#pager").pager({ pagenumber: pageclickednumber, pagecount: 5, buttonClickCallback: PageClick });
        console.log(pageclickednumber);
    }
</script>
```
### 二  在html文档中添加组件
```html
<div id="pager"></div>
```
![](https://github.com/lucyonegit/pagebeen/blob/master/pre/demo.jpg)

