# MDtoHTML
MDtoHTML可以快速将Markdown文件转换为HTML

### 环境要求
* PHP且 && CURL

### 示例
```
<!DOCTYPE html>
<html lang="zh-cmn-Hans" xmlns="http://www.w3.org/1999/xhtml">
<head>
	<meta charset="utf-8" />
	<title>MDtoHTML</title>
	<meta name="generator" content="EverEdit" />
	<meta name="author" content="" />
	<meta name="keywords" content="" />
	<meta name="description" content="" />
</head>
<body>
	<div id="mdtohtml"></div>
	<script src="https://cdn.bootcss.com/jquery/2.2.4/jquery.min.js"></script>
	<script>
		$(document).ready(function(){
			$.get("http://markdown.win/api.php?url=http://markdown.win/README.md",function(data,status){
				if(status == 'success') {
					$("#mdtohtml").html(data);
				}
			});
		});
	</script>
</body>
</html>
```

### 演示地址
* [http://markdown.win/](http://markdown.win/api.php?url=https://raw.githubusercontent.com/helloxz/IPinfo/master/readme.md)
