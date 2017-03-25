---
layout: doc_toc_ja
title: firmware update guide for mac(Virtualbox)
---
# Firmware Update Guide for mac(Virtualbox)

## 概要
CHIRIMENボードコンピュータのオペレーティングシステムをアップデート手順を解説します。ホストPCのOSはmac(Virtualbox)です。

## 必要な機材
- CHIRIMENボード本体
- HDMIモニター (CHIRIMENの出力を表示するため)
- HDMIケーブル (典型的なCHIRIMENパッケージに添付)
- CHIRIMEN用USB電源ケーブル (典型的なCHIRIMENパッケージに添付)
- USB電源(1A以上の電流供給能力が必要)

### ハードウェア構成図
![chirimen_fwup_conf](../images/chirimen_fwup_conf.jpg)

## Ubuntu 仮想環境構築
### 下記urlからUbuntu 仮想環境 vdi ファイルをダウンロードします。

  - [Ubuntu 仮想環境 vdi ファイル](https://drive.google.com/drive/folders/0B4V6iMhRJyKObjV3bmZDZVN4d1k)

<img src="../images/mac-01.png" width="800px">

### Virtualbox 選択します。
<img src="../images/mac-02.png" width="800px">

### Virtualbox 起動します。
<img src="../images/mac-03.png" width="800px">

### Virtualbox で 仮想環境を新規作成します。
<img src="../images/mac-04.png" width="800px">

<img src="../images/mac-05.png" width="800px">

### ダウンロードした vdi ファイルを選択します。
<img src="../images/mac-06.png" width="800px">

### 仮想環境が出来ました。
<img src="../images/mac-07.png" width="800px">

### 仮想環境の Ubuntu を起動します。
<img src="../images/mac-08.png" width="800px">

### パスワード：「chirimen」と入力します。
<img src="../images/mac-09.png" width="800px">

<img src="../images/mac-10.png" width="800px">

## ステップバイステップガイド
以下、順を追ってインストール手順を説明します。

### Ubuntuでの操作
- Ubuntuの端末（terminal）を起動します。
- 以下の手順は、基本的に端末（terminal）で行います。

### 最新イメージを取得します。
- 下記コマンド実行します。

  ```
  $ wget https://github.com/chirimen-oh/release/releases/download/CMN2015-1/CMN2015-1_B2GOS-2016XXXX.zip
  ```

  ```
  ※2016XXXX：バージョン
  ```
  ![wgetコマンド](../images/linux-02.png)


### 最新イメージを解凍／展開します。
- 下記コマンド実行します。

  ```
  $ unzip CMN2015-1_B2GOS-2016XXXX.zip
  ```

  ```
  ※解凍／展開されるとCMN2015-1_B2GOS-2016XXXX.img が作成されます。
  ```

  ```
  ※2016XXXX：バージョン
  ```
  ![unzipコマンド](../images/linux-03.png)


### CHIRIMEN BoardをPCとディスプレイに接続します。
- OTG と印字されたコネクタにUSBケーブルをPCに接続します。
- HDMI と印字されたコネクタにHDMIケーブルをディスプレイに接続します。

### CHIRIMEN Boardを通常モードで起動します。
- 電源接続し、起動します。
- Virtualbox の USB 設定を行います。
  - Virtualbox VM の Menu -> Devices -> USB
    - 画像のように [ CHIRIMEN Open Hardware chirimen [0222] ] チェックをつけてください
  <img src="../images/mac-11.jpg" width="800px">
  - Virtualbox VM の Menu -> Devices -> USB -> USB Setting
  <img src="../images/mac-12.jpg" width="800px">
  - USB デバイス 追加設定画面が表示されます。
  - "+"アイコンをクリックします。
  <img src="../images/mac-13.jpg" width="800px">
  - 先程と同様にが表示されます。
  - 画像のように [ CHIRIMEN Open Hardware chirimen [0222] ] チェックをつけてください
  <img src="../images/mac-14.jpg" width="800px">
  - USB デバイスが追加されると画像のようになります。
  <img src="../images/mac-15.jpg" width="800px">

### CHIRIMEN Boardを書き込みモードで起動します。
- 電源接続を一度、抜きます。
- Recover Mode Switchを押しながら電源接続します。
- Recover Mode Switchを押した状態で、ゆっくり10数えます。
- Virtualbox の USB 設定を再度行います。
  - Virtualbox VM の Menu -> Devices -> USB
    - 画像のように [ Unknown device 2207:300A [0100] ] チェックをつけてください
  <img src="../images/mac-17.jpg" width="800px">
  - Virtualbox VM の Menu -> Devices -> USB -> USB Setting
  <img src="../images/mac-18.jpg" width="800px">
  - USB デバイス 追加設定画面が表示されます。
  <img src="../images/mac-19.jpg" width="800px">
  - "+"アイコンをクリックします。
  - 先程と同様にが表示されます。
  - 画像のように [ Unknown device 2207:300A [0100] ] チェックをつけてください
  <img src="../images/mac-21.jpg" width="800px">
  - USB デバイスが追加されると画像のようになります。
  <img src="../images/mac-22.jpg" width="800px">




### CHIRIMEN Boardをファーム書き込みコマンドを実行します。
- 下記コマンド実行します。
  - sudo 無しでも実行できますが、確実性を上げるためにsudoを用いています。
  - 本手順では、画像の様にCHIRIMEN-toolsフォルダ内にimgファイルがあるものとして、手順を進めます。

  ```
  $ sudo ./Linux_Upgrade_Tool_v1.21/upgrade_tool uf CMN2015-1_B2GOS-20170301.img
  ※20170301：バージョン
  ```


  <img src="../images/mac-23.png" width="800px">
  <img src="../images/mac-24.png" width="800px">

### CHIRIMEN Boardの再起動待ち
- 以上でアップデート工程は完了しました。
  <img src="../images/mac-25.png" width="800px">
