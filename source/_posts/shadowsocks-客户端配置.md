---
title: shadowsocks 客户端配置
date: 2017-07-03 13:56:32
tags:
---
### 什么是shadowsocks
shadowsocks是一种基于Socks5代理方式的网络数据加密传输包程序，并采用Apache许可证、GPL、MIT许可证等多种自由软件许可协议开放源代码。源码存放在[<font color=#0000ff>github</font>](https://github.com/shadowsocks)上，shadowsocks分为服务器端和客户端，通过微信扫描文章末尾二维码可以获取shadowsocks服务端账户和密码。本教程主要介绍shadowsocks客户配置方法。  

### 客户端程序下载
shadowsocks支持客户端有：  
* windows  &nbsp; &nbsp; [<font color=#0000ff>github 下载地址</font>](https://github.com/shadowsocks/shadowsocks-windows/releases)
* mac &nbsp; &nbsp;  [<font color=#0000ff>  github 下载地址</font>](https://github.com/shadowsocks/shadowsocks-iOS/releases)
* android  &nbsp; &nbsp;  [<font color=#0000ff>  github 下载地址</font>](https://github.com/shadowsocks/shadowsocks-android/releases)
* ios  app商店搜Wingy  

### windows 使用说明
#### 安装shandowsocks客户端
windows 桌面任务栏打开隐藏按钮看到shandowsocks的
{% img /img/20170704/1.png 1394 956  %}
右击纸飞机图标----服务器----编辑服务器
{% img /img/20170704/2.png 1394 956  %}
{% img /img/20170704/3.png 1394 956  %}
输入：
* 服务器地址
* 服务器端口
* 密码
* 加密选择“aes-256-cfb"
* 备注随便填  

#### 安装chrome插件Proxy SwitchyOmega
下载地址：  
&nbsp; &nbsp; [<font color=#0000ff>点击直接下载Proxy SwitchyOmega(extension_2_4_6.crx)</font>](https://www.crx4chrome.com/down/998/cdn/)
Chrome 商店地址：[<font color=#0000ff>Proxy SwitchyOmega</font>](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif)
#### 浏览器安装
1. chrome 浏览器
在浏览器地址栏输入：chrome://extensions/
将下载的插件拖入浏览器中
{% img /img/20170704/4.png 1357  694  %}   
2. 360浏览器直接将插件拖拽到浏览器中  
3. 安装成功后浏览器的菜单栏多一个环形的图标
{% img /img/20170704/7.png 442  201  %}   
#### 参数配置
右击浏览器菜单上环形插件选择选项
{% img /img/20170704/8.png 1363 652  %}  

参数配置如下图
``` bash
点击红色标记1按钮
红色标记2 参数按图中一样
点击红色标记3 应用选项 保存参数
```
{% img /img/20170704/9.png 1365  650 %} 
``` bash
点击红色标记4按钮
点击红色标记5按钮
```
{% img /img/20170704/10.png 1363  648 %} 
``` bash
点击红色标记6按钮
红色标记7 出输入：https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt 
	这是大陆防火墙过滤名单地址，google, facebook等网站都在名单中，名单会定期更新
点击红色标记8 ，下载防火墙过滤名单，定期点击此按钮更新名单
红色标记9处会下载防火墙过滤的名单，
点击红色标记3 应用选项 保存参数
```
{% img /img/20170704/11.png 1361 647 %} 
#### 选项说明
{% img /img/20170704/12.png 258 300 %} 
``` bash
“直接连接”  访问网站不用代理
“系统代理”  访问网站使用系统的代理，系统代理一般在浏览器设置中配置
“proxy”		访问网站全部使用代理
“auto switch” 根据防火墙名单判断是否使用代理，如：访问百度是直接访问，访问google则使用代理
“添加条件” 设置当前网站是直接访问获取通过代理访问，设置成功后，只要访问该网站就会使用设置的方式访问
建议选择auto switch 因为通过代理访问国内的网站会变慢。如果遇到auto switch 不能访问的网站，选择添加条件设置为使用代理访问
```
微信扫描二维码获取shadowsocks免费账户


