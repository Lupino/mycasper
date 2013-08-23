mycasper
========

让 Ubuntu 在 u 盘 上更好的保存状态

Ubuntu 12.04 上测试成功

Usage:

    将 casper* 放在 initrd.lz scripts 目录下，替换原来的 casper*
    helpers 是放在 LIVE_MEDIA_PATH 下面的。

Grub.cfg:

    linux /boot/Ubuntu/vmlinuz boot=casper locale=zh_CN.UTF-8 copy-on-write-path=/copy-on-write live-media-path=/boot/Ubuntu # quiet splash --
    initrd  /boot/Ubuntu/initrd.lz
