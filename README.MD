# 如何科学上网教程

安装浏览器
--------

个人推荐直接使用谷歌Chrome浏览器，但国内因为无法直接下载和访问Chrome浏览器下载链接，个人推荐[Vivaldi](https://vivaldi.com/zh-hans/)。
Vivaldi有比较好的用户体验以及颜值，同时和谷歌Chrome一样支持标签云同步，当然其核心也是chrome的，所以支持chrome的任何插件。

安装ShadowSocks连接客户端
-----------------------
1. Windows

在安装前需要确保[微软.NET Framework 4.6.2或者以上版本](https://docs.microsoft.com/zh-cn/dotnet/framework/install/index)和[微软 Visual C++ 2015 Redistributable](https://www.microsoft.com/zh-CN/download/details.aspx?id=48145) 已经安装，否则会打不开ShadowSocks Windows版。

[下载ShadowSocks Windows版](https://github.com/shadowsocks/shadowsocks-windows/releases)，把压缩包解压放到非系统盘下，或者桌面上弄个文件夹也行，因为在系统盘下此App无法写配置文件到当前目录，所以如果你录入ss节点后关掉app所有记录会消失。



2. Mac

Mac下简单很多，直接[在这里下载zip之后](https://github.com/shadowsocks/ShadowsocksX-NG/releases/)，解压安装dmg文件，在右上角会多一个小飞机图标，就代表运行了。

* ShadowSocks 运行后会在Windows的任务栏右边或者Mac的系统菜单栏的最右边的状态栏多出一个小飞机的图标，就代表运行了。之后就是通过其中的扫码或者手动录入


SS服务购买推荐
------------

这里我推荐几个比较优秀的服务：

[RiftXX](https://portal.riftxx.com):按照流量收费， 日本香港 台湾节点Youtube快的飞起。

[CloudSS](https://go.cloudss.me):有流量和月租，日本香港也不错，但不支持Netflix

* 在上网时 当有网址提示想访问GeoLocation就是地理位置时，尽量选禁止。


SwitchyOmega安装和使用教程
------------------------

安装SwitchyOmega的步骤请参考[SwitchyOmega Wiki链接](https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList).
  * 一开始会因为无法翻墙而导致无法访问谷歌商店，您也可以直接[在 Github 上下载最新版安装包](https://github.com/FelisCatus/SwitchyOmega/releases)，然后按照下载页面上的说明手动安装。
  * Chrome浏览器在地址栏输入:chrome://extensions；Vivaldi浏览器则是vivaldi://extensions。进去以后可以把上面离线版的crx安装包拖入安装就可以。
  * 注意先开Shadowsocks Windows或者NG连接ss服务后才能通过此插件翻墙。SwitchyOmega原理就是把GFWList里需要翻墙的网址通过本地的1080端口走到ShadowSocks-Windows或者Ng进行通信。

  SwitchyOmega各种模式是什么
  ------------------------

  #### 自动代理模式(Auto Proxy)：

  这个模式当你访问一个网址时，插件会查找GFWList中的列表，如果找到了说明该网址是被屏蔽需要翻墙，如果是像国内的常用网址那就直接连接不走代理，以节省代理服务器压力和流量。

  #### 全局代理模式(Global Mode):
  
  这个模式下将无视列表，所有的网址都会走代理，注意在此模式开启下，部分国内视频会锁区，不过像某B站部分锁区视频也可以反过来解锁。

  #### 系统代理模式:

  此模式一般会在Mac下设置，而控制全局和自动模式则是小飞机ShadowSocks NG的职责。完游戏慎用ShadowSocks NG系统代理模式，因为所有App的连接都会试图走这一路。

这一些配置后就可以访问Youtube，Facebook， SoundCloud，Twitter，Discord等等的网站了
