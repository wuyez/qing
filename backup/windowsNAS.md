看到一篇文章，使用windows系统做NAS，这里复制下方案，备用。
系统：WINDOWS 10 专业版
基础环境: 基于PhpStudy的集成环境（包含php，mysql，nginx等一键安装配置）
[相册](https://www.smzdm.com/fenlei/xiangce/)软件：digikam （可按时间轴，[地图](https://www.smzdm.com/fenlei/ditu/)查看照片，有人脸识别，基于数据库，速度快）
影音服务：Jellyfin （老牌子了）
同步软件：微力同步 (可局域网也可外网同步，远程基于p2p)
备份：veeam backup 社区版 （超强备份软件，文件增量备份，hyper-v增量备份）
各类文件预览/远程访问：可道云（相当于web版远程桌面），也可以当web版照片管理软件
DDNS：花生壳 （用于内网穿透）
虚拟机：hyper-v / docker
搜索：Everything
1.Jellyfin满足影音管理，远程观看等
2.微力同步满足不同机器之间的同步需要
3.DigiKam和可道云满足照片管理需要，一个是本地端软件，一个是Web端
4.可道云可以满足在线编辑文档表格等，在线写代码都可以
5.Veeambackup基本满足了所有备份需求，如果有Mac需要需要备份在这个NAS上，可以通过创建VHD虚拟硬盘共享给MAC，网上有教程可以去查查
6.Windows共享基本满足了局域网共享磁盘的需要，如果满足不了还可以安装其他软件补充
7.windows强大的远程桌面基本上秒杀了各种NAS的网页管理体验
8.Docker和Hyper-v作为扩展，进行其他系统或软件的运行，不过这台矿渣弱了点，虚拟机费劲
9.花生壳做DDNS，方便远程访问
原文网址：https://www.cnblogs.com/lickyzh/p/14953015.html