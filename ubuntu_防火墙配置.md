# 安装防火墙
sudo sudo apt-get install ufw

# 防火墙开机自启
sudo ufw enable

# 查看防火墙放行规则(需要开启ssh的22端口)
sudo ufw status

# 开放指定协议的端口
sudo ufw allow [端口号]/tcp



# 关闭指定ip所有操作
sudo ufw delete allow from 192.168.121.1

# 删除放行规则
sudo ufw delete allow 21