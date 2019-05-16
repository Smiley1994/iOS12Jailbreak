# iOS12Jailbreak
Currently available iOS12 Jailbreak tool～～

### iOS12 Jailbreak

一 、 
iOS 12 - 12.1.2 不完美越狱，需要注意的是，本教程为不完美越狱，设备重启后还需要再重新越狱一次。另外，本次越狱，仅支持iPhone 6s - iPhone 8P等设备，太老或者最新的XS/XR等设备暂不支持，这点也需要注意下。

如果iPhone中已经下载了系统OTA 升级文件，则需要; 设置 -> 通用->iPhone存储空间里将已经下载的系统升级文件删除，再重启iPhone。如果没有，则忽视此步。

1.https://ignition.fun  install APP (ignition)

2.安装 UncOver (设置 -> 通用 -> 描述文件 -> 信任) 打开uncOver App

3.打开后点击 “ Jailbreak ”，进行越狱， 期间 N 次重启 每次重启后重新打开 uncOver 直到桌面出现 Cydia APP

4.如果没有Cydia或者Cydia出现闪退的，可以打开uncOver--Settings--将Reinstall Cydia打开、Reinstall System Daemons关闭。返回再重新击“Jailbreak”即可


***

https://github.com/nabla-c0d3/ssl-kill-switch2/releases  下载 .deb 文件

二 安装SSL KILL Switch  详情请参照：https://github.com/nabla-c0d3/ssl-kill-switch2
* 首先iOS系统必须是越狱之后的。

* 越狱成功之后手机桌面会有Cydia的app，在Cydia里边安装插件

1.Debian Packager

2.Cydia Substrate

3.PreferenceLoader

4.将 .deb 文件 拷贝到 已经越狱的 iPhone 里 
  scp  ***.deb root@192.***.*.**:/var/root/sslKillSwitch2

5.通过 终端 ssh root@192.***.*.**  进入iPhone 目录 执行 以下命令行。
  （ 链接Wi-Fi 查看 当前IP地址 ， 默认密码 ： alpine）
  
  ```   
  dpkg -i <package>.deb
  killall -HUP SpringBoard
  ```
     
完成之后在手机设置里边打开SSL Kill Switch开关。
