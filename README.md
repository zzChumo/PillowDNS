# PillowDNS，一款可以去广告的安全DNS。

## 关于
PillowDNS是一款支持广告去除的DNS，基于dnsmasq、[doh-server](https://github.com/m13253/dns-over-https)和Nginx搭建。    
通过PillowDNS，你可以绕过营运商的层层封锁，安全、快捷的到达你想去的地方。

### 广告去除
PillowDNS通过拒绝解析/劫持特定的广告域名到localhost以达到屏蔽广告的效果。      
你可以在该项目的Release界面中查看新增的屏蔽域名。

### 安全
PillowDNS支持DoH和DoT。拒绝运营商劫持，让解析更加安全。

## 连接
通过IP连接：154.12.37.236    
通过DoH连接：https://dns.loccc.top/     
通过DoT连接：dns.loccc.top     

## 更改DNS
如果您想要在您的设备上使用PillowDNS，请按照下列方式更改您的DNS设置：

### Linux
#### Android
##### 更改WLAN DNS
1. 进入WLAN设置。
2. 长按你正在使用的WLAN，选择修改网络。
3. 将IP选项由DHCP改为静态。
4. 填入路由器网关、路由器分配的原IP和网络前缀长度后，在DNS1内填入PillowDNS的IP，DNS2可留空或填入其他DNS。

##### 更改全局DNS（仅Android 9+）
1. 进入网络和互联网设置。
2. 将私人DNS改为`私人DNS提供商主机名`，并填入PillowDNS的DoT地址。

##### 更改v2rayNG DNS（仅Android 4+）
1. 进入v2rayNG设置。
2. 将VPN DNS改为PillowDNS的IP。

#### 其他发行版
1. 使用nano/vim/vi/micro/gedit在root用户下更改`/etc/resolve.conf`。

### Unix
同其他Linux发行版。

### Windows
（自行百度，太久没用Windows早忘光了）

## 捐赠
PillowDNS是一款非营利甚至非盈利的DNS，完全自费维护。     
如果你想要支持PillowDNS的稳定运行，请捐助我们。     
     
![AliPay](https://zzchumo.github.io/zzChat-Online/alipay.jpg)
