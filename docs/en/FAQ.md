---
layout: doc_toc_en
title: FAQ
---
# CHIRIMEN FAQ
 
## Q. CHIRIMENとは何ですか
CHIRIMEN is a development environment that allows to control the physical devices (such as sensors and actuators) only by Web browser technology and includes hardware (board computer) and software on it.
Their implementation includes hardware as a board computer, Web browser software (currently using Boot to Gecko), and low-level device APIs (WebGPIO and WebI2C etc.) to control physical devices by web apps or JavaScript It is developed by CHIRIMEN Open Hardware community and code-named “CHIRIMEN”.
Their hardware and software have been released as open source.

## Q. What is the capability of CHIRIMEN? 
CHIRIMEN can operate the contents within a screen, and a real physical device only with the technique of a web browser altogether simultaneously. 

## Q. Tell me about CHIRIMEN's hardware.
Its hardware is an embeddable board computer with interfaces such as I2C and GPIO etc., and it assumes web browsers ) currently it is Boot to Gecko (B2G) ) as a prerequisite. The "CHIRIMEN Board Computer CMN2015-1" by the CHIRIMEN Open Hardware community is the first prototype hardware for CHIRIMEN.

## Q. What has happened to the software part of CHIRIMEN? / What is OS of CHIRIMEN? 
Currently, it is Boot to Gecko (B2G) OS. It is not Firefox OS. It supports Boot to Gecko 2.5 currently.  Refer to the following clause for the reason which is not Firefox OS.

## Q. What is Boot to Gecko? Does it differ from Firefox OS? 
Boot to Gecko and Firefox OS is the same in code. After fulfilling conditions, such as quality and security, only the product which has obtained the licensing of the brand from Mozilla can use the name of Firefox OS. On occasions when it uses it as OSS without brand licensing, it is Boot to Gecko (B2G). 

## Q. What differs between Raspberry Pi, or other board computers and CHIRIMEN hardwares? 
The hardware of CHIRIMEN is designed on the assumption that a web browser or comfortable operation of Boot to Gecko. Since a browser requires comparatively high graphics performance, it is mainly the feature in contrast to other board computers. 
Therefore, SoC designed for a tablet or STB is carried. 

## Q. What kind of devices and peripherals can CHIRIMEN utilize? 
CHIRIMEN can utilize a cheap and general-purpose sensors and actuators with GPIO or I2C interface. The correspondence to the device using SPI or UART is also considered. Of course, USB can be utilized as an interface for keyboards, pointing devices, and network adapters. 

## Q. Who is making CHIRIMEN? 
It was developed by the CHIRIMEN Open Hardware community. However, that community itself does not do manufacturing and selling of that. 

## Q. Can I reuse only the hardware part of CHIRIMEN? 
Yes. However, assistance in particular of a software is not expectable from a community in that case.

## Q. How to get a CHIRIMEN hardware? 
Currently, the community member uses a small number of prototype for OS development. Purchase may become possible if it is mass-produced by the licensed marker based on the released source code. 

However, such a product has another product name from the constraint by the brand policy of CHIRIMEN. A viewing of "Based on CHIRIMEN technology" may be able to be seen for those products. 

## Q. When is CHIRIMEN put on the market? 
The community guarantees nothing about distribution of hardware. The CHIRIMEN Open Hardware community publishes only the source code of the hardware required for production of the CHIRIMEN, and the software by open source. However, they do not manufacture and sell hardwares. 
It may be sold when the company which manufactures and sells using the information on that open source appears. However, "CHIRIMEN" is not used by the CHIRIMEN license policy as such a product name that a certain company sells. 

## Q. How much is CHIRIMEN? 
A CHIRIMEN Open Hardware community does not manufacture and sell CHIRIMEN. Therefore, a community cannot specify its price. On the other hand, CHIRIMEN was designed manufacture at the same price point as the common board computer for prototypings. On the other hand, CHIRIMEN was designed so that it can manufacture at a comparable or lower price point as the common board computer for prototypings. 

## Q. Can the vendor which manufactures and sells a CHIRIMEN base computor advertize using the logo and word mark relevant to Mozilla or Firefox OS? 
They cannot do it without the grant from Mozilla Corporation. 

## Q. What kind of ones is the license of the source code? 
Mozilla Japan is doing the intellectual property control of the source code as a substitute of the community. Refer to [this information](https://chirimen-oh.github.io/license/) for a copyright and a license. 

## Q. What is contained in the source code released as the open source? 
Both the design information for manufacturing a CHIRIMEN board-computer hardware and the source code of B2G OS software for it are contained in it. 

## Q. What is offered as the source code of the hardware? 
A schematic, a print pattern (Gerber data), a partses layout, a parts list, etc. may be released. And, many of them are offered in the form of the electronic filing required for reproduce easily. 

## Q. Who can manufacture the hardware of CHIRIMEN? 
Anyone can manufacture it freely based on a license. However, "CHIRIMEN" cannot be used as a product name.But, it is possible without a prior authorization to carry out advertisement named "Based on CHIRIMEN technology". Please refer to [this license informtation](https://chirimen-oh.github.io/license/) for details.

## Q. Who can sell CHIRIMEN? 
Anyone can sell it based on [this license](https://chirimen-oh.github.io/license/). Please also refer to the preceding clause.

## Q. Is CHIRIMEN released by what kind of license? 
It is released to the public by the [CHIRIMEN license](https://chirimen-oh.github.io/license/) which covers both a hardware and a software. Please refer to [this](https://chirimen-oh.github.io/license/). 

## Q. Is CHIRIMEN a product of Mozilla? 
No, it is not a product of Mozilla. 

## Q. Is CHIRIMEN Open Hardware a project of Mozilla? 
No. CHIRIMEN Open Hardware is not a project of Mozilla Corporation or Mozilla Foundation. 

## Q. What is Mozilla Factory?
Mozilla Factory is the framework established as an environment for studying making ones by an open source. It was established under initiative of MJ in 2012. CHIRIMEN Open Hardware is the project currently promoted by the community in Mozilla Factory. [Please have a look here for details.](http://en.mozillafactory.org/about)

## Q. What is a CHIRIMEN Open Hardware project or community?
さまざまなモノがコンピュータネットワークで繋がる未来の社会において、ヒトとモ ノがウェブを介して互いに協調しあえる環境を作り、“ウェブらしさ”とは何か、ウェブを介したよりよいヒト・モノの関係とは何かを考えていくプロジェクトです。  
[詳しくはこちら](http://en.mozillafactory.org/post/10861582384/open-hardware-project)をご覧下さい:

## Q. What are the relationship between CHIRIMEN and CHIRIMEN Open Hardware and a difference? 
CHIRIMEN is one of the development productses by a CHIRIMEN Open Hardware community. CHIRIMEN is not one carefully. The first products developed in 2015 is called design ID CMN2015-1. In the CHIRIMEN Open Hardware community, the development of the open hardware and software which used web browser technologies including CHIRIMEN as the base is carried out. Please refer to the preceding clause for the establishment aim of a CHIRIMEN Open Hardware project. 

## Q. What is CHIRIMEN Open Hardware Project doing to open? 
The information required in order to manufacture the board computer of the web browser base which a CHIRIMEN Open Hardware community advocates is released by the open source. It contains both the design information for manufacturing a CHIRIMEN board-computer hardware and the source code of B2G OS software for it are contained in it. Furthermore, not only a source code but a development, investigation of API, and the process of an discussion are made open. 

## Q. Who can participate in a CHIRIMEN Open Hardware community?
Not only an individual but arbitrary organization and party can participate. 

## Q. What should I do to participate in CHIRIMEN Open Hardware community?
You can participate in CHIRIMEN Open Hardware community through the participate to [CHIRIMEN Open Hardware Facebook Group](https://www.facebook.com/groups/mozopenhard/), and [CHIRIMEN Open Hardware Google group](https://groups.google.com/forum/#!forum/chirimen-oh). 
