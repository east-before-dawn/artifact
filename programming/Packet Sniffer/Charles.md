# Charles

<img src="https://user-gold-cdn.xitu.io/2017/12/13/1604e05285fa5e14?imageView2/0/w/1280/h/960/format/webp/ignore-error/1" align='left' style="zoom:50%;" />

## 目录

[TOC]

## Charles代理端设置

### http  socks

Charles  Proxy->Proxy Setting->Proxies, enable transparent HTTP proxying

<img src="Charles.assets/Proxy Settings.png" align='left' style="zoom:80%;" />

### https

Charles  Proxy->SSL Proxying Settings

<img src="Charles.assets/SSL Proxying Settings.png" align='left' style="zoom:80%;" />

#### install Charles root certificate

Charles  Help->SSL Proxying->Install Charles Root Certificate



## 手机端的设置代理(IOS/Android)

设置 Charles 所在PC的IP地址和代理端口 8888

浏览器地址栏键入chls.pro/ssl 下载根证书 或者 Charles  Help->SSL Proxying->Save Charles Root Certificate，手动安装。

<img src="Charles.assets/yeshen proxy setting.png" align='left' style="zoom:50%;" />

### 注意

模拟器安装证书时候会提示设置一个PIN，PIN密码会用于锁屏。



##  android 7.0 问题

Android 7.0 开始，默认的网络安全性配置修改了，具体请阅读官方文档[网络安全性配置](https://developer.android.com/training/articles/security-config)。

网上的帖子描述了，不少的解决方法。但麻烦，除非实在没辙了，不然应该另辟蹊径。

可以通过安卓模拟器（夜神）设置代理，夜神android版本是android 5。



## 参考

- [Android 7.0 以上 Charles 和 Fiddler 无法抓取 HTTPS 包的解决方式](https://johnnyshieh.me/posts/android-7-capture-https-package/)



