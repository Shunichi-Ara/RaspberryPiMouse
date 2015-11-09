# RaspberryPiMouse

This repository has the source code and kernel objects
for the Raspberry Pi mouse.

## How to install the device driver

```
$ git clone https://github.com/rt-net/RaspberryPiMouse.git
### check the kernel version
$ uname -r
4.1.6-v7+
###choose a directory based on your RPi and the kernel version
$ cd RaspberryPiMouse/lib/Pi2B+/4.1.6-v7+/
###install the kernel object
$ sudo insmod rtmouse.ko
```

## ドライバの導入の際の注意

以下の設定を確認ください。
raspi-configコマンドで設定します。

* SPI機能を「入」にする。
* Device Tree機能を「切」にする。

## 日経Linux連載

連載（Raspberry Piで始めるかんたんロボット製作）で上田氏が書いた
シェルスクリプトは下記にあります。

https://github.com/ryuichiueda/RPiM
