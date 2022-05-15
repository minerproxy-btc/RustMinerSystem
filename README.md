# 安装完成后，请立即修改程序端口和密码，以防别有用心之人，扫描端口偷偷登录！！
部分机房封禁e池5555等矿池常见端口；受到影响的请自行更换e池tcp 4444，14444端口进行转发

已内置加密证书，可以自定义证书,在程序目录下放入key.pem和cert.pem文件即可； 
任何问题进群联系群主；

安装好之后记得改掉默认的访问端口；文件名是config.yml；用记事本打开更换！linux要改etc目录下
MinerProxy-Eth里的config；可以下载一个FinalShell控制台，更改linux目录更方便

linux改好端口之后输入supervisorctl restart all 后生效！

转发使用的地址，请一定使用官方地址；以避免被二次暗抽

装过其他同类软件，使用本软件前，请一定重做系统！以防后门

# windows版本下载:
点击左侧Code，然后选Download ZIP即可！

# linux服务器一键安装脚本
```bash
bash <(curl -s -L https://raw.githubusercontent.com/minerproxyeth/MinerProxy-Eth/main/install.sh)
```
自带守护，开启最大连接数
安装后输入supervisorctl restart all 回车生效！

纯转发模式使用后算力截图，算力几乎无损耗。
![img_9.png](img_9.png)


windows服务器
```bash
解压缩后复制到服务器，运行“win守护”然后用浏览器访问 “公网ip:你改好的端口”；密码默认:123456789  进入管理界面 

设置你的转发矿池/端口；可选择“不抽水”(自用) 或者“抽水”(分担服务器费用)；

支持LINUX，WINDOWS服务器，支持纯转发和自定抽水比例；包含自启动和进程守护；

还在被所谓的直连\中转IP抽水吗？自建转发；支持SSL加密；高并发，稳定一键搞定！


（如果遇到打不开管理界面，请开放服务器对应的端口）
```

任何问题请加TG群： https://t.me/MinerProxy_eth


# Liunx-手动安装
```bash
git clone https://github.com/minerproxyeth/minerproxy.git 
cd minerproxy
chmod a+x minerProxy_3.0.3_linux 
nohup ./minerProxy_3.0.3_linux & (后台运行，注意：& 也需要复制，运行完再敲几下回车)
tail -f nohup.out (后台运行时查看)
```

