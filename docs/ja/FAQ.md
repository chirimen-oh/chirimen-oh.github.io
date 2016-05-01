---
layout: doc_toc_ja
title: FAQ
---
# CHIRIMEN FAQ
 
## Q. CHIRIMENとは何ですか
CHIRIMEN はセンサーやアクチュエーターなどの物理デバイスを Webブラウザ技術だけで制御することができる開発環境で、ボードコンピュータとその上で動作するソフトウェアを含めた総称です。  
ボードコンピュータとしてのハードウェア、その上で動作するウェブブラウザ(現在は Boot to Gecko を使用) ソフトウェア、センサーや物理デバイスを ウェブアプリ・JavaScript から制御するための WebGPIO や WebI2C といった低レベルデバイス API の実装などが含まれており、CHIRIMEN Open Hardwareコミュニティによって開発され、CHIRIMEN というコードネームがつけられました。  
CHIRIMEN に関連するハードウェアととソフトウェアのソースコードは、オープンソースとして公開されます。

## Q. CHIRIMEN では何ができるのですか
CHIRIMEN では、バーチャルな画面内でのコンテンツとリアルな物理デバイスであるモノを同時に全て Webブラウザの技術だけで操作可能です。

## Q. CHIRIMENハードウェアについて知りたい
CHIRIMENハードウエアは、I2CやGPIOなどのインターフェースを持つ組み込みボードコンピュータです。
それはウェブブラウザ(現在はB2G OS)が適切に動作することを必要条件として想定しています。
CHRIMENボードコンピュータ デザインID CMN2015-1はCHIRIMEN Open Hardwareコミュニティが試作した最初のCHIRIMENハードウェアです。

## Q. CHIRIMEN のソフトウェア部分はどうなっていますか？/ CHIRIMEN のOS は何ですか
現在はBoot to Gecko(B2G) です。Firefox OS ではありません。現在Boot to Gecko 2.5 に対応しています。 Firefox OS ではない理由は次項を参照ください。

## Q. Boot to Gecko とは何ですか。Firefox OS とは違うのですか。
Boot to Gecko と Firefox OS はコード的には同じモノです。品質やセキュリティなどの条件を満たした上で、Mozilla からブランドの使用許諾を得ている製品だけが Firefox OS 搭載を謳えます。ブランド使用許諾無しで OSS として使用する場合は Boot to Gecko(B2G) になります。

## Q. CHIRIMEN のハードウェア (CBC) は Raspberry Pi や他のボードコンピュータと何が違うのですか。
CHIRIMEN のハードウェアはウェブブラウザもしくはBoot to Gecko の快適な動作を前提に設計されています。ブラウザは比較的高いグラフィックス性能を要求しますので、おもにそれが他のボードコンピュータに対する特徴です。そのため、タブレットやSTBのために設計されたSoCが搭載されています。

## Q. CHIRIMEN はどのようなデバイスと組み合わせて利用できますか
市場にたくさん出回っている、汎用のGPIO や I2C インターフェースを持ったセンサーやアクチュエータが利用できます。SPI や UART を用いるデバイスへの対応も検討されています。もちろん、USBはキーボードやポインティングデバイス、ネットワークアダプタのためのインターフェースとして利用可能です。

## Q. CHIRIMENは誰が作っているのですか
CHIRIMEN Open Hardware コミュニティによって開発されました。しかし製造販売をコミュニティが行うわけではありません。

## Q. CHIRIMENボードコンピュータのハードウェア部分だけを再利用できますか
オペレーティングシステム・ウェブブラウザエンジンとして CHIRIMEN Open Hardware コミュニティが規定したソフトウェア（現在はBoot to Gecko）以外を使用せずにボードコンピュータを製造や利用することは可能です。ただしコミュニティからソフトウェアのサポートを期待することはできないでしょう。

## Q. CHIRIMENボードコンピュータのハードウェアを入手したいのですが、どうすればよいですか。
現在は、少量の試作版をコミュニティメンバーが開発用に使っているのみになります。公開されたソースコードをもとに、ライセンスを受けた製造業者によって量産された場合は、広く購入可能になると思われます。しかし、その場合でもCHIRIMENのブランド名は製品名に使う事はできないので、他の名称での販売となるでしょう。それらの製品には、「Based on CHIRIMEN technology」の表示を見ることができるかもしれません。

## Q. CHIRIMEN はいつ発売されるのですか
未定です。CHIRIMEN Open Hardware コミュニティでは CHIRIMEN の作成に必要なハードウェア及びソフトウェアのソースコードをオープンソースとして公開しますが、ハードウェアの製造販売は行いません。  
ハードウェア(ボードコンピュータ)の製造情報はすべてオープンソース化されており、その情報を用いて製造販売おこなう企業が現れれば販売されるでしょう。ただし、企業は販売時に製品名に"CHIRIMEN"を使う事はできません。"Based on CHIRIMEN technology"の表記を使って製品を説明することが可能です。

## Q. CHIRIMEN はいくらで手に入るのですか
CHIRIMENの製造販売は CHIRIMEN Open Hardwareコミュニティは行いません。よってコミュニティとして値段を明示することはできません。一方、一般的なプロトタイピング用ボードコンピュータと同等以下の価格で製造・入手できるものとして CHIRIMEN は設計されました。

## Q. CHIRIMEN を製造・販売するベンダーが、Mozilla やFirefox OS に関連するロゴやワードマークを利用して宣伝することはできますか？
Mozilla Corporationによる別途の承諾なしに、それを行うことはできません。

## Q. ソースコードのライセンスはどのようなものですか
CHIRIMEN Open Hardware コミュニティによるソースコードの知財管理はコミュニティに代わりMozilla Japan が行っています。著作権やライセンスは[こちらのライセンス情報](https://chirimen-oh.github.io/license/)を参照ください。

## Q. オープンソースとして公開されるソースコードには何が含まれますか
ソースコードには、ハードウェアを製造するための設計情報と、同ハードウエア上で動作するBoot to Gecko OS ソフトウェアの両方が含まれます。

## Q. ハードウェアのソースコードとして何が提供されますか
回路図、プリントパターン、部品配置図、部品表などが公開されます。またそれらは再生産を容易にするために求められる電子ファイルの形式で提供されるでしょう。

## Q. CHIRIMEN のハードウェアは誰が製造できるのですか
製造自体はだれでも自由に行うことができます。ただし、"CHIRIMEN"という製品名で販売することはできません。一方、"Based on CHIRIMEN technology" という説明文を使うことができます。詳しくは[こちらのライセンス情報](https://chirimen-oh.github.io/license/)を参照ください。

## Q.CHIRIMEN の販売は誰ができるのですか
[こちらのライセンス情報](https://chirimen-oh.github.io/license/)に基づいて販売することができます。前項も参照にしてください。

## Q. CHIRIMEN はどのようなライセンスで公開されますか
ハードウェアとソフトウェア双方をカバーする[CHIRIMEN ライセンス](https://chirimen-oh.github.io/license/)に基づき公開されます。

## Q. CHIRIMEN は Mozilla の製品ですか
いいえ。CHIRIMEN は CHIRIMEN Open Hardwareコミュニティがプロトタイプとして開発している ウェブブラウザエンジンを搭載したボードコンピュータとそのソフトウェアであり、Mozilla の製品ではありません。

## Q. CHIRIMEN Open Hardware は Mozilla のプロジェクトですか
いいえ。CHIRIMEN Open Hardware は Mozilla Corporation や Mozilla Foundation によるプロジェクトではありません。Mozilla Factoryと呼ぶ枠組みの中の CHIRIMEN Open Hardwareコミュニティによって運営されているプロジェクトです。

## Q. Mozilla Factory とは何ですか
Mozilla Factory は Mozilla Japan が中心となってオープンソースによるモノづくりを学ぶ場所として 2012 年に立ち上げられた枠組みです。 CHIRIMEN Open Hardwareは Mozilla Factory の中のコミュニティによって進められているプロジェクトになります。   
[詳しくはこちらをご覧下さい](http://en.mozillafactory.org/about)

## Q. CHIRIMEN Open Hardware プロジェクト(コミュニティ） とは何ですか
さまざまなモノがコンピュータネットワークで繋がる未来の社会において、ヒトとモ ノがウェブを介して互いに協調しあえる環境を作り、“ウェブらしさ”とは何か、ウェブを介したよりよいヒト・モノの関係とは何かを考えていくプロジェクトです。  
[詳しくはこちら](http://en.mozillafactory.org/post/10861582384/open-hardware-project)をご覧下さい:

## Q. CHIRIMEN と CHIRIMEN Open Hardware の関係、違いは何ですか
CHIRIMEN は CHIRIMEN Open Hardware コミュニティによる開発成果の一つです。CHIRIMENは将来わたって、一つだけではないかもしれません。2015年に開発された最初の成果物はデザインID CMN2015-1と呼ばれています。CHIRIMEN Open Hardware コミュニティではCHIRIMEN をはじめとした、Web 技術をベースとしたオープンなハードウェアとソフトウェアの開発を進めています。その最初の開発成果はがCHIRIMENと呼ばれています。CHIRIMEN Open Hardware プロジェクトの設立趣旨は前項を参照ください。

## Q. CHIRIMEN Open Hardware では何をオープンにしているのですか
CHIRIMEN Open Hardwareコミュニティが提唱するウェブブラウザベースのボードコンピュータを製造するために必要な情報をオープンソースとして公開しています。それはハードウェアの製造に必要な情報とそこで稼働するオペレーティングシステムソフトウェアを含みます。また、ソースコードだけでなく開発や API の議論のプロセスもオープンにしています。

## Q. CHIRIMEN Open Hardware コミュニティには誰が参加できるのですか
個人だけでなく、任意の組織・団体が参加できます。

## Q. CHIRIMEN Open Hardware communityに参加したい場合はどうしたらよいですか。
[CHIRIMEN Open Hardware Facebook グループ](https://www.facebook.com/groups/mozopenhard/)への参加や[CHIRIMEN Open Hardware Google group](https://groups.google.com/forum/#!forum/chirimen-oh) を通してコミュニへ参加できます。
