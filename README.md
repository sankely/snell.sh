# 此脚本仅用于远程连接家中局域网内机器，请勿用于任何非法行为！
## Snell Version 2.0.6
## https://github.com/surge-networks/snell
## 运行完毕后屏幕显示psk，默认端口号13254（我随手那么一按( ̀⌄ ́)，按照标准填入Surge即可。

Debian & Ubuntu 用户请运行

```
apt update -y
wget --no-check-certificate -O snell.sh https://raw.githubusercontent.com/sankely/snell.sh/master/snell.sh
chmod +x snell.sh
./snell.sh
```

首次安装默认端口号13254，如需修改请
在所有脚本运行结束后运行

```
nano /etc/snell/snell-server.conf
systemctl restart snell
```

自行修改。

当然你也可以用 vi ^o^

查看运行状态：

```
systemctl status snell #查看运行状态
systemctl restart snell #重启Snell服务
systemctl start snell #启动Snell服务
systemctl stop snell #停止Snell服务
cat /etc/snell/snell-server.conf #查看Snell配置文件
vi /etc/snell/snell-server.conf #修改Snell配置文件
```

卸载方法：

```
wget --no-check-certificate -O uninstall-snell.sh https://raw.githubusercontent.com/primovist/snell.sh/master/uninstall-snell.sh
chmod +x uninstall-snell.sh
./uninstall-snell.sh
```
