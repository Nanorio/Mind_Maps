### 1.彻底卸载之前的wsl
### 2.打开windows功能组件Hyper-V,linux子系统,虚拟化平台三个功能
### 3.去github上的[微软项目](https://github.com/microsoft/WSL/releases),下载一个合适版本的wsl.msi
### 4.先安装上,忽略一些错误
### 5.尝试运行wsl --update
### 6.wsl的配置目录为：用户目录下的.wslconfig
```
[wsl2]
# 核心基础配置
memory=1536MB
swap=512MB
# 镜像网络与 DNS 隧道在 2.x 中已属于稳定配置
networkingMode=mirrored
dnsTunneling=false
firewall=true
autoProxy=true
guiApplications=false

[experimental]
# 这两项在某些版本中必须放在 experimental 下才能被识别
sparseVhd=true
autoMemoryReclaim=gradual
```
### 7.安装发行版,可以在微软商店或者命令行，也可以离线安装自己喜欢的发行版
### 8.默认启动使用wsl2设置——wsl --set-default-version 2
### 9.默认启动发行版设置——wsl --set-default [发行版]
### 10.启动命令——wsl --distribution [发行版] 或者 wsl