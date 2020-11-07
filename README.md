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
 - 不然可能会产生如下报错
```
./brook-pf-mod.sh: line 706: dig: command not found
```
- 从github拉取
```
For RHEL / CentOS:
yum install wget -y && wget https://raw.githubusercontent.com/ECIAP/brook/master/brook-pf-mod.sh && chmod +x brook-pf-mod.sh && bash brook-pf-mod.sh
```

# 其他错误
```
Brook v20200909版本无法正常启用，详细原因请查看Brook日志 [注意！我并未尝试其他服务器是否能复现此错误]
如遇到该版本无法正常启用，请回退版本至 v20200801
```
