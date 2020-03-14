# 科学上网完整攻略
## 客观条件要求：
### 1，代理节点：
>- 免费节点分享：http://bit.ly/3cFPrfV  
>- 免费节点订阅：http://bit.ly/2xa7o67  

### 2，代理客户端：
#### ssr客户端免费下载：
>- PC端：https://github.com/shadowsocksrr/shadowsocksr-csharp/releases  
> -下载最新版本的zip压缩包；  
>- MAC端：https://github.com/qinyuhang/ShadowsocksX-NG-R/releases  
> -下载最新版本的dmg安装包；  
>- 安卓端：https://github.com/shadowsocksrr/shadowsocksr-android/releases  
> -下载最上面的版本 APK安装包（一般Android手机浏览器会自动下安装）。  

#### v2ray客户端免费下载：
>- PC端和MAC端：https://github.com/v2ray/v2ray-core/releases  
> -PC端下载最新版本的zip压缩包；MAC端下载最新的macos版本zip压缩包后解压；  
>- MAC端其他版本v2rayU：https://github.com/yanue/V2rayU/releases  
> -下载最新版本的dmg安装包;  
>- 安卓端：https://github.com/2dust/v2rayNG/releases  
> -下载最新版本的APK安装包。  

>> IOS（苹果手机iphone或ipad）建议使用小火箭shadowrocket和quantumult，但因为大陆商店统统下架，所以只能使用非大陆地区的AppleID，打开App Store才能找到这两个软件，而且这两个软件收费;
>> 如果希望不花钱也可以安装小火箭，请看我的视频：[免费分享美区香港Apple ID(已购买小火箭shadowrocket)](https://youtu.be/NKqto1mePWE)

#### 小火箭shadowrocket和quantumult配置文件规则：
>- 最完善的小火箭翻墙规则：https://github.com/h2y/Shadowrocket-ADBlock-Rules  
>- 各种客户端配置规则：https://github.com/lhie1/Rules  
>> 以上规则足够使用；  
>> 如果youtube出现黑屏 请点进去所使用的规则列表 搜索youtube 删除 "ads.youtube.com"这条规则.
>> 如果不会添加规则，请看我的视频：[小火箭使用教程](https://youtu.be/AacJ9lNunrM)

## 自己搭建代理节点
自己搭建代理节点，需要租用一台vps，这里我以谷歌云为例，因为谷歌云可以免费申请300美金的赠金，并且有一年的有效期。假如赠金用光或是有效期到期，还可以申请新的账号，再获取300美金赠金，并可转移至老账户作为付款账户，如此可以不用修改已经在用的节点而一直免费使用，爽吧！

### 一，ssr节点搭建步骤
#### 系统要求：
>- `CentOS 6+ / Debian 6+ / Ubuntu 14.04 +`  
>- `推荐使用Debian 8+`  
#### 安装：
**简单的来说，如果你什么都不懂，那么你直接一路回车就可以了！**
##### 进入root目录：
>- 首先确认命令符框最前面是不是root@xxxxx  
>- 如果不是, 说明不在根目录，请输入：  

    sudo su
>- 输入上面代码回车后可能会提示你输入当前用户的密码，输入并回车后，没有报错就继续下面的步骤安装ShadowsocksR。

##### ssr一键安装脚本（逗比）：
    wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh
>- 运行后会提示你输入数字来选择要做什么。按提示操作即可;  
>- 如果全部完成，出现黑屏，请滑动一下你的鼠标滚轮！！！  
#### 使用管理：
>- 运行脚本：  

    bash ssr.sh
>- 输入对应的数字来执行相应的命令。  
#### 如果需要网络加速，可以安装BBR:
>- 同样，需要在根目录操作：  
>- 如果没有安装wget GCP服务器，输入安装：  

    yum -y install wget

##### bbr加速一键安装脚本：
    wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubiBackup/doubi/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh
>- 注意：在Debian系统中，删除旧内核时，会提示你是否终止删除内核的行为([点击打开图样](https://user-images.githubusercontent.com/43647204/59249448-653c3a00-8c57-11e9-834c-3d6b1130ca9e.png))，这个需要你选择 <No> (键盘方向键:选择，回车键:确认)。

##### 使用管理：
>- 1:启动bbr:`bash bbr.sh start`
>- 2:关闭bbr:`bash bbr.sh stop`
>- 3:查看bbr状态：`bash bbr.sh status`


### 二，v2ray节点搭建步骤

#### 系统要求：
>- `Ubuntu 16+ / Debian 8+ / CentOS 7+ 系统`  
>- `推荐使用 Debian 9 系统，脚本会自动启用 BBR 优化。`  

#### 安装：
##### 进入root目录：
>- 首先确认命令符框最前面是不是root@xxxxx  
>- 如果不是, 说明不在根目录，请输入：  

    sudo -i

##### v2ray一键安装脚本（233大佬)：
    bash <(curl -s -L https://git.io/v2ray.sh)

>- 如果提示 curl: command not found ，那是因为你的VPS没装Curl;  
>- ubuntu/debian系统安装Curl,输入: `apt-get update -y && apt-get install curl -y`  
>- centos系统安装Curl,输入: `yum update -y && yum install curl -y`  
>- 安装好curl之后就能安装脚本了!  
>- 安装完成后，自动启用bbr加速;  
>- 根目录下输入：`v2ray` 即可管理 V2Ray;  
>- 如果提示你的系统不支持此脚本，那么请尝试更换系统.  

#### 快速管理
>- 查看 V2Ray 配置信息：`v2ray info`
>- 修改 V2Ray 配置：`v2ray config`
>- 生成 V2Ray 配置文件链接：`v2ray link`
>- 生成 V2Ray 配置信息链接：`v2ray infolink`
>- 生成 V2Ray 配置二维码链接：`v2ray qr`
>- 查看 V2Ray 运行状态：`v2ray status`
>- 启动 V2Ray：`v2ray start`
>- 停止 V2Ray：`v2ray stop`
>- 重启 V2Ray：`v2ray restart`
>- 查看 V2Ray 运行日志：`v2ray log`
>- 更新 V2Ray：`v2ray update`
>- 更新 V2Ray 管理脚本：`v2ray update.sh`
>- 卸载 V2Ray：`v2ray uninstall`
    

**请勿违反国家法律法规，否则后果自负！  
使用一键脚本并不会害了你，并且会让你节省大量的时间，工具从来都是为了更快的解决问题。**
