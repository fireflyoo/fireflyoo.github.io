---
title: "在Caddy2上配置WebDAV"
date: 2021-10-23
draft: false
---
我是在Termux上运行的,所以路径有点长



因为用到了80端口所以手机需要root,

我的手机是用Magisk ROOT掉的,

权限管理也在Magisk里,需要手动添加Termux到列表里

termux里还需要`pkg install tsu`

caddy的handle命令相当于nignx的location

保存下列内容到当前目录的Caddyfile后,执行`sudo caddy run`就成了

```
:80
root * /data/data/com.termux/files/home/www
file_server
redir /webdav /webdav/
handle_path /webdav/* {
    root * /data/data/com.termux/files/home/webdav
    @notget not method GET

    route @notget {
            # 密码不能为明文，可以使用自带的工具加密：
            # caddy hash-password  --plaintext sdderght
        basicauth {
            name hashed_password_base64
        }
        webdav
    }
    file_server browse
}
# https://caddy.community/t/file-server-basics/8843
# https://github.com/mholt/caddy-webdav
```