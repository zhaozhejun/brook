# Brook 端口转发 一键管理脚本
原 逗比 Brook 端口转发 一键管理脚本 修改版
增加对动态域名的支持，开启监控后自动更新域名IP

# ECIAP 再修改分支
尝试修复 https://github.com/yulewang/brook/issues/4 此问题的分支

- 在使用此脚本前Linux服务器应先进行以下操作
```
For RHEL / CentOS:
sudo yum install bind-utils -y

For Debian / Ubuntu
sudo apt-get install dnsutils
```
不然可能会产生如下报错
```
./brook-pf-mod.sh: line 706: dig: command not found
```
