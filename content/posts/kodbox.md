---
title: "Openwrt下安装KodBox"
date: 2021-10-22
author: fireflyoo
---
[下载地址][1]

- 硬件：R4S -- 4GB内存,ARM64 CPU
- 系统：OpenWRT 21.02 
- Web Server：Nginx 1.19.6
- 后端语言：PHP 8.0.9

需要安装的依赖
用 `opkg install package-name` 安装；
安装前记得 `opkg update` 下。
```
nginx-all-module
php8
php8-fpm
php8-mod-curl
php8-mod-gd
php8-mod-iconv
php8-mod-mbstring
php8-mod-pdo
php8-mod-pdo-sqlite
php8-mod-sqlite3
php8-mod-xml
php8-mod-session
zoneinfo-asia
unzip
```

安装些工具用来[新增用户][2],因为php8-fpm不能用root执行
```
opkg update
opkg install shadow-groupadd
opkg install shadow-useradd
groupadd www-data
useradd http -g www-data
```

编辑 `/etc/php8-fpm.d/www.conf` 修改下用户名
并记住里面listen的值（一般是 `/var/run/php8-fpm.sock`)
```
user = http
group = www-data
```
注释调/etc/php.ini里的
```
;doc_root = "/www"
```

配置/etc/nginx
参考[kod官方文档][3]
```
#核心配置，其他略
location /kodbox {
     alias /opt/usr/share/kodbox;
     index index.php;
      location ~ \.php(.*)$ {
        fastcgi_split_path_info  ^(.+\.php)(.*)$;
        fastcgi_param  PATH_INFO $fastcgi_path_info;
        fastcgi_param SCRIPT_FILENAME $request_filename;
        fastcgi_pass unix:/var/run/php8-fpm.sock;
        include fastcgi_params;
    }
 }
```
然后打开http://openwrt.lan/kodbox应该就能进入了

[1]:https://kodcloud.com/download/
[2]:https://oldwiki.archive.openwrt.org/doc/howto/secure.access
[3]:http://doc.kodcloud.com/v2/#/help/pathInfo?id=nginxapache%e6%94%af%e6%8c%81path_info%e6%a8%a1%e5%bc%8f
