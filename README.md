# Honeypot-data
部分蜜罐数据及分析 Some honeypot data and analysis(IP address and dicts)


### password
* total:572600
* Duplicate remova:53876

![](https://raw.githubusercontent.com/Kevin-sa/Honeypot-data/master/image/password.png)
图说：从572600次密码爆破中提取频次最多的20个词组。123456、password、admin常见弱密码占据前三位且出现频次大幅度领先。

### username
* total:607222
* Duplicate remove:1736

![](https://raw.githubusercontent.com/Kevin-sa/Honeypot-data/master/image/username.png)
图说：从607222次用户名爆破中提取频次最多的20个词组。第一位是root，出现572584次，是第二位admin出现8943次的64倍，占据总次数的95%。

### ip
* total:139457
* Duplicate remova：3769

![](https://github.com/Kevin-sa/Honeypot-data/blob/master/image/attack_ip.png?raw=true)
图说：从3769个IP地址中提取10个请求次数最多IP，前五位请求均为8670次，且均为腾讯云IP。
![](https://github.com/Kevin-sa/Honeypot-data/blob/master/image/time.png?raw=true)
图说：整理一天24小时内被请求次数，可以发现凌晨5-6点钟到达最高而后慢慢下降，在14：00左右达到小高峰。
![](https://raw.githubusercontent.com/Kevin-sa/Honeypot-data/master/image/ip_country.png)
图说：由于此次数据来源于部署在腾讯云VPS上的蜜罐，所以可以发现攻击IP大多数来自于国内IP。
![](https://raw.githubusercontent.com/Kevin-sa/Honeypot-data/master/image/ip_source.png)
图说：IP地址来源。

### version
* total:92

### Common
* total：40131

Num |Common
----|------
7508| mkdir /tmp/.xs/'  
2996| /tmp/.xs/test.mod
2994| /tmp/.xs/daemon.mipsel.mod
2994| /tmp/.xs/daemon.armv4l.mod
2992| /tmp/.xs/daemon.i686.mod
2990| /tmp/.xs/daemon.mips.mod
1505| cat >/tmp/.xs/daemon.armv4l.mod
1502| cat >/tmp/.xs/daemon.i686.mod
1501| cat >/tmp/.xs/daemon.mips.mod
1500| cat >/tmp/.xs/test.mod




### 期待进一步分析
* ip地址经纬度->ip精确地址
* 开放端口、协议、版本等
* ip的逆向历史域名
* 查询相关威胁情报平台，ip分析的威胁类型，如VPN、C2、Botnet等
