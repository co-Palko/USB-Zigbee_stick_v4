# USB-Zigbee_stick_v4

Очередная вариация USB stick для работы совместно с zigbee2mqtt.

![alt tag](https://github.com/co-Palko/USB-Zigbee_stick_v4/blob/master/images/render.JPG)
Разработана на основе топологии платы LAUNCHXL-CC1352P-2 и документации от TI (https://www.ti.com/lit/zip/swrc350). 

Оснащена по подобию отладочной платы кнопками BTN-1, BTN-2, Reset. 
Кроме того четырьмя LED индикаторами Power, активности UART, RedLED и GrnLED. 


На плате присутствуют все радиоканалы, как 2.4 GHz (+PA 2.4 Ghz) так и 868 MHz / 915 MHz / 433 MHz.
Производитель заявляет поддержку чипом Thread, Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4g, IPv6-enabled smart objects (6LoWPAN), MIOTY® , Wireless M-Bus, WiSUN® , KNX RF, proprietary systems, SimpleLink™ TI 15.4-Stack (Sub-1 GHz), and Dynamic Multiprotocol Manager (DMM) driver. (https://www.ti.com/lit/gpn/cc1352p)

При необходимости, без переделки платы, на нее можно установить чип CC2652P (pin to pin).

Плата снабжена полноценным разъемом ARM Cortex debug 10pin для прошивки и отладки (при необходимости).
Прошивка осуществляется посредством J-Link либо XDS110. Проверено с J-Link и пакетами Uniflash и J-Flash.
Кроме того возможна прошивка через встроенный UART посредством Bootloader, в режим которого можно войти при запуске с помощью кнопки BTN-1.

Прошивка стандартная от уважемого @Koen Kanters (https://github.com/Koenkk) https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0
разработанная для платы LAUNCHXL. 
 
Обсудить (на русском) можно здесь: https://t.me/zigbeer

# In English 

This stich is developed based on LAUNCHXL-CC1352P-2 board topology and TI documentation (https://www.ti.com/lit/zip/swrc350).

Equipped with BTN-1, BTN-2 and Reset buttons similar to a debug board. In addition, four LED indicators for Power, UART activity, RedLED and GrnLED.

The board contains all radio channels, both 2.4 GHz (+ PA 2.4 Ghz) and 868 MHz / 915 MHz / 433 MHz. The TI claims support for Thread, Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4g, IPv6-enabled smart objects (6LoWPAN), MIOTY®, Wireless M-Bus, WiSUN®, KNX RF, proprietary systems, SimpleLink ™ TI 15.4 -Stack (Sub-1 GHz), and Dynamic Multiprotocol Manager (DMM) driver. (https://www.ti.com/lit/gpn/cc1352p)

If necessary, without altering the board, you can install the CC2652P (pin to pin) chip on it. (This chip can`t equipped sub-GHz channel).

The board is equipped with a full ARM Cortex debug 10pin connector for firmware and debugging (if necessary). The firmware is carried out via J-Link or XDS110. Tested with J-Link and Uniflash and J-Flash packages. In addition, it`s possible to flash through the built-in UART using the Bootloader, which can be entered at startup using the BTN-1 button (DIO15).

Standard firmware made by @Koen Kanters (https://github.com/Koenkk) https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0 developed for the board LAUNCHXL.

You can discuss (in Russian) here: https://t.me/zigbeer
