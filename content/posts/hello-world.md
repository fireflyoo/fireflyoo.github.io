---
title: "hugo后台管理"
date: 2021-10-15
author: fireflyoo
---
准备用cgi远古魔法弄一个网页端后台处理脚本
不然总是要进ssh手动执行hugo生成本地静态页面，挺麻烦的。还有要弄个一键push到github的cgi脚本。
任务列表

    1.  cgi脚本，用来执行hugo，生成本地静态页面
    2.  cgi脚本，用来执行git push，同步源码到github
我发现lighttpd的webdav好像不支持符号链接？
任务一基本完成，现在可以通过/hugo.cgi魔法直接发布文章，编辑文章通过webdav.