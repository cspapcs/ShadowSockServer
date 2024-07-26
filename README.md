# ShadowSockServer
ShadowSockServer Created In Linux.

```
apt -y install gcc automake autoconf libtool make
wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
chmod +x shadowsocksR.sh
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
```

第一步：设定密码，default 为默认密码
第二步：设定端口，default 为随机生成默认端口
第三步：设定加密方式，default 为默认加密方式
第四步：设协议，default 为默认协议
第五步：设定混淆方式，default 为默认混淆
第六步：安任意键，回车开始进行安装，安装完成后自动启动

安装过后如果想要修改，运行如下相关命令

启动：/etc/init.d/shadowsocks start

停止：/etc/init.d/shadowsocks stop

重启：/etc/init.d/shadowsocks restart

状态：/etc/init.d/shadowsocks status

配置文件路径：/etc/shadowsocks.json 修改文件用vi 或者 vim命令，使用方法百度

日志文件路径：/var/log/shadowsocks.log

安装路径：/usr/local/shadowsocks/shadowsoks

卸载./shadowsocksR.sh uninstall

# BBR加速
安装bbr加速
```
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
chmod +x bbr.sh
./bbr.sh
```
重新连接后，输入 lsmod | grep bbr 查看BBR是否启动

# 下载ShadowSocksR客户端
https://github.com/ShadowsocksR-Live/ssrWin/releases
