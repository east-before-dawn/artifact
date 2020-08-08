# VMware 共享文件夹







```bash
vmware-hgfsclient # 命令查看当前有哪些共享的目录
sudo apt-get install open-vm-dkms
mount  -t vmhgfs .host:/VMware_share /mnt/hgfs  # 挂载共享文件
```

