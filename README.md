# Beautify-cnblogs
Beautify-cnblogs

The method and relatd code to make your cnblogs looks more beautiful.

# 前端小白/渣 也能快速学会的博客园博客美化全攻略

## 美化方法论简介

一般而言，需要选一个默认的skin，然后在该基础上调整。
宽屏模版：
Minyx2_Lite
lessIsMore
BlueSky

组成及对应关系

园子 - 博客园 https://home.cnblogs.com/feed/all/
进博客园首页，发状态@博客园团队，申请开头js权限。

## 准备工作

### js权限申请
(需要截图)

登陆后点击“我的博客”——“管理”——“设置”———在下拉后找到“博客侧边栏公告”，后方有一个“申请js权限”。

源码:
yanglr/Beautify-cnblogs: Beautify-cnblogs
<https://github.com/yanglr/Beautify-cnblogs>




## 如何模仿一个博客园的自定义风格(样式css+动态效果js)?

模仿一个cnblogs

```css
<link id="MainCss" type="text/css" rel="stylesheet" href="/skins/LessIsMore/bundle-LessIsMore.css?...">

<link type="text/css" rel="stylesheet" href="/blog/customcss/198996.css?v=...">
```


宽屏模版：
Minyx2_Lite
lessIsMore
BlueSky

补充完整前缀：http://www.cnblogs.com
即可进行模仿。


## markdown样式自定义
默认markdown状态下，代码中的字比较小。

```css
/* 文章标题样式(这个不是markdown里的标题) */
#topics .postTitle a {
    /* color: #169fe6; */
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	font-weight: bold;
}
 
/* 普通文字样式 */
#cnblogs_post_body p {
	margin: 18px auto;
	color: #000;
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	font-size: 16px;
	text-indent: 0;
}
 
/* 标题样式 */
#cnblogs_post_body h1 {
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	font-size: 32px;
	font-weight: bold;
	line-height: 1.5;
	margin: 10px 0;
}

#cnblogs_post_body h2 {
	font-family: Consolas, "Microsoft YaHei", monospace;
	font-size: 26px;
	font-weight: bold;
	line-height: 1.5;
	margin: 20px 0;
}

#cnblogs_post_body h3 {
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	font-size: 20px;
	font-weight: bold;
	line-height: 1.5;
	margin: 10px 0;
}

#cnblogs_post_body h4 {
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	font-size: 18px;
	font-weight: bold;
	margin: 10px 0;
}
/* 标题样式设置结束 */
 
/* 去除双下划线斜体样式 */
em {
	font-style: normal;
	color: #000;
}
 
/* 无序列表 */
#cnblogs_post_body ul li {
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	color: #000;
	font-size: 16px;
	list-style-type: disc;
}
 
/* 有序列表 */
#cnblogs_post_body ol li {
	font-family: Georgia,Times New Roman,Times,sans-serif, monospace;
	color: #000;
	font-size: 16px;
	list-style-type: decimal;
}
 
/* 超链接 */
#cnblogs_post_body a:link {
	text-decoration: none;
	color: #002C99;
}
 
/* 引用背景 */
#topics .postBody blockquote {
	background: #fff3d4;
	border: none;
	border-left: 5px solid #f6b73c;
	margin: 0;
	padding-left: 10px;
}
 
/* 单行代码 */
.cnblogs-markdown code {
	font-family: Consolas, "Microsoft YaHei", monospace !important;
	font-size: 16px !important;
	line-height: 20px;
	background-color: #f5f5f5 !important;
	border: 1px solid #ccc !important;
	padding: 0 5px !important;
	border-radius: 3px !important;
	line-height: 1.8;
	margin: 1px 5px;
	vertical-align: middle;
	display: inline-block;
}
 
/* 多行代码, 引用 */
.cnblogs-markdown .hljs {
	font-family: Consolas, "Microsoft YaHei", monospace !important;
	font-size: 16px !important;
	line-height: 1.5 !important;
	padding: 5px !important;
}
```



## 在页面顶部添加"自定义搜索"功能



## 在页面顶部添加"音乐播放器"(Flash)

效果图: gif



## 在页面顶部添加"Fork me on Github"图标



## 为导航栏设置渐变背景色



## 在公告栏添加动态文字



## 在公告栏加入自己的社交网络账号 - 图片链接



## 在公告栏添加一个能旋转的rss图标



效果图: gif



## 在公共栏添加"小人时钟"(Flash)

```html
<embed wmode="transparent" src="https://files.cnblogs.com/files/enjoy233/honehone_clock_tr.swf" quality="high" bgcolor="#FDF6E3" width="200" height="120" name="honehoneclock" align="middle" allowscriptaccess="always"type="application/x-shockwave-flash" pluginspage="http://www.macromedia.com/go/getflashplayer">
```

效果图: gif



## 在公共栏添加"站点统计"功能



## 页面底部添加"回到顶部"功能



## 页面底部添加"收藏"功能



## 页面底部添加"快速评论"功能



## "自动移动的目录"功能

效果图: gif



## 改进评论的显示样式
改成了微信聊天的样式。




## 在公告栏添加"友情链接"
cnblogs博客后台提供了"链接"功能，这个就是用来添加友情链接的。



## "博客签名"功能

虽然cnblogs博客后台提供了"博客签名"功能，测试发现IE下不能用，只好改为用JQuery来实现了。

```html
<script type="text/javascript">
$(document).ready(function(){
	$("#cnblogs_post_body").append('<br/><hr/><div style="border: 2px dotted #4d90fe; padding: 2px; background-color: lightgray">    作者：<a href="http://www.cnblogs.com/enjoy233/" target="_blank" title="Enjoy233的博客" style="color: brown">Bravo Yeung</a><br>    出处：<a href="http://www.cnblogs.com/Enjoy233/" target="_blank" title="http://www.cnblogs.com/Enjoy233/" style="color: blue">http://www.cnblogs.com/Enjoy233/</a>    <br>如果您觉得阅读本文对您有帮助，请点击一下右下方的<b style="color: blue; font-size: 16px">推荐</b>按钮，您的<b style="color: blue; font-size: 16px">推荐</b>将是我写作的最大动力！    <br>版权声明：本文为博主原创或转载文章，欢迎转载，<b>但转载文章之后必须在文章页面明显位置注明出处</b>，否则保留追究法律责任的权利。</div>');
});
</script>
```

## 禁用页面的"选中复制"功能
```css
/* 禁止页面，选中 复制 */
html,body {
	moz-user-select: -moz-none;
	-moz-user-select: none;
	-o-user-select: none;
	-khtml-user-select: none;
	-webkit-user-select: none;
	-ms-user-select: none;
	user-select: none;
}
```

## 不显示底部广告

```css
#ad_t2,#cnblogs_c1,#under_post_news,#cnblogs_c2,#under_post_kb {
display:none; !important
}
```

