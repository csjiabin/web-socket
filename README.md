#web-socket
###  **web-socket即时聊天应用** 
> 你需要在本机安装Node.js（废话）

> 模块都安装好的没删掉不需要重新安装

> 进入文件夹，按shift+鼠标有键打开命令行，运行node server启动服务器

> 打开浏览器访问localhost:3000(3000端口)

![输入图片说明](http://git.oschina.net/uploads/images/2017/0302/102049_f4cde327_1013316.png "在这里输入图片标题")
![输入图片说明](http://git.oschina.net/uploads/images/2017/0302/102118_852d81eb_1013316.png "在这里输入图片标题")
```
<!doctype html>
<html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
        <meta name="author" content="Wayou">
        <meta name="description" content="hichat | a simple chat application built with node.js and websocket">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Web Socket</title>
        <link rel="stylesheet" href="css/main.css">
        <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
        <link rel="icon" href="favicon.ico" type="image/x-icon">
    </head>
    <body>
        <div class="wrapper">
            <div class="banner">
                <h1>Web Socket</h1>
                <span id="status"></span>
            </div>
            <div id="historyMsg">
            </div>
            <div class="controls" >
                <div class="items">
                    <input id="colorStyle" type="color" placeHolder='#000' title="font color" />
                    <input id="emoji" type="button" value="emoji" title="emoji" />
                    <label for="sendImage" class="imageLable">
                        <input type="button" value="图片"  />
                        <input id="sendImage" type="file" value="图片"/>
                    </label>
                    <input id="clearBtn" type="button" value="清屏" title="清除屏幕" />
                </div>
                <textarea id="messageInput" placeHolder="输入发送"></textarea>
                <input id="sendBtn" type="button" value="发送">
                <div id="emojiWrapper">
                </div>
            </div>
        </div>
        <div id="loginWrapper">
            <p id="info">连接到服务器...</p>
            <div id="nickWrapper">
                <input type="text" placeHolder="昵称" id="nicknameInput" />
                <input type="button" value="OK" id="loginBtn" />
            </div>
        </div>
        <footer>
            <small>view on <a href="https://github.com/Wayou/HiChat">GitHub</a> | <a href="mailto:liuwayong@gmail.com">contact me</a></small>
        </footer>
        <script src="/socket.io/socket.io.js"></script>
        <script src="js/hichat.js"></script>
        <script>
        /**如果你不能删除我访问谷歌服务**/
          (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
          (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
          m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
          })(window,document,'script','//www.google-analytics.com/analytics.js','ga');
        
          ga('create', 'UA-46794744-7', 'hichat.herokuapp.com');
          ga('send', 'pageview');
        /**删除结束**/
    </script>
    </body>
</html>

```
