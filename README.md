
##集成阿里百川电商sdk成功过，配置都齐全

###第一次成功 9/28 ：
com.android.tools.build:gradle:3.4.1
gradle-5.1.1-all.zip

debug   版本成功初始化及授权操作
release 版本成功初始化及授权操作（上线）


###第二次上线发版本失败 10/26：
com.android.tools.build:gradle:3.5.1
gradle-5.4.1-all.zip

debug   版本成功初始化及授权操作
release 版本 初始化失败 code = 1 （上线）

logcat ErrorCode = 199
![image.png](/img/bVbzGM2)
![image.png](/img/bVbzGNa)

###于是我换了一台新电脑，装as编辑器的环境，从git拉下上一个电脑提交的代码，直接运行

com.android.tools.build:gradle:3.5.1
gradle-5.4.1-all.zip

debug   版本成功初始化及授权操作
release 版本成功初始化及授权操作（上线）


###最后，我换了一台新mac来装环境。
最开始也是好，用着用着，也出现打release版本无法初始化的问题了。这时候我觉得得解决这个问题，之前是感觉之前得电脑打包坏了，现在复现说明不是。

清空过 .gradle  清空过 .android 都不行，一直初始化失败，但是，dubug百分百可以跑成功，而且初始化以及其他功能都没问题。

替换 com.android.tools.build:gradle:3.5.1
到   com.android.tools.build:gradle:3.4.2
到   com.android.tools.build:gradle:3.4.0
（百川论坛上说：）

![image.png](/img/bVbzGLH)
[https://baichuan.bbs.taobao.com/detail.html?spm=a3c0d.7998979.0.0.5cfb2f45SmgNau&postId=9317077](https://baichuan.bbs.taobao.com/detail.html?spm=a3c0d.7998979.0.0.5cfb2f45SmgNau&postId=9317077)

然后我又测试了demo
点击登陆  提示登陆失败
点击其中一个按钮 闪退  出现如下：
![image.png](/img/bVbzGLX)


请问这个时候我该往那个方向去考虑呢？
