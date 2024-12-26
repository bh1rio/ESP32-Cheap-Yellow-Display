# 小黄屏上的MicroPython 

## 安装Micropython

[适用于 ESP32 的 MicroPython 标准版本](https://micropython.org/download/ESP32_GENERIC/)在这个模块上运行良好。

## 附加库

显示屏和触摸屏的驱动程序可在[micropython - ili9341](https://github.com/rdagger/micropython-ili9341)项目中找到。

## 示例代码

查看`demo.py`，其中的代码展示了如何使用：

* ✅ 显示和背光
* ✅ RGB LED
* ✅ SD card
* ✅ 光照传感器
* ✅ t触屏

尚未测试：

* ❓ I2S 音频输出（[MicroPython 中应原生支持](https://docs.micropython.org/en/latest/library/machine.I2S.html)）

译者注：

* 上述测试需要使用原生ESP32的MicroPython。如果使用的是带有`lvgl`的MicroPython，内置的ili9341模块会优先生效，切会有过时提醒，并报错无法找到`Display`。
* 上述测试译者未测试。译者手里没有CYD或者CYD2,译者手里只有一块全动电子出品的3.2寸改良版CYD，其显示芯片是st7789p3。
* 有时间的话，译者争取添加针对全动3.2改良版的演示代码。