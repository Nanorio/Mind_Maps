<center>AT指令</center>
=============================

### 🚩信息查看
#### 测试指令
`AT`
#### 查询wifi模式
`AT+CWMODE?`
#### 查询wifi重连条件
`AT+CWRECONNCFG?`
#### AP信息
`AT+CWJAP?`
#### 查询AP模式时DHCP的配置信息
`AT+CWDHCPS?`
#### 扫描并显示附近AP
`AT+CWLAP`
#### 查询上电时是否自动连接可连接的AP
`AT+CWAUTOCONN?`
#### 查询AP模式下的802.11协议标准
`AT+CWAPPROTO?`
#### 查看STA模式下的802.11协议标准
`AT+CWSTAPROTO?`
#### 查看本设备AP的MAC地址
`AT+CIPAPMAC?`
#### 查看STA的MAC地址
`AT+CIPSTAMAC?`
#### 查看本设备AP的IP地址
`AT+CIPAP?`
#### 查看本设备STA的IP地址
`AT+CIPSTA?`
#### 查看当前时间
`AT+CIPSNTPTIME?`
<hr />

### 🚩配置命令(配置修改后即写入存储，rst后生效)

#### 复位指令
`AT+RST`
#### 开启DHCP(AP模式或STA模式)
`AT+CWDHCP`
#### 设置AP模式时DHCP分配的ip地址范围,租约时间
`AT+CWDHCPS`
#### 断开与当前AP的连接
`AT+CWQAP`
#### 设置AP模式时的SSID和密码
`AT+CWSAP`
#### 踢除连接本AP的所有设备(或指定设备)
`AT+CWQIF`
#### 设置扫描AP时的设置
`AT+CWLAPOPT`
#### 查看已连接AP的信息(ip,mac)
`AT+CWLIF`
#### 配置上电时是否自动连接可连接的AP
`AT+CWAUTOCONN`
#### 配置AP模式下的802.11协议标准
`AT+CWAPPROTO`
#### 配置STA模式下的802.11协议标准
`AT+CWSTAPROTO`
#### 配置本设备AP的MAC地址
`AT+CIPAPMAC`
#### 配置本设备STA的MAC地址
`AT+CIPSTAMAC`
#### 配置本设备AP的IP地址
`AT+CIPAP`
#### 配置本设备STA的IP地址
`AT+CIPSTA`
#### 开启SmartConfig
`AT+CWSTARTSMART`
#### 关闭SmartConfig
`AT+CWSTOPSMART`
#### 开启WPS功能(即WiFi连接保护设置,当设备对连接本AP时,使用WPS并输入配对码避免直接输入密码,提高安全性)
`AT+WPS`
#### 设置mDNS功能(访问本设备时,通过主机名而非IP地址访问本设备)
`AT+MDNS`
#### 设置STA模式下的本主机名(注意:AP模式下本主机名不可设置,两者是独立的)
`AT+CIPHOSTNAME`
#### 将ESP设备连接入MQTT服务器
`AT+MQTTUSERCFG=0,1,"{设备名称}","{产品ID}","{token计算工具生成的token}",0,0,""`



### 🚩例子
`AT+CWSAP="ESP01s1A","",1,0,4,0`设置ap模式的参数，包括名称，密码，信道，加密方式，最大连接数，是否隐藏(1为隐藏)
`AT+CIPAPMAC="7c:7d:21:f6:97:9c"`修改AP的mac地址，貌似只能修改ap的mac地址，client的mac无法设置



















