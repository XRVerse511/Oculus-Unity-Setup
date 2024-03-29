# Oculus 设置

1. 基础的配置教程：https://ocguide.eyw015.com/ 详细的问题可以加 tg 群：https://t.me/Ocguide_cn
2. 不需要折腾 WIndows 上面 Clash 的 TUN 模式，直接 Oculus 里面连接 WiFi 时候用你电脑做代理服务器即可
3. 下载[SideQuest](https://sidequestvr.com/setup-howto)并注册账号，下载[Clash For Android](https://github.com/Kr328/ClashForAndroid/releases/download/v2.5.9/cfa-2.5.9-premium-arm64-v8a-release.apk)，之后用 SideQuest 把它侧载到 Oculus 里面
4. 打开 Oculus 浏览器进入你梯子的网站复制订阅导入到 Clash 里面即可，以后就不需要用电脑做代理服务器了
5. Oculus 里面要开启防护系统与手势追踪的功能

6. PC 端和手机端下载 Oculus

   1. 注册 Oculus 账号登录
   2. 手机端 app 配对成功之后打开开发者模式
   3. PC 端开启允许未知来源的应用与开发者 Runtime 功能

7. PC 端下载 Oculus Develop Hub 并注册开发者账号

# 开发设置

- IDE：Unity Hub + Unity Editor 2021.3.4f1 + Visual Studio 2019
- Unity编辑器设置
  - Edit > Preferences > External Tools > External Script Editor 选中 Microsoft Visual Studio 2019 下面的框都勾选
  - Edit > Project Settings > Player > PC图标 > Resolution and Presentation > Resolution > Fullscreen Mode > 选中 Windowed
  - Edit > XR Plug-in Management > Intall > 之后在PC图标和安卓图标下面勾选Oculus
  - File > Build Settings > Scenes In Build > Add Open Scenes
- Oculus 连接电脑之后要启动 Oculus Rift Link 的界面才能推流 Debug 的画面
- 关于 Demo：
  - 目前按照油管系列教程完成：[How to Make a VR Multiplayer Game - PART 1 - YouTube](https://www.youtube.com/watch?v=KHWuTBmT1oI&t=1211s)
  - 网络层的解决方案使用的是 Photon Pun 2 提供的免费服务，上海的服务器
  - 尚未加入手势识别功能，还是使用控制器
- 下一步的改进计划：
  - 使用 [Mirror](https://mirror-networking.gitbook.io/docs/) 或者 [MLAPI](https://docs-multiplayer.unity3d.com/netcode/current/about/index.html) 重写网络层的画面同步，并部署 Server 
    - Mirror 是第三方的库， MLAPI 是 Unity 官方推出的 UNet 后继版本
    - 目前倾向于使用 MLAPI
  - 集成 Oculus 提供的手势识别SDK，做动作识别功能
  - 优化游戏场景与人物 Avatar 
