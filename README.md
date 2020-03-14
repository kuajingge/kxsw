## 一，ssr安装
### 进入root目录：
	sudo su
### ssr一键安装脚本：
    wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh
### 使用管理：
    bash ssr.sh
### bbr加速一键安装脚本：
    wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubiBackup/doubi/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh
### 使用管理：
#### 1:启动bbr:
    bash bbr.sh start
#### 2:关闭bbr:
    bash bbr.sh stop
#### 3:查看bbr状态：
    bash bbr.sh status
### ssr客户端下载：
> PC端：https://github.com/shadowsocksrr/shadowsocksr-csharp/releases
下载最新版本的zip压缩包；  
> MAC端：https://github.com/qinyuhang/ShadowsocksX-NG-R/releases
下载最新版本的dmg安装包；  
> 安卓端：https://github.com/shadowsocksrr/shadowsocksr-android/releases
下载最上面的版本 APK安装包（一般Android手机浏览器会自动下安装）。  
> IOS 建议使用shadowrockt 和quantumult，但因为大陆商店统统下架，所以只能使用非大陆地区的AppleID再打开App Store才能找到这两个软件，而且这两个软件收费 但建议购买 如何充值非大陆地区AppleID 可以去我视频里找教程

## 二，v2ray安装

### 进入root目录：
    sudo -i

### v2ray一键安装脚本：
    bash <(curl -s -L https://git.io/v2ray.sh)

备注：安装完成后，自动启用bbr加速，根目录下输入：`v2ray` 即可管理 V2Ray

### 快速管理
#### 查看 V2Ray 配置信息：
    v2ray info
#### 修改 V2Ray 配置：
    v2ray config
#### 生成 V2Ray 配置文件链接：
    v2ray link
#### 生成 V2Ray 配置信息链接：
    v2ray infolink
#### 生成 V2Ray 配置二维码链接：
    v2ray qr
#### 查看 V2Ray 运行状态：
    v2ray status
#### 启动 V2Ray：
    v2ray start
#### 停止 V2Ray：
    v2ray stop
#### 重启 V2Ray：
    v2ray restart
#### 查看 V2Ray 运行日志：
    v2ray log
#### 更新 V2Ray：
    v2ray update
#### 更新 V2Ray 管理脚本：
    v2ray update.sh
#### 卸载 V2Ray：
    v2ray uninstall

请勿违反国家法律法规，否则后果自负！  
使用一键脚本并不会害了你，并且会让你节省大量的时间，工具从来都是为了更快的解决问题。
