# Oculus设置

1. 基础的配置教程：https://ocguide.eyw015.com/，详细的问题可以加tg群：https://t.me/Ocguide_cn
2. 不需要折腾WIndows上面Clash的TUN模式，直接Oculus里面连接WiFi时候用你电脑做代理服务器即可
3. 下载[SideQuest](https://sidequestvr.com/setup-howto)并注册账号，下载[Clash For Android](https://github.com/Kr328/ClashForAndroid/releases/download/v2.5.9/cfa-2.5.9-premium-arm64-v8a-release.apk)，之后用SideQuest把它侧载到Oculus里面
4. 打开Oculus浏览器进入你梯子的网站复制订阅导入到Clash里面即可，以后就不需要用电脑做代理服务器了
5. Oculus里面要开启防护系统与手势追踪的功能

6. PC端和手机端下载Oculus
   1. 注册Oculus账号登录
   2. 手机端app配对成功之后打开开发者模式
   3. PC端开启允许未知来源的应用与开发者Runtime功能

7. PC端下载Oculus Develop Hub并注册开发者账号

# 开发设置

+ IDE：Unity Hub + Unity Editor 2021.3.4f1

+ Oculus连接电脑之后要启动Oculus Rift Link的界面才能推流Debug的画面
+ 关于Demo：
  + 目前按照油管系列教程完成：[How to Make a VR Multiplayer Game - PART 1 - YouTube](https://www.youtube.com/watch?v=KHWuTBmT1oI&t=1211s)
  + 多人画面同步使用的是Photon Pun 2提供的服务，服务器是大陆的服务器
  + 尚未加入手势识别功能，还是使用控制器