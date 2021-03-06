# ACT.Hojoring
[![Downloads](https://img.shields.io/github/downloads/anoyetta/ACT.Hojoring/total.svg)](https://github.com/anoyetta/ACT.Hojoring/releases)
[![License](https://img.shields.io/badge/license-BSD--3--Clause-blue.svg)](https://github.com/anoyetta/ACT.Hojoring/blob/master/LICENSE)

「補助輪」  
Advanced Combat Tracker の FFXIV向けプラグインの詰合せです。  
スペスペ・ウルスカ・TTSゆっくりをまとめたものです。これ自体が独立したプラグインではありません。

## 最新リリース
**[Lastest-release](https://github.com/anoyetta/ACT.Hojoring/releases/latest)**  
[pre-releease](https://github.com/anoyetta/ACT.Hojoring/releases)

## インストール
### ALL-IN-ONE インストール
ALL-IN-ONEインストーラ「**[Actor](https://github.com/eai04191/Actor)**」を使用してACT本体ごと簡単に導入できます。設定も引き継がれますのでこの方法でのインストールをお勧めします。  
1. 最新版の Actor を **[こちら](https://github.com/eai04191/Actor/releases)** からダウンロードする  
2. Actor の **[README](https://github.com/eai04191/Actor)** を読む。
3. **Actor.exe** を実行する

### マニュアルインストール
自分でDLLを入手して手動で追加したい方はこちらの方法になります。

1. 各種ランタイムをインストールする  
**[Visual Studio 2017 用 Microsoft Visual C++ 再頒布可能パッケージ](https://go.microsoft.com/fwlink/?LinkId=746572)**  
**[Microsoft .NET Framework 4.7](https://www.microsoft.com/en-us/download/details.aspx?id=55170)**  
をインストールする。

2. 最新版を取得する  
最新リリースからダウンロードします。

3. 解凍する  
ダウンロードしたプラグイン一式を解凍し任意のフォルダに配置します。  
Discord への通知を使用する場合は、lib\libopus.dll, lib\libsodium.dll を **ACT本体と同じフォルダ** にコピーします。

4. ACTに追加する
ACTにプラグインとして追加します。3つのプラグインそれぞれを登録します。  
必要なものだけ登録してください。もちろんすべて登録しても問題ありません。  

  * ACT.SpecialSpellTimer.dll
  * ACT.UltraScouter.dll
  * ACT.TTSYukkuri.dll

### 動作環境
* Windows 10 以降

## 使い方
基本的に **[Wiki](https://github.com/anoyetta/ACT.Hojoring/wiki)** を見てください。

#### おすすめ設定とか教えて
**[ACT.Hojoring アップローダ](https://ux.getuploader.com/hojoring/)**  
設定の共有向けにアップローダを用意しました。作者または有志が公開してくれた設定がアップロードされていますので自由にお使いください。

##### Hojoring の設定ファイルあれこれ
1. 格納場所  
%APPDATA%\anoyetta\ACT  
にすべて格納されています。よって、OSの再インストール等のときはこのディレクトリを丸ごとバックアップして再インストール後に配置しなおせば、再インストール前の設定を復元できます。

2. 設定ファイル  
ACT.SpecialSpellTimer.config  
ACT.TTSYukkuri.config  
ACT.UltraScouter.config  
それぞれ、スペスペ・ゆっくり・ウルスカの設定ファイルです。  
スペスペではトリガ以外のオプション関係の設定が保存されています。他のプラグインではプラグインそのものの設定が保存されています。  

3. スペスペのトリガの設定ファイル  
ACT.SpecialSpellTimer.Panels.xml  
ACT.SpecialSpellTimer.Spells.xml  
ACT.SpecialSpellTimer.Telops.xml  
スペスペの各種トリガの設定ファイルです。それぞれ、スペルパネル・スペル・テロップの設定ファイルになります。  
前述の格納場所に上書きしても使えますし、UIからインポートしても使えます（スペルパネルはインポートできません）。ファイルを上書きしたときは丸ごと入れ替わります。インポートした場合は、既存の設定に追加される形になります。他人のトリガを取り込む場合はインポートで追加したほうが良いでしょう。

##### アップローダの注意事項
* アップローダの利用規約を遵守してください
* 公序良俗に違反しない範囲で自由に使用してください
* アップロードされたものは [MIT License](https://ja.wikipedia.org/wiki/MIT_License) にもとづいて公開されているものとします
* アップローダの容量の問題や公開物の内容によっては予告なく削除されることがあります

## ライセンス
[3-Clause BSD License](LICENSE)  
&copy; 2017 anoyetta  

ただし下記の行為を禁止します。
* 配布されたバイナリに対してリバースエンジニアリング等を行い内部を解析する行為
* 配布されたバイナリのすべてもしくは一部を本来の目的とは異なる目的に使用する行為

## お問合わせ
### なんかエラー出た
開発者に質問する場合は、下記の情報を添えてください。
* ACT本体のログファイル  
* 当プラグインのログファイル
* （あれば）エラーダイアログのスクリーンショット

##### [Help] → [サポート情報を保存する] から必要な情報一式を保存できます。
![help](https://github.com/anoyetta/ACT.Hojoring/blob/master/images/help.png?raw=true)

##### 起動できないなどUIから取得できない場合は下記のフォルダから収集してください。
%APPDATA%\Advanced Combat Tracker\Advanced Combat Tracker.log  
%APPDATA%\anoyetta\ACT\logs\ACT.Hojoring.YYYY-MM-DD.log  

### スペルが動かない
前述の情報に以下の情報も追加で必要になります。  
* 引っ掛けたい対象のログ
* 対象のスペルやテロップの設定

これらの情報がない場合は回答できません。

### まったく分かっていない
リモートでサポートすることも出来ます。  
下記のいずれかのリモートソフトウェアを使用して [DISCORD](https://discord.gg/n6Mut3F) 経由でリモートサポートを依頼してください。  
* [TeamViewer](https://www.teamviewer.com)
* [Google リモートデスクトップ](https://support.google.com/chrome/answer/1649523?co=GENIE.Platform%3DDesktop&hl=ja)  

また、リモートサポートの依頼ではなくても説明が困難な場合はリモートによる設定を案内する場合があります。その場合は案内に従ってください。

### 問合せフォーム
[https://github.com/anoyetta/ACT.Hojoring/issues/new](https://github.com/anoyetta/ACT.Hojoring/issues/new)  
からチケットを登録してください。[issues](https://github.com/anoyetta/ACT.Hojoring/issues) から既存の課題、現在の状況を確認出来ます。  
重複する質問はご遠慮ください。

### 連絡先
discord:  [Hojoring Forum](https://discord.gg/n6Mut3F)  
mail:     anoyetta(at)gmail.com  
twitter:  [@anoyetta](https://twitter.com/anoyetta)  
まで。  
基本的に issues からお願いします。issues の課題から優先的に対応します。  
どうしても直接連絡したい場合はなるべく discord を使用してください。 
