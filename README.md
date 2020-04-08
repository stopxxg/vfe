V2RaySSR综合网
 首 页
 服 务 器
 客 户 端
 优 化 加 速
 VPS各类一键脚本
VPS推荐-评测
 登录   注册
V2RaySSR 综合网还提供 VPS 服务器的推荐和评测。本身不参与和提供工具开发、下载、存储以及任何代理服务。本站非 V2Ray、SSR 官方网站。

遵守国家法律法规、不散谣言、不谈政治、不碰黄赌毒！时刻保持爱国心！若您不能遵守，请离开！

V2RaySSR 综合网仅提供其他作者（V2Ray 搭建、V2Ray 工具、V2Ray 配置、SSR 搭建、SSR 工具、SSR 配置等）作品的解释、介绍及汇总。


 > Trojan搭建 > Trojan搭建失败？Trojan证书未签发？试试最新的Trojan一键脚本！从根本上解决Trojan搭建和安装出现的问题！
Trojan搭建失败？Trojan证书未签发？试试最新的Trojan一键脚本！从根本上解决Trojan搭建和安装出现的问题！
 Trojan搭建  波仔分享  3周前 (03-20)  18453次浏览  27个评论

 
文章导读目录	
前言
准备工作
开始搭建 Trojan
1、检查 SELinux 是否为关闭状态
2、安装基础依赖环境
3、开始运行 Trojan 安装代码
4、安装 BBRPLUS 加速
后记
前言
最近电报群关于 Trojan 的问题是越来越多了，汇聚了大部分的问题发现，居然搭建不成功的占大多数。

但是不成功的大多数又是证书的各种问题，包括证书不签发、证书部署失败。。。 。。。

上一期的手动安装 Trojan 的教程，波仔感觉也是太臃肿了，那么今天来一期简单的半自动化教程。

那么这样的话，大家就知道错误在哪个地方了，解决相应的问题就好了

此脚本写了半天，用各种系统均测试一遍，未发现问题，若有问题，欢迎电报！

GitHub 项目地址：点击访问

视频安装地址：点击观看

Trojan搭建失败？Trojan证书未签发？试试最新的Trojan一键脚本！从根本上解决Trojan搭建和安装出现的问题！

准备工作
1、VPS 一台，系统随意（最好重置新系统，防止各种端口被占用而导致的错误）

2、域名一个，做好解析并已经生效（这一步不懂或是不会请去波仔 YouTube 里面爬楼）

3、赋有极大热情和耐以折腾的精神。。。（这点至关重要）

4、大家一致需要的 V2rayN Trojan 版本来了（支持 Trojan 的 V2rayN）：点击下载

开始搭建 Trojan
1、检查 SELinux 是否为关闭状态
一般情况下，VPS 的 SELinux 处于关闭状态，但是不排除所有，大家检查一下！

/usr/sbin/sestatus -v      ##如果返回参数为 enabled 即为开启，disabled 为关闭
若是开启状态，如何关闭 SELinux 服务？

修改 /etc/selinux/config 文件

将 SELINUX=enforcing 改为 SELINUX=disabled

重启 VPS 以后 SELinux 即为关闭状态。

2、安装基础依赖环境
yum -y install wget    ##ContOS Yum 安装 wget
apt-get install wget   ##Debian Ubuntu 安装 wget
3、开始运行 Trojan 安装代码
代码很简单，三行代码，大家一行一行的复制进去运行，任何问题均有相关提示!

wget -N --no-check-certificate "https://raw.githubusercontent.com/V2RaySSR/Trojansh/master/trojan1.sh" && chmod +x trojan1.sh && ./trojan1.sh
wget -N --no-check-certificate "https://raw.githubusercontent.com/V2RaySSR/Trojansh/master/trojan2.sh" && chmod +x trojan2.sh && ./trojan2.sh
wget -N --no-check-certificate "https://raw.githubusercontent.com/V2RaySSR/Trojansh/master/trojan3.sh" && chmod +x trojan3.sh && ./trojan3.sh
Trojan搭建失败？Trojan证书未签发？试试最新的Trojan一键脚本！从根本上解决Trojan搭建和安装出现的问题！

4、安装 BBRPLUS 加速
wget -N --no-check-certificate "https://github.com/ylx2016/Linux-NetSpeed/releases/download/sh/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
后记
此代码原则上解决了 99.99%的人不会安装 Trojan 的问题，有问题请进群咨询。（不接受私聊，谢谢大家）

V2RaySSR综合网 丨 V2RaySsr.Com
转载链接：Trojan搭建失败？Trojan证书未签发？试试最新的Trojan一键脚本！从根本上解决Trojan搭建和安装出现的问题！
喜欢 (36)
TrojanTrojan MacTrojan 安卓Trojan 安装Trojan一键Trojan一键安装脚本Trojan一键脚本Trojan出错Trojan失效Trojan失败Trojan安装Trojan客户端Trojan成功Trojan搭建Trojan无响应Trojan无法访问Trojan最简单Trojan服务器Trojan续签Trojan脚本Trojan证书Trojan配置最新Trojan
 黑苹果很难吗？记录波仔一次安装黑苹果的过程！4小时的录制，浓缩10分钟的精华。Trojan面板一键搭建！Trojan-Panel一键安装代码！多用户Trojan搭建自动脚本教程！搭建过程中 Compose Token！ 
Trojan面板一键搭建！Trojan-Panel一键安装代码！多用户Trojan搭建自动脚本教程！搭建过程中 Compose Token！
Trojan面板一键搭建！Trojan-Panel一键安装代码！多用户Trojan搭建自动脚本教程！搭建过程中 Compose Token！Trojan客户端下载！告别Trojan.exe和start.bat，一个软件运行Trojan！Trojan也可以如此方便！
Trojan客户端下载！告别Trojan.exe和start.bat，一个软件运行Trojan！Trojan也可以如此方便！Trojan-Panel！Trojan面板！Trojan多用户管理面板！Trojan多人使用流量管控！Trojan Panel搭建保姆级教程！
Trojan-Panel！Trojan面板！Trojan多用户管理面板！Trojan多人使用流量管控！Trojan Panel搭建保姆级教程！最新Trojan一键安装脚本，自动获取Trojan官方最新版本，集成BBRPLUS加速，WIN/MAC客户端智能配置
最新Trojan一键安装脚本，自动获取Trojan官方最新版本，集成BBRPLUS加速，WIN/MAC客户端智能配置
Trojan+宝塔！Trojan与宝塔面板共存！很遗憾，由于Trojan的工作机制，SSL不能被开启！Trojan手动安装教程！手动申请SSL证书、手动搭建/配置Trojan服务器！Trojan客户端软件 Trojan(windows/mac/android/ios)客户端下载全系统支持，Trojan一键安装脚本，自动续签SSL证书，自动配置伪装网站，支持centos7+/debian9+/ubuntu16+VPS综合性能测试！包含VPS硬件信息测试、VPS网络速度测试、VPS回程路由。整合脚本！Trojan面板一键搭建！Trojan-Panel一键安装代码！多用户Trojan搭建自动脚本教程！搭建过程中 Compose Token！Trojan客户端下载！告别Trojan.exe和start.bat，一个软件运行Trojan！Trojan也可以如此方便！Trojan-Panel！Trojan面板！Trojan多用户管理面板！Trojan多人使用流量管控！Trojan Panel搭建保姆级教程！

 
您必须 登录 才能发表评论！
 (27)个小伙伴在吐槽

為什麼最近證書都沒辦法申請成功？
supermarco2020-04-07 19:32 (1天前)登录以回复
«123
热门脚本或工具直达
Trojan 各类安装教程汇聚 V2Ray 各类安装教程汇聚 VPS性能、测速一键脚本 原版BBR/魔改BBR/BBR Plus/锐速V2ray+Ws+Tls+Nginx一键安装脚本



 
随机推荐文章
解锁NetFlix，VPS视讯网站解锁教程，解锁你VPS的奈飞服务（NetFlix），VPS怎么观看奈飞（NetFlix）
解锁NetFlix，VPS视讯网站解锁教程，解锁你VPS的奈飞服务（NetFlix），VPS怎么观看奈飞（NetFlix）
2020-01-0510评论
零成本，体验软路由！Windows虚拟机搭建软路由！OpenWRT最新虚拟机固件！2020-03-05版本！
零成本，体验软路由！Windows虚拟机搭建软路由！OpenWRT最新虚拟机固件！2020-03-05版本！
2020-03-103评论
VPS常用性能测试代码，VPS速度测试代码，VPS一键测试代码（测速代码中文版）
VPS常用性能测试代码，VPS速度测试代码，VPS一键测试代码（测速代码中文版）
2018-12-271评论
原版BBR/魔改BBR/BBR Plus/锐速(Lotserver)四合一脚本/一键安装
原版BBR/魔改BBR/BBR Plus/锐速(Lotserver)四合一脚本/一键安装
2019-04-292评论
香港VPS超低价9.9元/月起，三网直连，香港建站VPS，免备案主机，香港独立网站主机月付9.9元
香港VPS超低价9.9元/月起，三网直连，香港建站VPS，免备案主机，香港独立网站主机月付9.9元
2019-12-313评论

更多标签V2ray Trojan 热门标签
一键安装脚本 (11)V2Ray (10)Trojan (9)V2ray搭建 (7)v2ray+ws+tls (6)V2ray配置 (6)V2ray教程 (5)Trojan教程 (5)Trojan搭建 (5)v2ray一键安装 (4)V2ray客户端 (4)Trojan一键安装脚本 (4)CN2 GIA (4)CN2 GIA线路 (4)v2ray+nginx (3)V2ray安全 (3)Trojan客户端 (3)Trojan Android (3)Trojan原版安装 (3)VPS推荐 (3)美西VPS (3)v2ray+ws+tls一键安装 (2)VPS (2)V2rayIOS (2)V2rayX (2)V2rayU (2)ClashX (2)Trojan一键脚本 (2)V2Ray脚本 (2)Trojan速度怎么样 (2)SSR搭建 (2)Trojan配置 (2)SSR脚本 (2)SSR一键安装 (2)SSR教程 (2)SSR安装 (2)洛杉矶CN2 GIA (2)Trojan IOS (2)Trojan下载 (2)Trojan客户端教程 (2)
最新评论
mmm5小时前说：波哥 PHP7.2等基础依赖安装不成功 怎么处理呢？
waigin11小时前说：面板‘502 Bad Gateway’咋搞
mmm20小时前说：安装源是什么命令 小白求指教
曹小贱23小时前说：GCP搭建了，网站打不开，v2ray也连不上。
supermarco1天前说：為什麼最近證書都沒辦法申請成功？
Copyright © 2019 V2RaySSR综合网 | 网站地图 | 加入波仔电报群
