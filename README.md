# Mac 装机必备 App、常见设置、删除自带 ABC 输入法

## 常用软件

### 工具类

- 微信输入法：https://z.weixin.qq.com
- 搜狗输入法：https://pinyin.sogou.com/mac
- PasteNow 历史剪切板：https://apps.apple.com/cn/app/pastenow-剪贴板工具/id1552536109
- One Switch 快捷开关：https://fireball.studio/oneswitch
- Keka 压缩：https://www.keka.io/en
blackmagic-disk-speed-test/id425264550
- AS Timer 倒计时：https://apps.apple.com/cn/app/as-timer/id512464723
- GitHub Desktop：https://desktop.github.com
- MonitorControl 控制外接显示器亮度：https://github.com/MonitorControl/MonitorControl
- Visual Studio Code 微软出品：https://code.visualstudio.com
- PopClip 制作 PopMaker：https://brettterpstra.com/2014/05/12/popmaker-popclip-extension-generator
- Hapigo 第三方聚焦搜索：https://www.hapigo.com
- QuickRecorder 录屏软件：https://github.com/lihaoyun6/QuickRecorder
- Timer 桌面计时器：https://github.com/michaelvillar/timer-app/releases
- AirBattery 显示手机等设备电量：https://github.com/lihaoyun6/AirBattery
- Command X 剪切：https://apps.apple.com/us/app/command-x/id6448461551

### 处理图片
- Upscayl 图片放大：https://github.com/upscayl/upscayl
- PictureView 图片预览查看：https://wl879.github.io/apps/picview/index.html

### 窗口管理
- Rectangle 窗口管理：https://github.com/rxhanson/Rectangle/releases
- Contexts 切换后台应用：https://contexts.co/

### 硬盘信息
- Drivedx 硬盘信息：https://binaryfruit.com/drivedx
- Blackmagic Disk Speed Test 硬盘读写：https://apps.apple.com/cn/app/
- iStat Menus 监控系统数据：https://bjango.com/mac/istatmenus


### 代理
- Speedtest 测网速：https://apps.apple.com/cn/app/speedtest-by-ookla/id1153157709
- Mihomo Party 代理工具：https://mihomoparty.org


### 浏览器
- Chrome：https://www.google.com/intl/zh-CN/chrome
- Firefox：https://www.mozilla.org/zh-CN/firefox/new
- Safari 去广告 Adguard：https://apps.apple.com/cn/app/adguard-for-safari/id1440147259
- Safari Tampermonkey：https://apps.apple.com/cn/app/tampermonkey/id1482490089
- 沉浸式翻译 Safari 扩展：https://apps.apple.com/cn/app/沉浸式翻译safari扩展/id6447957425
- 文本识别 TextSniper 支持多国语言：https://textsniper.app

### 社交

- 微信：https://weixin.qq.com
- Telegram：https://telegram.org
- 微博 Maipo：https://apps.apple.com/cn/app/maipo-for-微博/id789066512

### 翻译
- 翻译 Bob：https://apps.apple.com/cn/app/bob-翻译和-ocr-工具/id1630034110
- 划词扩展 PopClip：https://apps.apple.com/cn/app/popclip/id445189367


1. 快捷启动应用 Thor：https://github.com/gbammc/Thor
2. 密码管理 Enpass：https://apps.apple.com/cn/app/enpass-password-manager/id732710998

### 截图
- CleanShot X：https://cleanshot.com
- Shottr：https://shottr.cc
- Xnip：https://apps.apple.com/cn/app/xnip-截图-标注/id1221250572

### Markdown
- Markdown Typora：https://www.typora.io
- Markdown MWeb Pro：https://apps.apple.com/cn/app/one-markdown/id1507139439

### 邮件
- Spark：https://apps.apple.com/cn/app/spark-readdle-出品的邮箱应用/id1176895641

### 影音
- IINA 播放器：https://iina.io
- IINA+ 直播助手：https://github.com/xjbeta/iina-plus
- Simple Live 斗鱼 B 站直播 ：https://github.com/xiaoyaocz/dart_simple_live
- APTV 看央视直播：https://apps.apple.com/cn/app/aptv/id1630403500

### 处理视频
- handbrake 视频压缩：https://handbrake.fr/
- Downie 下载视频：https://software.charliemonroe.net/downie
- VideoProc Converter 视频裁剪：https://www.videoproc.com

### 卸载/清理垃圾
- App Cleaner & Uninstaller 卸载：https://nektony.com/mac-app-cleaner
- 腾讯柠檬：卸载清理垃圾：https://lemon.qq.com

### 计算器
- Soulver 3：：https://apps.apple.com/cn/app/soulver-3/id1508732804
- Numi：https://numi.app

### 云盘
- 阿里云盘：https://www.alipan.com

## 程序坞显示时间
如果你习惯隐藏程序坞，鼠标放在屏幕底部，默认显示程序坞非常慢，你可以在【终端】输入或粘贴下面命令，将数值改为 `0`，这样，显示程序坞会变的很快。

```
defaults write com.apple.dock autohide-delay -int 0
```

再输入下面命令。

```
killall Dock
```



## 允许任何来源
【终端】输入或粘贴以下命令，按回车键，输入密码按回车键。

```
sudo spctl --master-disable
```



## 密码位数

管理员默认密码至少为 `4` 位，【终端】输入或粘贴以下命令支持将密码改为 `1` 位。

```
pwpolicy -clearaccountpolicies
```



## SIP 状态
【终端】输入 `csrutil status`，按回车键。

### 关闭 SIP
1. Mac 开机立即按住 `Command-R`
2. 进入实用工具窗口，点击**实用工具**里【终端】，输入下面命令按回车键，重启 Mac

```
csrutil disable
```

### 开启 SIP
同上，【终端】输入下面命令。

```
csrutil enable
```



## 关闭输入法切换提示
终端里运行完以下两个命令后重启 Mac

```
sudo mkdir -p /Library/Preferences/FeatureFlags/Domain
```
```
sudo /usr/libexec/PlistBuddy -c "Add 'redesigned_text_cursor:Enabled' bool false" /Library/Preferences/FeatureFlags/Domain/UIKit.plist
```



## 提示“已损坏，无法打开，移到废纸篓”
1. 打开允许任何来源（上方）
2. 打开终端，输入 `xattr -cr`（cr后面加入一个空格），将 App 拖到终端，按回车键

注1：Ventura 13 以上系统，先前往设置 - 隐私与安全性 - 完整磁盘访问权限中允许终端。然后才能操作，否则会遇到 Operation not permitted\
注2：macOS 13+ 以上系统上操作之后如果还是提示损坏，右键软件选择【打开】




## 删除 ABC

1. 系统偏好设置 → 键盘 → 输入法编辑 → 添加英语（选择美国），再删除 ABC。
2. 前往文件夹（Command-Shift-G）输入下面路径找到对应文件，并用 [Xcode](https://apps.apple.com/cn/app/xcode/id497799835?mt=12) 软件打开。

注：路径中 `XXX` 替换为你的 Mac 用户名。
```
/Users/XXX/Library/Preferences/com.apple.HIToolbox.plist
```

3. 删除所有包含 `U.S.` 的文件并保存，重启 Mac。
![](https://i.imgur.com/q9xTLLL.png)

还原：系统偏好设置 → 键盘 → 输入法 → 添加 `US 美国` 或 `ABC`。



## 查看 Mac 硬盘写入量
1. 下载工具并安装：https://sourceforge.net/projects/smartmontools/
2. 打开终端，输入下面代码按回车键
```
/usr/local/sbin/smartctl -a /dev/disk0
```



## 退出所有程序快捷指令

https://www.icloud.com/shortcuts/9075b6e71a4e4045a372c5557349fb8c


## 测试网速
在终端中输入 `networkQuality`

官网介绍：https://support.apple.com/zh-cn/101942



## Chrome 浏览器开启 HDR
打开浏览器输入 [chrome://flags/#force-color-profile](chrome://flags/#force-color-profile) 选择 HDR10

## 启动台行列
【终端】输入或粘贴以下命令，修改后面的数字更改行列数。

行数

```
defaults write com.apple.dock springboard-rows -int 7
```

列数

```
defaults write com.apple.dock springboard-columns -int 9
```

最后输入以下命令

```
killall Dock
```

## 网页显示方框里带问号
安装新字体时字体冲突，导致浏览器网页中字体显示成方块里带问号，需要清一下字体缓存。
![](https://i.imgur.com/Lkk0Gja.png)

1. 关闭所有 app
2. 打开终端 Terminal
3. 终端输入：`sudo atsutil databases -remove`
4. 输入电脑密码，按回车
5. 终端输入：`atsutil server -shutdown`
6. 终端输入：`atsutil server -ping`
7. 重启电脑


