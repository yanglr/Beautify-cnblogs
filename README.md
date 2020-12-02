- [前端小白也能快速学会的博客园博客美化全攻略](#前端小白也能快速学会的博客园博客美化全攻略)
  * [美化方法论简介](#美化方法论简介)
  * [准备工作](#准备工作)
    + [js权限申请](#js权限申请)
  * [如何模仿一个博客园的自定义风格(样式css+动态效果js)?](#如何模仿一个博客园的自定义风格样式css动态效果js)
  * [markdown样式自定义](#markdown样式自定义)
  * [在页面顶部添加"自定义搜索"功能](#在页面顶部添加自定义搜索功能)
  * [在页面顶部添加"音乐播放器"(Flash)播放背景音乐](#在页面顶部添加音乐播放器Flash播放背景音乐)
  * [在页面顶部添加"Fork me on Github"图标](#在页面顶部添加fork-me-on-github图标)
  * [为导航栏设置渐变背景色](#为导航栏设置渐变背景色)
  * [在公告栏添加滚动文字](#在公告栏添加滚动文字)
  * [在公告栏加入自己的社交网络账号 - 图片链接](#在公告栏加入自己的社交网络账号---图片链接)
  * [在公告栏添加一个能旋转的rss图标](#在公告栏添加一个能旋转的rss图标)
  * [在公共栏添加"小人时钟"(Flash)](#在公共栏添加小人时钟(Flash))
  * [在公共栏添加"站点统计"功能](#在公共栏添加站点统计功能)
  * [在公告栏中加入"自定义搜索"(PopUp弹窗)](#在公告栏中加入自定义搜索PopUp弹窗)
  * [页面底部添加"回到顶部" + "收藏" + "快速评论"功能](#页面底部添加回到顶部--收藏--快速评论功能)
  * ["自动移动的目录"功能](#自动移动的目录功能)
  * [改进评论的显示样式](#改进评论的显示样式)
  * [在公告栏添加"友情链接"](#在公告栏添加友情链接)
  * ["博客签名"功能](#博客签名功能)
  * [禁用页面的"选中复制"功能](#禁用页面的选中复制功能)
  * [不显示底部广告](#不显示底部广告)
  * [修改导航栏(修改部分链接的文字 + 增加下拉菜单)](#修改导航栏修改部分链接的文字--增加下拉菜单)
  * [微博秀的嵌入(支持http/https访问)](#微博秀的嵌入支持httphttps访问)
  * [分享组件的嵌入(支持http/https访问)](#分享组件的嵌入支持httphttps访问)
  * [打赏功能](#打赏功能)
  * [复制文字时自动加版权](#复制文字时自动加版权)
  * [隐藏博文右下角的"反对"](#隐藏博文右下角的反对)

<br/>

欢迎访问作者的个人网站: [极客中心](https://www.geekzl.com)

# 前端小白也能快速学会的博客园博客美化全攻略

**<font size=6>A呦V，博客园er的自我修养是什么？第一条，别只顾收藏和偷师呀，记得点支持或关注本人喔~ </font>**

## 美化方法论简介

一般而言，需要选一个默认的skin，然后在该基础上调整。

官方介绍：
博客皮肤模板 <http://skintemplate.cnblogs.com/>



官方文档 - 【博客园skin开发文档 】:

<https://docs.qq.com/sheet/DZFJDeGVuRW5QRmJa>



宽屏模版：

SimpleMemory

Minyx2_Lite

lessIsMore

BlueSky
<br>


博客园布局的组成及其对应关系(下方一图来自于**网络**):
![common_skin_layout](https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_common-skin-layout.png)


## 准备工作

1. 首先你得有个cnblogs博客
2. 申请js权限

**附该美化过程的github项目:**
[yanglr/Beautify-cnblogs: Beautify-cnblogs](https://github.com/yanglr/Beautify-cnblogs)

欢迎fork或star~

本博客的所有代码在此github项目的`src`文件夹中~

**源码使用步骤：**

1. 打开 博客后台管理 → “设置”
2. 在博客皮肤选项卡中将博客皮肤设置为： `LessIsMore`
3. 将`src`文件夹下的页面定制.css 复制到 页面定制CSS代码 代码框内
4. 将同一文件夹下的 页首.html 复制到 页首Html代码 代码框内
5. 将同一文件夹下的 页尾.html 复制到 页脚Html代码 代码框内
6. 保存，即可见效。


### js权限申请

登陆后依次点击“我的博客” → “管理” → “设置”，在下拉后找到“博客侧边栏公告”，后方有一个“申请js权限”。

![Apply_js](https://raw.githubusercontent.com/yanglr/Beautify-cnblogs/master/images/Apply-js-with-Content.jpg)

或者也可进博客园园子页面(<https://home.cnblogs.com/feed/all/>)，发状态@博客园团队，申请开通js权限。

也可发个邮件到[contact@cnblogs.com](mailto:contact@cnblogs.com)申请js权限。



**申请时内容模板已为你备好:**

> 尊敬的博客园管理员：
>
> 本人请求申请开通js权限，希望能够把博客修饰的漂亮点，点缀自定义js插件效果，希望管理员可以批准，多谢~



提交完申请，会弹出提示:

`JS权限申请已提交，待审核。`

剩下的就是耐心等待了，一般来说挺快就会通过。如果设置页面上公告栏标题右侧不存在“申请js权限”，说明已成功开通js权限。



## 如何模仿一个博客园的自定义风格(样式css+动态效果js)?

模仿一个cnblogs的全局css，只需打开Chrome浏览器，按下F12，找里面的skin css和custom css，例如：

```css
<link id="MainCss" type="text/css" rel="stylesheet" href="/skins/LessIsMore/bundle-LessIsMore.css?...">

<link type="text/css" rel="stylesheet" href="/blog/customcss/198996.css?v=...">
```




补充完整前缀：<http://www.cnblogs.com>，使用ref将该两个css引用到自己的博客中，即可进行大概样子的模仿，其他部分需要细调。



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

css部分：
```css
<style type="text/css"> 
    #auto_div {
        display: none;
        width: 257px;
        border: 1px #74c0f9 solid;
        background: #FFF;
        position: absolute;
        top: 24px;
        left: 0;
        margin-top: 15px;
        color: #323232;
        /*设置显示在当前页面的上一层*/
        z-index: 1;
    }
 
    .side_search {
        float: left;
        position: relative;
        height: 31px;
        margin-left: 25px;
        display: inline-block;
    }
 
        .side_search:hover {
            -webkit-box-shadow: 0 0 3px #999;
            -moz-box-shadow: 0 0 3px #999
        }
 
    .search_input {
        width: 210px;
        vertical-align: middle;
        height: 30px;
        line-height: 30px;
        border: 1px solid #999;
        border-radius: 2px 0 0 2px;
        padding: 4px 7px;
        background-color: #fbfbfb;
    }
 
    .delete_btn {
        background: #fbfbfb;
        margin-left: -6px;
        border: 1px solid #fbfbfb;
        border-radius: 0 3px 3px 0;
        cursor: pointer;
        display: inline-block;
        vertical-align: middle;
        color: red;
        font-weight: bold;
        width: 38px;
        font-size: 25px;
        height: 38px;
        padding-bottom: inherit;
    }
 
    .search_btn {
        border-radius: 3px 3px 3px 3px;
        background: #4d90fe;
        margin-left: -7px;
        border: 1px solid #4d90fe;
        cursor: pointer;
        display: inline-block;
        vertical-align: middle;
        color: #f3f7fc;
        font-weight: bold;
        width: 100px;
        font-size: 18px;
        height: 41px;
    }
 
        .search_btn:hover {
            background: #1874CD
        }
 
    .search_btn2 {
        border-radius: 3px 3px 3px 3px;
        background: #F0CB85;
        border: 1px solid #F0CB85;
        cursor: pointer;
        display: inline-block;
        vertical-align: middle;
        color: #DC143C;
        font-weight: bold;
        width: 100px;
        font-size: 18px;
        height: 41px;
    }
 
        .search_btn2:hover {
            background: #DEB887
        }
 
    input, button, textarea, select, optgroup, option {
        font-family: inherit;
        font-size: inherit;
        font-style: inherit;
        font-weight: inherit;
    }
</style>
```

js部分:
```html
<script src="https://cdn.bootcss.com/jquery/3.2.1/jquery.min.js" type="text/javascript"></script>
<script type="text/javascript">
    var availableTags = [
        "C#", "C++", "算法",
        "ASP", "MySQL", "Oracle",
        "HTML", "CSS", "JavaScript",
        "jQuery", "AJAX", "微软系列技术",
        "Sublime", "Git",
        "Visual Studio Code",
        "Eclipse",
        "C#开发", "C++开发", "Java开发",
        "PHP开发",
        "Python开发",
        "Web前端开发",
        "Windows Forms",
        "WPF",
        "计算机数学",
        "浏览器插件",
        "软件推荐",
        "算法实践",
        "专业学习",
        "Leetcode",
        "知乎",
        "Bravo Yeung",
        "legege007",
        "enjoy233",
        "数学",
        "内容太长，显示其中的一部分"
    ];
    var old_value = "";
    var highlightindex = -1;   //高亮

    //自动完成
    function AutoComplete(auto, search, mylist) {
        if ($("#" + search).val() != old_value || old_value == "") {
            var autoNode = $("#" + auto);   //缓存对象（弹出框）
            var carlist = new Array();
            var n = 0;
            old_value = $("#" + search).val();
 
            for (i in mylist) {
                if (mylist[i].indexOf(old_value) >= 0) {
                    carlist[n++] = mylist[i];
                }
            }
            if (carlist.length == 0) {
                autoNode.hide();
                return;
            }
            autoNode.empty();  //清空上次的记录
            for (i in carlist) {
                var wordNode = carlist[i];   //弹出框里的每一条内容

                var newDivNode = $("<div>").attr("id", i);    //设置每个节点的id值
                newDivNode.attr("style", "font:14px/25px arial;height:25px;padding:0 8px;cursor: pointer;");
 
                newDivNode.html(wordNode).appendTo(autoNode);  //追加到弹出框

                //鼠标移入高亮，移开不高亮
                newDivNode.mouseover(function () {
                    if (highlightindex != -1) {        //原来高亮的节点要取消高亮（是-1就不需要了）
                        autoNode.children("div").eq(highlightindex).css("background-color", "white");
                    }
                    //记录新的高亮节点索引
                    highlightindex = $(this).attr("id");
                    $(this).css("background-color", "#ebebeb");
                });
                newDivNode.mouseout(function () {
                    $(this).css("background-color", "white");
                });
 
                //鼠标点击文字上屏
                newDivNode.click(function () {
                    //取出高亮节点的文本内容
                    var comText = autoNode.hide().children("div").eq(highlightindex).text();
                    highlightindex = -1;
                    //文本框中的内容变成高亮节点的内容
                    $("#" + search).val(comText);
                })
                if (carlist.length > 0) {    //如果返回值有内容就显示出来
                    autoNode.show();
                } else {               //服务器端无内容返回 那么隐藏弹出框
                    autoNode.hide();
                    //弹出框隐藏的同时，高亮节点索引值也变成-1
                    highlightindex = -1;
                }
            }
        }
 
        //点击页面隐藏自动补全提示框
        document.onclick = function (e) {
            var e = e ? e : window.event;
            var tar = e.srcElement || e.target;
            if (tar.id != search) {
                if ($("#" + auto).is(":visible")) {
                    $("#" + auto).css("display", "none")
                }
            }
        }
 
    }
 
    $(function () {
        old_value = $("#zzk_q").val();

        $("#zzk_q").keyup(function () {
            AutoComplete("auto_div", "zzk_q", availableTags);
        });
    });
 
    function quickdelete() {
        document.getElementById("zzk_q").value = "";
    }
 
    function zzk_go() {
        var n = encodeURIComponent(document.getElementById("zzk_q").value);
        window.location = "http://zzk.cnblogs.com/s?w=blog%3AEnjoy233+" + n + "&t="
    }
    function zzk_go2() {
        var n = encodeURIComponent(document.getElementById("zzk_q").value);
        window.location = "http://zzk.cnblogs.com/s?w=" + n
    }
    function zzk_go_enter(n) {
        if (n.keyCode == 13)
            return zzk_go(), !1
    }
</script>
```
如果需要修改自动完成的下拉选项，修改变量`availableTags`的值即可见效。


html部分：

```html
<h1 style="margin-left: 570px;padding-top:15px;padding-bottom: 15px; color: #337ab7;font-size: 3em;font-weight: bold;font-style: italic;text-shadow: 1px 0px 0px #1E90FF;">  </h1>
<div class="side_search">
    <input type="text" id="zzk_q" class="search_input" onkeydown="return zzk_go_enter(event);" placeholder="输入 回车搜索" tabindex="1" autofocus x-webkit-speech>
    <div id="auto_div">
    </div>&nbsp;
    <input onclick="quickdelete()" type="button" class="delete_btn" value="×" title="清空">
    <input onclick="zzk_go()" type="button" class="search_btn" value="本博搜索">
    <input onclick="zzk_go2()" type="button" class="search_btn2" value="园内搜索">
</div>
```



效果图:

![customSearch1](https://files.cnblogs.com/files/enjoy233/customSearch1.bmp)



## 在页面顶部添加"音乐播放器"(Flash)播放背景音乐

先登录网易云音乐网页版，搜索到想要的音乐，然后点击"生成外链播放器"即可得到相应的html代码。

![163music_palyer](https://raw.githubusercontent.com/yanglr/Beautify-cnblogs/master/images/163music_player.bmp)



**表现形式一：单曲播放** (type = 1)

```html
<embed src="http://music.163.com/outchain/player?type=0&amp;id=26237342&amp;auto=0&amp;height=430" width="100%" height="450" frameborder="no" marginwidth="0" marginheight="0"></embed> 
```

或

```html
<embed src="https://music.163.com/style/swf/widget.swf?sid=26237342&type=2&auto=0&width=320&height=66" width="340" height="86"  allowNetworking="all" ></embed>
```

参数说明：

> 播放器可修改参数：
> width=100% #自适应宽度, 本博客使用了固定宽度320
> height=66 #根据自己需要来改
> sid=26237342 # 此数字是歌曲的ID http://music.163.com/#/song?id=26237342
> auto=0 # 0表示不自动播放，1表示自动播放



**表现形式二：列表播放** (type = 0)

```html
<embed src="https://music.163.com/outchain/player?type=0&amp;id=78413764&amp;auto=0&amp;height=430" width="100%" height="450" frameborder="no" marginwidth="0" marginheight="0"></embed> 
```

当然该`url`中的`https:`也可删掉。

![playList](https://raw.githubusercontent.com/yanglr/Beautify-cnblogs/master/images/163playList.bmp)



参数说明

> 播放器可修改参数：
> width=100% # 自适应宽度
> height=450 # 根据自己的需要修改
> id=34238509 # 此数字是歌曲列表页的ID, 例如：http://music.163.com/#/playlist?id=34238509
> auto=0  # 0表示不自动播放，1表示自动播放




将该代码贴进页首html即可见效(如果代码中含有`iframe`，需替换成`embed`)~

```html
<div style="display: table; text-align: center; width: 40%; height: 100%;">
<embed src="https://music.163.com/style/swf/widget.swf?sid=26237342&type=2&auto=0&width=320&height=66" width="340" height="86"  allowNetworking="all" ></embed>
</div>
```



效果图: 

![163music_player](https://files.cnblogs.com/files/enjoy233/163music_player.gif)





## 在页面顶部添加"Fork me on Github"图标

页首html需要添加
```html
<div>
<a href="http://github.com/yanglr" target="_blank" style="position: absolute;right: 0;  top: 0; z-index: 100;">
    <img src="http://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_git-right-link.gif" alt="Fork me on github">
</a>
</div>
```

效果见[本页面](https://www.cnblogs.com/enjoy233/p/10328361.html)右上角。



如果想对该图标进行更多颜色或位置的设置，请参考：[GitHub Ribbons - The GitHub Blog](https://github.blog/2008-12-19-github-ribbons/).



## 为导航栏设置渐变背景色

```css
/* 头部 */
#header {
	position: relative;
	height: 280px;
	margin: 0;
	background: #020031;
	background: -moz-linear-gradient(45deg,#020031 0,#6d3353 100%);
	background: -webkit-gradient(linear,left bottom,right top,color-stop(0%,#020031),color-stop(100%,#6d3353));
	background: -webkit-linear-gradient(45deg,#020031 0,#6d3353 100%);
	background: -o-linear-gradient(45deg,#020031 0,#6d3353 100%);
	background: -ms-linear-gradient(45deg,#020031 0,#6d3353 100%);
	background: linear-gradient(45deg,#020031 0,#6d3353 100%);
	filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#020031', endColorstr='#6d3353', GradientType=1);
	-webkit-box-shadow: inset 0 3px 7px rgba(0,0,0,.2),inset 0 -3px 7px rgba(0,0,0,.2);
	-moz-box-shadow: inset 0 3px 7px rgba(0,0,0,.2),inset 0 -3px 7px rgba(0,0,0,.2);
	box-shadow: inset 0 3px 7px rgba(0,0,0,.2),inset 0 -3px 7px rgba(0,0,0,.2);
}
```



## 在公告栏添加滚动文字

使用`marquee`标签即能实现文字的滚动 

```html
<marquee><a href="#"><font color="blue" size="4">You will make it!
</marquee>
```

效果图:

![slide_words](https://files.cnblogs.com/files/enjoy233/slide_words.gif)




## 在公告栏加入自己的社交网络账号 - 图片链接

可以将自己不同社交网络的账号放在同一个span中，然后嵌入到div里，代码如下：
```html
    <div nowrap align=center>
        <img src="http://images.cnblogs.com/cnblogs_com/enjoy233/1389971/o_gzh.png" width=150 height=150>
    </div>
<br>
<div align="center">
     <a href="http://stackoverflow.com/users/6075331/bravo-young" target="_blank" class="mr5 "><strong>StackOverflow</strong></a><font  style="color:#BF7158">(</font>
    <img src="http://images.cnblogs.com/cnblogs_com/enjoy233/1389971/o_reputation-rp.png" class="mr5">
    <span style="color:#BF7158" class="mr10">406 <font size=4 color=black>⬆</font>)</span>
</div>

<br>

<div class="c-social" align="center">
<span>
    <a href="https://github.com/yanglr" target="_blank">
      <img src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_github.png" class="mr5" width = 40 height=40>
    </a>
    <a href="http://blog.csdn.net/lzuacm" target="_blank">
      <img src="http://images.cnblogs.com/cnblogs_com/enjoy233/1389971/o_csdn.png" class="mr5" width = 40 height=40>
    </a>
    <a href="https://www.zhihu.com/people/legege007" target="_blank">
      <img src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_zhihu.png" class="mr5" width = 40 height=40>
    </a>
    <a href="http://weibo.com/546671991" target="_blank">
      <img src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_weibo.png" class="mr5" width = 40 height=40>
    </a>

</span>
```
效果图:

![socialLinks](https://files.cnblogs.com/files/enjoy233/socialLinks.gif)

对于知乎，可以这样写更详细些：
```html
<div valign="middle" align="left" bgcolor='#F6F8FA'>
    <span>
        <a href="https://www.zhihu.com/people/legege007" title="知乎撩我" target="_blank">
            <img src="http://images.cnblogs.com/cnblogs_com/enjoy233/1389971/o_zhihu-dog.jpg" height='22'>
        </a>
    </span>
    <span valign='middle'>
        <font>(</font>
        <img src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_vote.png" width='14' height='14' title="赞同">
        42.8k <font color=black></font>
        <img src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_fav.png" width='14' height='14' title="收藏">
        90.7k <font  color=black></font>
        <img src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_thank.png" width='14' height='14' title="感谢">
        21.7k <font color=black></font>)
    </span>
</div>
```
而对于stackoverflow，官方在StackExchange页面提供了flair，比如我的是: [User Bravo Yeung - Stack Exchange](https://stackexchange.com/users/4637854/bravo-yeung?tab=flair) ，页面中提供了可嵌入的html代码:

```html
<a href="https://stackexchange.com/users/4637854/bravo-yeung"><img src="https://stackexchange.com/users/flair/4637854.png" width="208" height="58" alt="profile for Bravo Yeung on Stack Exchange, a network of free, community-driven Q&amp;A sites" title="profile for Bravo Yeung on Stack Exchange, a network of free, community-driven Q&amp;A sites" /></a>
```
将其用div包起来，放进公告.html即可见效。


## 在公告栏添加一个能旋转的rss图标

先将相应的css放入页面定制css或公告栏的css中，然后在后面使用。
```css
#feed_icon {
	border: #000 solid 2px;
	display: block;
	margin: 50px auto;
	border-radius: 50%;
	transition: all 2.0s;
}

#feed_icon:hover {
	transform: rotate(360deg);
}
```

然后将如下代码贴进公告中~
```html
<div id="feed">
  <a href="https://www.cnblogs.com/enjoy233/rss" title="订阅Feed"  target="_blank">
     <img id="feed_icon" src="https://www.cnblogs.com/images/cnblogs_com/enjoy233/1389971/o_rss.png" alt="" style="border: 0pt none;" width = 60 height=60>
  </a>
</div>
```



效果图:

![rss_roate](https://files.cnblogs.com/files/enjoy233/rss_rotate.gif)



## 在公共栏添加"小人时钟"(Flash)

```html
<embed wmode="transparent" src="https://files.cnblogs.com/files/enjoy233/honehone_clock_tr.swf" quality="high" bgcolor="#FDF6E3" width="200" height="120" name="honehoneclock" align="middle" allowscriptaccess="always"type="application/x-shockwave-flash" pluginspage="http://www.macromedia.com/go/getflashplayer">
```



效果图: 

![clock_result](https://files.cnblogs.com/files/enjoy233/clock_run.gif)



## 在公共栏添加"站点统计"功能
打开网站：http://www.flagcounter.com/ ，无需注册，点击黄色按钮"Get Your Flag Counter"，即可生成嵌入该插件的html代码。
![FlagCounter](http://images.cnblogs.com/cnblogs_com/enjoy233/1389971/o_flagCounter.png)

生成的html代码如下：
```html
<div>
<a href="https://info.flagcounter.com/LCgi"><img src="https://s04.flagcounter.com/count2/LCgi/bg_FFFFFF/txt_000000/border_CCCCCC/columns_2/maxflags_10/viewers_0/labels_1/pageviews_1/flags_0/percent_0/" alt="Flag Counter" border="0"></a>
<div>
```
最后将该代码加入到公告栏的html代码中即能生效。



## 在公告栏中加入"自定义搜索"(PopUp弹窗)

**实现的基本原理:**

> onclick = "window.open()", target = popUpWindow

此功能的特色在于用户搜索之后，搜索结果页面并不会影响到原博客页面，而是在弹出的独立窗口显示，而且很容易扩展出很多其他站点的搜索功能。

在公告html中贴入如下代码:

```html
<div id="sidebar_search_new" class="mySearch">
<h3 class="catListTitle">自定义搜索(PopUp窗口)</h3>
    <input type="text" id="zzk_q1" class="input_my_zzk_new" placeholder="Bravo Yeung"> 
<span>
    <input type="button" class="btn_my_zzk" value="本博搜索" onclick="window.open('https://zzk.cnblogs.com/my/s/blogpost-p?Keywords=' + document.getElementById('zzk_q1').value,'popUpWindow','height=750,width=1000,left=10,top=10,scrollbars=yes,menubar=no'); return false;" />
&emsp;
<input type="button" class="btn_my_zzk" value="站内搜索" onclick="window.open('https://zzk.cnblogs.com/s/blogpost?w=' + document.getElementById('zzk_q1').value,'popUpWindow','height=750,width=1000,left=10,top=10,scrollbars=yes,menubar=no'); return false;" />
</div>
<span>
<span>
    <input type="button" class="btn_my_zzk" value="知乎搜索" onclick="window.open('https://www.zhihu.com/search?type=content&q=' + document.getElementById('zzk_q1').value,'popUpWindow','height=750,width=1000,left=10,top=10,scrollbars=yes,menubar=no'); return false;" />
&emsp;
<input type="button" class="btn_my_zzk" value="CSDN搜索" onclick="window.open('https://so.csdn.net/so/search/s.do?t=blog&u=yanglr2010&q=' + document.getElementById('zzk_q1').value,'popUpWindow','height=750,width=1000,left=10,top=10,scrollbars=yes,menubar=no'); return false;" />
</div>
```



效果图:

![customSearch2](https://raw.githubusercontent.com/yanglr/Beautify-cnblogs/master/images/custom_search2.bmp)





## 页面底部添加"回到顶部" + "收藏" + "快速评论"功能

html部分：

```css
<div class="scrollBtn" id="scrollBtn">
    <ul class="clearfix">
        <li class="sB-home">
            <a href="http://www.cnblogs.com/enjoy233" class="ff-t" title="首页"></a>
        </li>
        <li class="sB-comment">
            <a href="#blog-comments-placeholder" onclick="$('#tbCommentBody').focus();" class="ff-t" title="添加评论"></a>
        </li>
        <li class="sB-share"><a onclick="if(cb_entryId !=undefined){AddToWz(cb_entryId)}" href="javascript:void(0);" title="收藏"></a></li>
        <li class="sB-goTop" id="goTop" style="display: list-item;">
            <a href="#top" title="回顶部"></a>
        </li>
    </ul>
</div>
```

效果图:

![custom_Tool_Bar](https://files.cnblogs.com/files/enjoy233/CustomtoolBar.gif)

## "自动移动的目录"功能

页脚html引入css文件nav.my.css和nav.my.js。

```html
<link href="//blog-static.cnblogs.com/files/enjoy233/nav.my.css" rel="stylesheet">
<script type="text/javascript" src="//files.cnblogs.com/files/enjoy233/nav.my.js"></script>
```

然后将下方代码贴进页脚html.

JS部分:

```html
<script language="javascript" type="text/javascript">
//生成目录索引列表
function GenerateContentList()
{
    var jquery_h3_list = $('#cnblogs_post_body h4');//如果你的章节标题不是h4,只需要将这里的h4换掉即可
    if(jquery_h3_list.length>0)
    {
        var content = '<a name="_labelTop"></a>';
        content    += '<div id="navCategory">';
        content    += '<p style="font-size:18px"><b>阅读目录</b></p>';
        content    += '<ul>';
        for(var i =0;i<jquery_h3_list.length;i++)
        {
            var go_to_top = '<div style="text-align: right"><a href="#_labelTop">回到顶部</a><a name="_label' + i + '"></a></div>';
            $(jquery_h3_list[i]).before(go_to_top);
            var li_content = '<li><a href="#_label' + i + '">' + $(jquery_h3_list[i]).text() + '</a></li>';
            content += li_content;
        }
        content    += '</ul>';
        content    += '</div>';
        if($('#cnblogs_post_body').length != 0 )
        {
            $($('#cnblogs_post_body')[0]).prepend(content);
        }
    }    
}
GenerateContentList();
</script>

```



效果图: 

![autoMoveContents](https://files.cnblogs.com/files/enjoy233/autoMoveContents.gif)



## 改进评论的显示样式
这里我索性改成了熟悉的微信聊天的样式。




纯css实现:

```css
    .blog_comment_body {
        background: #B2E866;
        float: left;
        border-radius: 5px;
        position: relative;
        overflow: visible;
        margin-left: 33px;
        max-width: 700px;
    }

    .feedbackListSubtitle a.layer {
        background: #B2E866;
        color: #414141 !important;
        padding: 2px 4px;
        border-radius: 2px;
    }
```

将上面的代码贴紧页面css文本框即可见效果。



**效果图:**

![custom_comments](https://files.cnblogs.com/files/enjoy233/custom_comments.bmp)




## 在公告栏添加"友情链接"
cnblogs博客后台提供了"链接"功能，这个就是用来添加友情链接的。



**设置方法(见下图):**

编辑分类 -> 添加链接，设置好后公告栏上会显示相关内容，不过可能会有延时，需要等一会。


![friend_links](https://files.cnblogs.com/files/enjoy233/cnblogs-Link.bmp)



效果图:

![friend_link_result](https://files.cnblogs.com/files/enjoy233/friendLink.bmp)



## "博客签名"功能

虽然cnblogs博客后台提供了"博客签名"功能，测试发现该该方法实现的博客签名在IE中打开时不显示，只好改为用跨浏览器的JQuery来实现了。

```html
<script type="text/javascript">
$(document).ready(function(){
	$("#cnblogs_post_body").append('<br/><hr/><div style="border: 2px dotted #4d90fe; padding: 2px; background-color: lightgray">    作者：<a href="http://www.cnblogs.com/enjoy233/" target="_blank" title="Enjoy233的博客" style="color: brown">Bravo Yeung</a><br>    出处：<a href="http://www.cnblogs.com/Enjoy233/" target="_blank" title="http://www.cnblogs.com/Enjoy233/" style="color: blue">http://www.cnblogs.com/Enjoy233/</a>    <br>如果您觉得阅读本文对您有帮助，请点击一下右下方的<b style="color: blue; font-size: 16px">推荐</b>按钮，您的<b style="color: blue; font-size: 16px">推荐</b>将是我写作的最大动力！    <br>版权声明：本文为博主原创或转载文章，欢迎转载，<b>但转载文章之后必须在文章页面明显位置注明出处</b>，否则保留追究法律责任的权利。</div>');
});
</script>
```



## 禁用页面的"选中复制"功能

在css中进行相应的设置，只需将下方代码贴入"页面css"文本框即可。

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

综合考虑后，这种处理方式并不太友好，于是采用了后文中的"复制博客内容时自动加版权说明"。



## 不显示底部广告

在css中进行相应的设置，只需将下方代码贴入"页面css"文本框即可。

```css
#ad_t2,#cnblogs_c1,#under_post_news,#cnblogs_c2,#under_post_kb {
    display:none; !important
}
```



## 修改导航栏(修改部分链接的文字 + 增加下拉菜单)

css部分:
```css
/* 定制自己导航栏的样式 */
#shwtop ul {
    margin: 0;
    padding: 0;
    list-style-type: none; /*去除li前的标注*/
    background-color: #333;
    overflow: hidden; /*隐藏溢出的部分，保持一行*/
}
#shwtop li {
    float: left; /*左浮动*/
}
#shwtop li a, .dropbtn {
    display: inline-block; /*设置成块*/
    color: white;
    text-align: center;
    text-decoration: none;
    padding: 14px 16px;
}
/*鼠标移上去，改变背景颜色*/
#shwtop li a:hover, .dropdown:hover .dropbtn { 
    /* 当然颜色你可以自己改成自己喜欢的，我还是挺喜欢蓝色的 */
    background-color: blue;
}
#shwtop .dropdown {
    /*
    display:inline-block将对象呈递为内联对象，
    但是对象的内容作为块对象呈递。
    旁边的内联对象会被呈递在同一行内，允许空格。
    */
    display: inline-block;
}
#shwtop .dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
}
#shwtop .dropdown-content a {
    display: block;
    color: black;
    padding: 8px 10px;
    text-decoration:none;
}
#shwtop .dropdown-content a:hover {
    background-color: #a1a1a1;
}
#shwtop .dropdown:hover .dropdown-content{
    display: block;
}
```



页脚html部分：

```html
<!-- 更新导航栏的菜单-->
<script>
    $(function(){
            $("#navigator").append('<div id="shwtop" >    <ul style="margin-left:5px;margin-right: 5px;">       <div class="dropdown">            <a href="#" class="dropbtn">后台管理</a>            <div class="dropdown-content">                <!-- <a class="menu" href="这里是你文章或随笔分类的链接地址，自己修改下面同理"> 这里更改下拉具体内容 </a> -->                <a class="menu" href="http://i.cnblogs.com/Configure.aspx"  target="_blank">GUI配置</a>                <a class="menu" href="http://i.cnblogs.com/posts" target="_blank">博文列表</a>                <a class="menu" href="http://wz.cnblogs.com/" target="_blank">收藏</a>                               <a class="menu" href="http://i.cnblogs.com/Files.aspx" target="_blank">文件</a>   <a class="menu" href="https://i.cnblogs.com/EditGalleries.aspx" target="_blank">相册</a>          </div>        </div>    </ul></div>');

        $("#navList").append('<li id="nav_home"><a id="enjoy233" rel="nofollow" href="https://ing.cnblogs.com/" target="_blank" title="进入我的闪存">闪存</a></li>');
        $("#navList").append('<li id="nav_follow"><a id="enjoy233" rel="nofollow" href="http://home.cnblogs.com/followees/" target="_blank" title="进入我的关注">我关注</a></li>');          

        $('#navList')[0].children["nav_contact"].innerHTML='<a id="nav_contact" class="menu" rel="nofollow" href="https://msg.cnblogs.com/send/Enjoy233">私信</a>';
        $('#navList')[0].children["nav_rss"].innerHTML='<a id="nav_rss" class="menu" rel="nofollow" href="https://www.cnblogs.com/enjoy233/rss">RSS订阅</a>';

            //加载图片
            var ponum1 = $(".postTitle").length;
            var ponum2 = $(".entrylistPosttitle").length;
            if(ponum1!=0)
                articleimg(ponum1);
            if(ponum2!=0)
                entrylistarticleimg(ponum2);
        });
</script>
```


效果图:

![custom-nav](https://raw.githubusercontent.com/yanglr/Beautify-cnblogs/master/images/custom-navigate.bmp)

如需调整请自行修改~



## 微博秀的嵌入(支持http/https访问)

参看本人的另一篇文章 [当今最全面可用的微博分享组件嵌入方法(亲测2019年2月仍有效) - Enjoy233](https://www.cnblogs.com/enjoy233/p/10349500.html) 即可。



效果图(见本博客左侧公告栏):

![weibo_show](https://files.cnblogs.com/files/enjoy233/weibo_show.gif)



## 分享组件的嵌入(支持http/https访问)

由于官方的 [Baidu Share](bdimg.share.baidu.com/static/) 的ssl证书已过期，只好找到一个替代镜像 `//static.dmzj.com/baidushare/static/js/shell_v2.js`，使得通过https访问或http访问本博客都可以看到左下角的分享按钮~




在页脚.html中加入如下代码:

```html
<!-- Baidu Share BEGIN -->
<div id="bdshare" class="bdshare_t bds_tools get-codes-bdshare"> 
<span class="bds_more">分享到：</span> 
<a href="#" class="bds_tsina" data-cmd="tsina" title="分享到新浪微博"></a>
<a href="#" class="bds_qzone" data-cmd="qzone" title="分享到QQ空间"></a>
<a href="#" class="bds_sqq" data-cmd="sqq" title="分享到QQ好友"></a>
<a href="#" class="bds_douban" data-cmd="douban" title="分享到豆瓣网"></a>
<a href="#" class="bds_youdao" data-cmd="youdao" title="分享到有道云笔记"></a>
<a href="#" class="bds_renren" data-cmd="renren" title="分享到人人网"></a>
<a href="#" class="bds_kaixin001" data-cmd="kaixin001" title="分享到开心网"></a>
<a href="#" class="bds_mail" data-cmd="mail" title="分享到邮件分享"></a>
</div> 
<script type="text/javascript" id="bdshare_js" data="type=tools&amp;uid=2883522" ></script> 
<script type="text/javascript" id="bdshell_js"></script> 
<script type="text/javascript"> 
document.getElementById("bdshell_js").src = "//static.dmzj.com/baidushare/static/js/shell_v2.js?cdnversion=" + Math.ceil(new Date()/3600000) 
</script> 
<!-- Baidu Share END -->
```



官方demo:

[分享按钮-百度分享](http://share.baidu.com/code) (获取代码 -> 按向导操作，可查看网页侧边的动态使用效果，也可看到相应代码。)



效果图:

![baiduShare](https://files.cnblogs.com/files/enjoy233/BaiduShareTool.gif)



## 打赏功能

本博客基于开源插件 [tctip](<https://github.com/greedying/tctip>) v1.0.3 来实现~

在页脚.html中插入如下代码即可:

```html
<!-- tctip 支付赞赏/打赏 -->
<script type="text/javascript" src="//files.cnblogs.com/files/enjoy233/tctip-1.0.3.min.js"></script> <!-- js文件引入 -->
<script>
    new tctip({
        top: '20%',
        button: {
            id: 1,
            type: 'zanzhu',
        },
        list: [
            {
                type: 'alipay',
                qrImg: 'https://files.cnblogs.com/files/enjoy233/Reward_Alipay_Charge.bmp' //替换成自己的支付宝付款码
            }, {
                type: 'wechat',
                qrImg: 'https://files.cnblogs.com/files/enjoy233/Reward_WX_Charge.bmp' //替换成自己的微信付款码
            }
        ]
    }).init()
</script>
```



效果图:

![custom-nav](https://files.cnblogs.com/files/enjoy233/reward.gif)

还看到过一个不错的方法，亲测有效：[自制简易打赏功能 - EritPang](https://www.cnblogs.com/eritpang/p/7465484.html) .




## 复制文字时自动加版权

确保页面能成功引入JQuery.js后在页首html中加入如下代码:
```html
<script language="javascript" type="text/javascript">
jQuery(document).on('copy', function(e)
{
  var selected = window.getSelection();
  var copyFooter = '<br>---------------------<br>著作权归作者所有。<br>' 
                        + '商业转载请联系作者获得授权，非商业转载请注明出处。<br>'
                        + '作者：Bravo Yeung<br> 源地址：' + document.location.href
                        + '<br>来源：博客园cnblogs<br>© 版权声明：本文为博主原创文章，转载请附上博文链接！';
  var copyHolder = $('<div>', {html: selected + copyFooter, style: {position: 'absolute', left: '-99999px'}});

  $('body').append(copyHolder);
  selected.selectAllChildren( copyHolder[0] );
  window.setTimeout(function() {
      copyHolder.remove();
  },0);
});
</script>
```

当用户复制文中内容(ctrl+C或鼠标右击复制)时，会自动加上版权文字，csdn的代码复制功能以及知乎的内容复制都有此功能。



**效果图:**

![copy-With-Copyright](https://raw.githubusercontent.com/yanglr/Beautify-cnblogs/master/images/copyWithCopyright.bmp)



##  隐藏博文右下角的"反对"按钮

只需在页面的css(设置下的第一个文本框)中加入如下代码:

```css
.buryit {
	display: none;
}

.comment_bury {
	display: none;
}
```
效果请见[本页面](https://www.cnblogs.com/enjoy233/p/10328361.html)右下角。
