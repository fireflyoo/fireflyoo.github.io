---
title: "Hugo编译小记"
date: 2021-10-13T05:15:48Z
draft: false
---
## 准备好编译环境
我的硬件是R4S,CPU是arm64架构，系统装的是openwrt21.02
我试过Openwrt官方库里的gcc是不能编译出extended版本的Hugo的。
需要下载第三方的编译工具
我是从[这里][1]发现下载地址的。

```bash
wget https://musl.cc/aarch64-linux-musl-native.tgz
tar zxvf aarch64-linux-musl-native.tgz
````
编辑`/etc/profile`或`~/.profile`里的PATH
弄好git和go
我怕空间不够用，全装在另外一个分区(/opt)了
所以还要编辑/etc/opkg.conf添加如下行

```
dest opt /opt
```
然后安装
```bash
opkg install git-http -d opt
opkg install golang -d opt
```
装完后记得添加执行路径到profile的path里，或者添加符号链接到/usr/bin下
## 静态编译
```bash
git clone https://github.com/gohugoio/hugo.git
cd hugo
CGO_ENABLED=1 CC=aarch64-linux-musl-gcc CXX=aarch64-linux-musl-g++ \
go install --tags extended -ldflags '-s -w --extldflags "-static -fpic"'
```

[1]:https://github.com/eyasliu/blog/issues/27

