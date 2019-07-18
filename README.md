# preview-photo-with-html5
## preview-photo-with-html5
## exif.js获取exif信息。
## JQueryRotate.js 不同设备可能会显示旋转的图片，获取exif信息摆正。
## 使用css3将图片旋转移动
 ```
 $("#preview").css({"transform":"translate("+a+"px,"+b+"px) rotate(90deg)"});
```
使用css样式垂直居中：
```
{
    display: table-cell;
    text-align:center;
    vertical-align: middle;
}
```
使用外层div#container旋转不会出现错位，直接旋转img会出现错位
```
 $("#container").css({"transform":"rotate(90deg)"}); 
 ```
## weinre远程调试
```
npm -g install weinre
weinre -boundHost 192.168.2.185 -httpPort 8000
```
全局安装并运行到指定ip和端口
然后将ip和端口写入到所嵌入的需要调试的html中
```
<script src="http://192.168.2.185:8000/target/target-script-min.js#anonymous"></script>
```
在PC端即可访问
```
http://192.168.2.185:8000/client/#anonymous
```
来查看控制台输出等调试功能

# webcam与canvas

https://developer.mozilla.org/zh-CN/docs/Web/API/MediaDevices/getUserMedia
http://www.w3school.com.cn/tags/html_ref_canvas.asp
https://developer.mozilla.org/zh-CN/docs/Web/API/Canvas_API/Tutorial