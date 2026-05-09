### 一般客户端连接
+ MQTT服务器地址：mqtts.heclouds.com:1883.对应ip与端口是183.230.40.96:1883
+ 主题订阅: $sys/{产品ID}/{设备名称}/#
+ 主题发布：$sys/{产品ID}/{设备名称}/dp/post/json
+ 发布消息格式：{"id":13,"dp":{"data":[{"v":{"数据流名称1":34,"va1":10,"1on":109.731653,"1at":28.289839}}]}}

### Token生成工具(设备级),用于设备身份认证 !!!注意要在windows10下运行!!!
+ Res 指定到设备ID
`products/{产品id}/devices/{设备名称}`
+ et 过期时间点,是一个时间戳格式
`1757317687`到9月份
+ key
`设备级的key,也就是设备密钥`或`产品级的key,也就是产品界面的access_key`或`用户级别的key,也就是用户Accesskey!!!慎用,权限较高,当设备级key不可用时可尝试`
+ method 加密方式,md5即可
+ version 版本号,默认即可
那Client ID就是:设备名称
用户名是:产品ID
登录的密码就是生成的token

### Token生成工具(产品级),用于设备身份认证


产品级key：cRHpzdufF1NTb7t9geMjQVttNR+XWZGXIRuHXUu9LR8=
用户级key：p2j3QRmqHrXHFCsuNWLmzcJ4iyvyAUDAW0fCAaS0ChRokyKQPOQJEn2vup4ZficM