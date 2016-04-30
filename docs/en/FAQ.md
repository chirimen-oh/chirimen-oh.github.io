---
layout: doc_toc_en
title: FAQ
---
# CHIRIMEN FAQ
 
## Q. CHIRIMENとは何ですか
CHIRIMEN はセンサーやアクチュエーターなどの物理デバイスを Webブラウザ技術だけで制御することができる開発環境で、ボードコンピュータとその上で動作するソフトウェアを含めた総称です。  
ボードコンピュータとしてのハードウェア、その上で動作するウェブブラウザ(現在は Boot to Gecko を使用) ソフトウェア、センサーや物理デバイスを ウェブアプリ・JavaScript から制御するための WebGPIO や WebI2C といった低レベルデバイス API の実装などが含まれており、CHIRIMEN Open Hardwareコミュニティによって開発され、CHIRIMEN というコードネームがつけられました。  
CHIRIMEN に関連するハードウェアととソフトウェアのソースコードは、オープンソースとして公開されます。

## Q. What is the capability of CHIRIMEN? 
CHIRIMEN can operate the contents within a screen, and a real physical device only with the technique of a web browser altogether simultaneously. 

## Q. Tell me about CHIRIMEN's hardware.
Its hardware is an embeddable board computer with interfaces such as I2C and GPIO etc., and it assumes web browsers ) currently it is Boot to Gecko (B2G) ) as a prerequisite. The "CHIRIMEN Board Computer CMN2015-1" by the CHIRIMEN Open Hardware community is the first prototype hardware for CHIRIMEN.

## Q. What has happened to the software part of CHIRIMEN? / What is OS of CHIRIMEN? 
Currently, it is Boot to Gecko (B-2G). It is not Firefox OS. It supports Boot to Gecko 2.5 currently.  Refer to the following clause for the reason which is not Firefox OS.

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
Yes. However, assistance in particular of a software is not expectable from a community in that case. Moreover, "Based on CHIRIMEN technology" cannot be displayed, either. 

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

## Q. オープンソースとして公開されるソースコードには何が含まれますか
ソースコードには、ハードウェアを製造するための設計情報と、同ハードウエア上で動作するBoot to Gecko OS ソフトウェアの両方が含まれます。

## Q. ハードウェアのソースコードとして何が提供されますか
回路図、プリントパターン、部品配置図、部品表などが公開されます。またそれらは再生産を容易にするために求められる電子ファイルの形式で提供されるでしょう。

## Q. CHIRIMEN のハードウェアは誰が製造できるのですか
製造自体はだれでも自由に行うことができます。ただし、それに CHIRIMEN という名称を付けて販売するには、CHIRIMEN Open Hardware コミュニティによる承認が必要です。ただし、CHIRIMENという製品名で販売することはできません。詳しくは[こちらのライセンス情報](https://chirimen-oh.github.io/license/)を参照ください。

## Q.CHIRIMEN の販売は誰ができるのですか
CHIRIMEN Open Hardwareコミュニティによる承認が得られた業者が販売できます。承認を得るために必要な手順や条件は[こちらのライセンス情報](https://chirimen-oh.github.io/license/)に記述されています。

## Q. CHIRIMEN はどのようなライセンスで公開されますか
ハードウェアとソフトウェア双方をカバーする[CHIRIMEN ライセンス](https://chirimen-oh.github.io/license/)に基づき公開されます。ライセンスは現在法的レビュー中となっており、ソースコード公開時に同時に公開予定です。

## Q. CHIRIMEN ブランドポリシーはどこにありますか
[CHIRIMEN ライセンス](https://chirimen-oh.github.io/license/)を参照ください。

## Q. CHIRIMEN は Mozilla の製品ですか
いいえ。CHIRIMEN は CHIRIMEN Open Hardwareコミュニティがプロトタイプとして開発している ウェブブラウザエンジンを搭載したボードコンピュータとそのソフトウェアであり、Mozilla の製品ではありません。

## Q. CHIRIMEN Open Hardware は Mozilla のプロジェクトですか
いいえ。CHIRIMEN Open Hardware は Mozilla Corporation や Mozilla Foundation によるプロジェクトではありません。Mozilla Factoryと呼ぶ枠組みの中の CHIRIMEN Open Hardwareコミュニティによって運営されているプロジェクトです。

## Q. Mozilla Factory とは何ですか
Mozilla Factory は Mozilla Japan が中心となってオープンソースによるモノづくりを学ぶ場所として 2012 年に立ち上げた枠組みですです。 CHIRIMEN Open Hardwareは Mozilla Factory の中のコミュニティによって進められているプロジェクトになります。   
[詳しくはこちらをご覧下さい](http://en.mozillafactory.org/about)

## Q. CHIRIMEN Open Hardware プロジェクト(コミュニティ） とは何ですか
さまざまなモノがコンピュータネットワークで繋がる未来の社会において、ヒトとモ ノがウェブを介して互いに協調しあえる環境を作り、“ウェブらしさ”とは何か、ウェブを介したよりよいヒト・モノの関係とは何かを考えていくプロジェクトです。  
[詳しくはこちら](http://en.mozillafactory.org/post/10861582384/open-hardware-project)をご覧下さい:

## Q. CHIRIMEN と CHIRIMEN Open Hardware の関係、違いは何ですか
CHIRIMEN は CHIRIMEN Open Hardware コミュニティによる開発成果の一つです。CHIRIMEN Open Hardware コミュニティではCHIRIMEN をはじめとした、Web 技術をベースとしたオープンなハードウェアとソフトウェアの開発を進めています。その最初の開発成果はがCHIRIMENと呼ばれています。CHIRIMEN Open Hardware プロジェクトの設立趣旨は前項を参照ください。

## Q. CHIRIMEN Open Hardware では何をオープンにしているのですか
ボードコンピュータを製造するために必要な情報をオープンにしています。それはハードウェアの製造に必要な情報とそこで稼働するオペレーティングシステムソフトウェアを含みます。また、ソースコードだけでなく開発や API の議論のプロセスもオープンにしています。

## Q. CHIRIMEN Open Hardware コミュニティには誰が参加できるのですか
個人だけでなく、任意の組織・団体が参加できます。

## Q. CHIRIMEN Open Hardware communityに参加したい場合はどうしたらよいですか。
[CHIRIMEN Open Hardware Facebook グループ](https://www.facebook.com/groups/mozopenhard/)への参加や[CHIRIMEN Open Hardware Google group](https://groups.google.com/forum/#!forum/chirimen-oh) を通してコミュニへ参加できます。


