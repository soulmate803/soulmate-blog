---
layout:     post
title:      "how to bulid your own blog"
subtitle:   "通过github搭建个人主页"
date:       2016-07-09 12:00:00
author:     "Wang Dandi"
header-img: "img/post-bg-07.jpg"
---


<blockquote>几天的小学期经历让我们对于撘网站从不会成长为会那么一点点，老师给的的教程以及网上的教程都有或多或少的坑，让我们开启一篇新的也许没那么坑的教程贴吧。</blockquote>

<h2>1.注册Github账号</h2>

<h1>既然本次采用的是将个人主页部署到github上，第一步当然是到<a href="https://github.com" alt="https://github.com" >github官方网站</a>注册账号，一定要牢记自己的用户名哟。如果你已经有账号和密码，那么点击右上角的sign in 直接登录，如果没有可以按照以下步骤进行注册。</h1>

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

<a href="#">
    <img src="{{ site.baseurl }}/img/build10.jpg" alt="Post Build Image">
</a>

<h2>3.建立Github Page页</h2>

<blockquote>可通过直接从别人的github页面中fork需要的jekyll模板，但此方法较为简单，不利于本次学习html语言的初衷及目的，因而不采用此方法。以下教程为将下载的bootstrap框架部署至github上的具体相关操作，尽量写的简单明了。</blockquote>

<h3>3.1 建立本地页面</h3>

<h1>建立本地页面可以上网下载Bootstrap框架，挑选自己喜欢的网站下载至本地，可用eclipse修改。新建Dynamic Web Project，配置服务器，将下载的框架文件夹添加至WebContent中。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build11.jpg" alt="Post Build Image">
</a>

<a href="#">
    <img src="{{ site.baseurl }}/img/build12.jpg" alt="Post Build Image">
</a>

<h1>打开文件，进行修改，直至获得自己想要的结果，可通过运行index.html页面查看本地效果。至此，本地页面搭建成功。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build13.jpg" alt="Post Build Image">
</a>

<h3>3.2 创建本地版本库</h3>

<h1>在本地创建一个名为username.github.io的空文件夹，在shell中进入该文件，输入git init，在文件夹中生成.git文件，并将之前修改后的本地页面相应文件添加其中，创建本地版本库。</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build14.jpg" alt="Post Build Image">
</a>

<h1>上述步骤只是将文件添加到相应的文件夹中，并未添加到仓库，可通过以下操作来将其放入git 仓库：</h1>

<h1>$ git add .</h1>
<h1>$ git commit -m "wdd"</h1>

<h1>简单解释一下git commit命令，-m后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录。git commit命令执行成功后会告诉你gitc仓库里哪些文件被修改。</h1>


<h3>3.3 同步至远程仓库 </h3>

<h1>在本地创建Git仓库之后，可在Github上也创建一个Git仓库，实现部署。首先，登陆GitHub，然后，在右上角找到“Create a new repo”按钮，创建一个新的仓库:</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build15.jpg" alt="Post Build Image">
</a>

<h1>如上图所示，在Repository name中填写username.gitub.io，创建新的远程库。添加远程库。目前，在GitHub上的这个learngit仓库还是空的，GitHub告诉我们，可以从这个仓库克隆出新的仓库，也可以把一个已有的本地仓库与之关联，然后，把本地仓库的内容推送到GitHub仓库。现在，在本地的username.github.io仓库下运行命令：</h1>

<h1>$ git remote add origin git@github.com:username/username.github.io.git</h1>

<h1>请千万注意，把上面的username替换成你自己的GitHub账户名，否则，以后的推送将不能成功。添加后，远程库的名字就是origin，这是Git默认的叫法，也可以改成别的，但是origin这个名字一看就知道是远程库。下一步，就可以把本地库的所有内容推送到远程库上：</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build16.jpg" alt="Post Build Image">
</a>

<h1>把本地库的内容推送到远程，用git push命令，实际上是把当前分支master推送到远程。由于远程库是空的，我们第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。推送成功后，可以立刻在GitHub页面中看到远程库的内容已经和本地一模一样：</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build17.jpg" alt="Post Build Image">
</a>

<h1>此时，已将本地仓库推送至Github，可打开链接查看部署后的页面：</h1>

<a href="#">
    <img src="{{ site.baseurl }}/img/build18.jpg" alt="Post Build Image">
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