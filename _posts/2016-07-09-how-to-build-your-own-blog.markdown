---
layout:     post
title:      "how to bulid your own blog"
subtitle:   "通过github搭建博客"
date:       2016-07-09 12:00:00
author:     "Wang Dandi"
header-img: "img/post-bg-07.jpg"
---


<blockquote>几天的小学期经历让我们对于撘网站从不会成长为会那么一点点，老师给的的教程以及网上的教程都有或多或少的坑，让我们开启一篇新的也许没那么坑的教程贴吧。</blockquote>

<h2>1.注册Github账号</h2>

<h1>既然本次采用的是将个人博客部署到github上，第一步当然是到<a href="https://github.com" alt="https://github.com" >github官方网站</a>注册账号，一定要牢记自己的用户名哟。如果你已经有账号和密码，那么点击右上角的sign in 直接登录，如果没有可以按照以下步骤进行注册。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build1.jpg" alt="Post Build Image">
</a>

<h1>按要求填写用户名、注册邮箱和密码：</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build2.jpg" alt="Post Build Image">
</a>

<h1>用户名一栏，每次在你输入昵称之后，都会检查是否已经被注册。如果被注册了，那么会提示Username is already taken。此时请换另一个昵称进行注册。此外，用户名中只能出现字母、数字、短横线（-）。并且短横线不能打头。所以中文是不合法昵称。而_abcd也不合法，因为短横线在开头。</h1>

<h1>邮箱邮箱要填写合法邮箱，并且是未在github注册过的邮箱。否则会弹出错误提示。</h1>

<h1>至于密码，密码至少有7个字符，其中至少有一个小写字母，至少有一个是数字，且不能使用中文。</h1>

<h1>在三个输入框中的信息都合法之后，它们右边会出现绿色小箭头。此时点击最下方的绿色大按钮来开始注册。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build3.jpg" alt="Post Build Image">
</a>

<h1>这时会弹出一个界面，让你选择你的私人计划（personal plan），即选择免费用户还是付费用户。付费用户可以拥有私人代码仓库（repos），即别人不能查看你的代码。免费用户的仓库都是公开的，任何人都能查看。这里我们选择免费用户就可以了。默认的FREE后面Chosen按钮已经是选中状态了。如果你想成为付费用户，那么点击上面的Chosen按钮。第二个红箭头前面的单选框是可选的，打不打勾都可以，最后我们点击右下角的绿色按钮Finish sign up来完成注册。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build4.jpg" alt="Post Build Image">
</a>

<a href="#">
    <img src="{{ site.baseurl }}/img/build5.jpg" alt="Post Build Image">
</a>

<h2>2.建立Guithub Page页面</h2>

<h3>2.1 安装git工具 </h3>

<h1><a href="https://windows.github.com" alt="https://windows.github.com" >https://windows.github.com</a></h1>

<h1><a href="https://mac.github.com" alt="https://mac.github.com" >https://mac.github.com</a></h1>

<h1><a href="https://git-for-windows.github.com" alt="https://windows.github.com" >https://git-for-windows.github.com</a></h1>

<h3>2.2 创建步骤 </h3>

<h1>安装好相应软件之后，在开始菜单中找到Git Bash并打开，在打开的窗口（shll）内执行以下命令，设置你的git用户名和邮箱：</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build6.jpg" alt="Post Build Image">
</a>

<h1>为了和Github的远程仓库进行传输，需要进行SSH加密设置。在刚才打开的Shell内执行如下：</p>

<a href="#">
    <img src="{{ site.baseurl }}/img/build7.jpg" alt="Post Build Image">
</a>

<h1>可以不输入其他信息，一直敲回车直到命令完成。 这时你的用户目录（win7以上系统默认在 C:\Users\你的计算机用户名）内会出现名为 .ssh 的文件夹，点进去能看到 id_rsa 和 id_rsa.pub 两个文件，其中 id_rsa 是私钥，不能让怪人拿走， id_rsa.pub 是公钥，无需保密。</h1>

<h1>接下来用你的浏览器登录Github，点击右上角的“Settings”，用文字处理软件打开刚才的 id_rsa.pub 文件，复制全部内容。点击“SSH Keys”，“Add SSH Key”，任意取名之后，将复制的内容粘贴在Key中，点“Add Key”确定，SSH配置完毕。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build8.jpg" alt="Post Build Image">
</a>

<a href="#">
    <img src="{{ site.baseurl }}/img/build9.jpg" alt="Post Build Image">
</a>









<p>顿顿不开心</p>

<iframe height=498 width=510 src="http://player.youku.com/embed/XMTYzMzA1MTczMg==" frameborder=0 allowfullscreen></iframe>

<p>你想知道原因吗，就不告诉你.</p>

<video id="my_video_1" class="video-js vjs-default-skin" controls    preload="auto"width="640"height="480"poster="video-js/my_video_poster.png"    data-setup="{}">
	<source src="{{ site.baseurl }}/text.mp4" type='video/mp4'> 
</video>


<script>
 if (navigator.userAgent.indexOf('Opera') >= 0){
    document.getElementById("videoDiv").innerHTML='<embed src="{{ site.baseurl }}/text.mp4" autostart="true" loop="true" width="640" height="480" >';
    }
</script>
 
<script>
    if (navigator.userAgent.indexOf('MSIE') >= 0){
		document.getElementById("videoDiv").innerHTML='<embed src="{{ site.baseurl }}/text.mp4" autostart="true" loop="true" width="640" height="480" >';
    }
</script>