---
layout: doc_ja
title: Index Page
---
# ボードコンピュータ　コネクタ配置
CHIRIMENボードコンピュータのコネクターおよびスイッチの配置を紹介します。

## コネクタ配置図

![chirimen_board_front](../images/chirimen_board_front.jpg) 

![chirimen_board_back](../images/chirimen_board_back.jpg) 

1. USB OTG  
開発用ホストコンピュータを接続するためのMicroUSB Type BのUSBポートです
1. Micro HDMI type video connector  
HDMIビデオモニタを接続するためのコネクタです
1. USB UART
この端子は、多くのケースで使用しません。SoCが搭載するUARTxポートをUSBに変換した信号が出力されます。
1. 5V power in  
5Vの電源の入力コネクタです。外径2.5mmのDCコネクタです。
1. USB HOST  
ネットワークアダプタやポインティングデバイスなどを接続するためのUSB Type Aポートです。
1. Recover mode switch  
ファームウェアのアップデートのために主に使用するスイッチです。
1. CN1 (Connector1)  
GPIO, I2C, UART, SPIなどの信号が集約されたスルーホールの多用途入出力端子です。端子の信号配置図は後の章を参照してください。
1. CN2  (Connector2)  
もうひとつの多用途入出力端子です。
1. Micro SD Slot  
MicroSDスロットです。2016年2月現在まだOSはサポートしていません。

## 多用途入出力端子のピン配置

||CN1 (Connector1)| |CN2 (Connector2)|
|------------|:--:|:----------:|:----------------:|
|Number|Description| |Description
|1|GND| |GND|
|2|I2C-2 SDA| |GND|
|3|I2C-2 SCL| |GND|
|4|UART-3 RX| |GND|
|5|UART-3 TX| |Audio L out|
|6|ADC-0 in| |Audio R out|
|7|SPI-0 CS| |Audio L in|
|8|SPI-0 CLK| |Audio R in|
|9|SPI-0 RX| |Audio GND|
|10|SPI-0 TX| |PWM-0|
|11|SPI-1 CS| |I2C-0 SCL|
|12|SPI-1 CLK| |I2C-0 SDA|
|13|SPI-1 RX| |UART-0 TX|
|14|SPI-1 TX| |UART-0 RX|
|15|GND| |GPIO-6 A1|
|16|VCC 3.3V| |Power ON|
|17|VCC 3.3V| |GND|
|18|VCC 5V| |VSYS 5V|