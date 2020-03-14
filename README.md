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
