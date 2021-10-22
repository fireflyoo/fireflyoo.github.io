---
title: "Conemu+plink打造还算完美的ssh client"
date: 2021-10-19
author: fireflyoo
draft: false
---
## plink是什么？

plink就是一个windows上的ssh client，putty是GUI版本，plink是命令版本

**不过现在Win10上已经自带ssh了，配合Windows Terminal**

除了没有plink免输密码的-pw选项，其实也挺好用。

## 下载地址

- [plink修改版][1]
- [Conemu官网][2]

## 配置
然后在Conemu里新建一个Task
```
chcp 65001 && plink username@host.name -pw password -P 22

```

## 尚未修复的BUG

plink修改版修复了原版的Bug(相对于Conemu来说，在自家的Putty上是没问题的)

还有个Bug是终端只能适配刚启动时的窗口大小，不能改。这个Bug一直没改


    Plink survives on Ctrl+C and is transmitted the keypress to server instead.
    Keyboard fixes.
        Arrows are working: Up/Down for history, Left/Right for moving in prompt.
        Esc keypress transmitted to server (Vim and so on).
    ssh terminal size is properly initialized on startup (on-the-fly resize is not supported yet).


[1]:https://github.com/Maximus5/plink/releases/download/v151109/plink-151109.7z
[2]:https://conemu.github.io/