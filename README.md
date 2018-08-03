# js
js的三种使用方式（行内js、内部js、外部js）

1、行内js：js不单独写出
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>js使用方式1：行内js</title>
</head>
<body>
<input type="button" value="点击有惊喜" onclick="javascript:alert('哈哈哈哈')">
<!--onclick:点击触发一个事件，alert：弹出一个对话框-->
</body>
</html>

```
2、内部js：script里的程序整个页面都可以用
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>js使用方式2：内部js</title>
    <script type="text/javascript">
        //声明一个函数(整个文档都可以使用)
        function surprise() {
            alert('恭喜你中了一百万')/*弹出框*/
        }
    </script>
</head>
<body>
<input type="button" value="点击有惊喜" onclick="surprise()"><!--调用函数-->
<input type="button" value="点击" onclick="surprise()">
</body>
</html>

```
3、外部js：很多html页面都可以调用设定的js页面
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>js使用方式3：外部js</title>
    <!--很多html页面都可以调用js4.js页面-->
    <script src="../../js/js4.js" type="text/javascript" charset="utf-8">
    </script>
</head>
<body>
<input type="button" value="点击" onclick="test()">
</body>
</html>

```
