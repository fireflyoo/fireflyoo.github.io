---
title: "小新Pad Pro 2020(Lenovo_TB_J706F) BL解锁+ROOT指南"
date: 2026-01-22
author: fireflyoo
---
参考：https://wiki.postmarketos.org/wiki/Unlocking_Bootloaders/Lenovo_ZUI
## 解锁BL

联想ZUI官网申请完unlockBL后，并不会发邮件给你解锁文件sn.img..
1. 需要自己下载
下载地址为：
    http://cdn.zui.lenovomm.com/developer/tabletboot/SN-NUMBER/sn.img, where SN-NUMBER is the serial number of your device.
SN-NUMBER为八位数，可以查看平板背面或者开启adb通过`adb devices`查看，`adb devices`显示出来的设备名既是SN码..
2. Reboot into fastboot mode.
3. Flash the image using `fastboot flash unlock sn.img`
4. Unlock using `fastboot oem unlock-go`. You need to quickly confirm using the volume buttons. If you get the error "Prohibit unlock operation", it's because you forgot to enable "OEM unlocking" in "Developer options".
5. Check if bootloader is now unlocked `fastboot getvar` unlocked

以下为平板进入各种急救模式的按键：
- EDL Mode: Hold down Volume Up, then connect the device to a computer with an USB cable.
- FFBM Mode: Power on the device with both Power and Volume Up buttons.
- Fastboot Mode: Power on the device with both Power and Volume Down buttons.
- Recovery Mode: Boot into Fastboot mode and select recovery using the Volume/Power buttons.
## 刷机
我用的镜像是[ZUI_12.6.133](https://mirrors-obs-1.lolinet.com/firmware/lenowow/2020/Tab_P11_Pro/TB-J706F/TB-J706F_CN_WIFI_USER_Q00010.0_R_ZUI_12.6.133_ST_210813_qpst.zip)
刷机工具我用的是官方提供的联想[平板自助刷机工具](https://iknow.lenovo.com.cn/detail/424556)
这工具会偷偷在C盘生成一个工具，并在你关闭它后偷偷删除。
我只好在它偷偷生成的时候复制里面的命令行工具，并替换里面的刷机镜像image，不然它只会刷最新版的ZUI（也不是不行，不过我没试过新版是否也可以正常解锁BL，毕竟我已经解锁了）

如何想刷镜像库里的国际版需要改区域码，不然刷完后会跳出一个警告，却进不了系统..可以参考[这篇文章](https://www.bilibili.com/opus/717652433632755731)。
注意国际版没法用sn.img解锁BL..
## ROOT
root工具我用的是magisk,用magisk修补上文镜像里的boot.img再通过`fastboot flash boot boot-modified_by_magisk.img`刷入修改后的boot.img就好了。
