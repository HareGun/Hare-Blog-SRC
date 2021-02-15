---
title: WSL 安装
---


https://docs.microsoft.com/zh-cn/windows/wsl/install-win10


给WSL配置固定IP
wsl -d Ubuntu-20.04 -u root ip addr add 192.168.159.16/24 broadcast 192.168.159.255 dev eth0 label eth0:1
netsh interface ip add address "vEthernet (WSL)" 192.168.159.10 255.255.255.0
然后，可用192.168.159.16访问Ubuntu，192.168.159.10访问Win10。
