mycasper
========

让 Ubuntu 在 u 盘 上更好的保存状态

Usage:

    将 casper* 放在 initrd.lz scripts 目录下，覆盖原来的 casper*
    helpers 是放在 LIVE_MEDIA_PATH 下面的。

Grub.cfg:

    linux /boot/Ubuntu/vmlinuz boot=casper locale=zh_CN.UTF-8 copy-on-write-path=/copy-on-write live-media-path=/boot/Ubuntu # quiet splash --
    initrd  /boot/Ubuntu/initrd.lz
