## Linux 操作體驗問題集錦

1. ##### 使用shadowsocks代理命令行命令

參考自https://github.com/shadowsocks/shadowsocks/wiki/Using-Shadowsocks-with-Command-Line-Tools

apt-get install proxychains
Make a config file at ~/.proxychains/proxychains.conf with content:
```
strict_chain
proxy_dns 
remote_dns_subnet 224
tcp_read_time_out 15000
tcp_connect_time_out 8000
localnet 127.0.0.0/255.0.0.0
quiet_mode

[ProxyList]
socks5  127.0.0.1 1080
```
使用：proxychains wget/curl/pip/git XXXX

##### 2. 那些可以在linux上一鍵安裝的軟件就別再找下載鏈接了

sudo apt-get install vlc/shadowsocks/texmaker/

