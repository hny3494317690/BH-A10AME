HL出品的BH-A10AME是一款由紫晶储存定制的BDXL刻录机，基于MT1959平台，其硬件配置与AUAS BW-16D1HT一模一样<br/><br/>
由于紫晶专有固件的限制，BH-A10AME可以刻录紫晶定制的三菱100GB BDXL蓝光碟，但是代价是失去了UHD读取能力，虽然是2020年的产品，却只支持AACS v62加密，这将导致其无法识别所有的UHD电影碟<br/><br/>
好消息是，我们可以通过将其刷入AUAS BW-16D1HT的固件来使其具有UHD读写能力，如果您在某些中国购物网站购买了该产品并且您只有一个蓝光光驱，这个方法可以让你不用再去购买额外的光驱来读取UHD电影碟<br/><br/>
本方案只适用于Windows，且不适用于使用SATA to USB的笔记本用户，支持MakeMKV完整功能
方法如下：<br/><br/>
1.在 https://github.com/hny3494317690/BH-A10AME/releases 中下载最新版的SDFtool.Flasher
2.下载https://github.com/hny3494317690/BH-A10AME/blob/main/ASUS-BW-16D1HT-3.10-WM01601-211901041014.bin
3.保持光驱连接电脑，取出光驱里的光盘
4.打开SDFtool.Flasher，在下拉栏中选择BH-A10AME，右侧选择Read FW，点击Start，耐心等待完成
5.在软件根目录Firmware_Dumps文件夹下找到备份的FW文件，妥善保管，这是你当前光驱的固件备份，可用于后续还原固件
6.在软件窗口右侧选择RECOVER Drive，在弹出的文件管理器中选择ASUS-BW-16D1HT-3.10-WM01601-211901041014.bin文件打开，点击Start
7.耐心等待烧录完成后，重启电脑
8.正常读取UHD电影碟
