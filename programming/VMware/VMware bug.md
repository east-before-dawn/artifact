# VMware bug

## 目录

[TOC]

## 虚拟机 ubuntu ens32 没有分配到 IP(dhcp)

在常规配置NAT网络，虚拟网络编辑器 -> 还原默认设置，还不能正常连接网络，虚拟机内有线连接丢失的情况下。 

dhcp自动分配IP不成功，分配了169.254网段IP

应该检查 /etc/network/interfaces

```
auto lo
iface lo inet loopback

auto ens32
iface ens32 inet dhcp
```

### 自动获取dhcp

```
auto ens32  
iface ens32 inet dhcp  
---
auto eth0  
iface eth0 inet dhcp 
```

配置完还是没有dhcp自动分配的 ip

手动配置

```
sudo dhclient ens32
ifconfig ens32
```

### 静态设置IP

```
auto eth0  
  
iface eth0 inet static  
address 192.168.80.129 #ip地址  
netmask 255.255.255.0  #子网掩码  
gateway 192.168.80.2  #网关  
```

### ipconfig

```shell
ipconfig /release # 回车,释放目前已获取的ip
ipconfig /renew   # 回车 重新获取新的ip
ipconfig /all     # 查看ip地址
```



或者关闭VMware服务，让其重新分配IP

