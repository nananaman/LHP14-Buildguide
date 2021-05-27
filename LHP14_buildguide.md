# LHP14　ビルドガイド

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0481.JPG)



## はじめに

アナログジョイスティック付き左手デバイス『**LHP14**』のビルドガイドです。
（LHP=Left Hand Playing。ライトハンド奏法(=Right Hand Playing)にあやかって命名しました）

最近のアナログスティック付きデバイス入手難に際し、お困りの方々へ少しでも支援になればと開発しました。
ハンダ付け初心者の方にも組み立てられるよう、設計段階で色々工夫しました。もしかしてビルドガイドを見て不安になった貴方。実際に作ってみると案外難しくないかもです。（たぶん極とか零式以下の難易度です:-） **Let's do it!**



## キット内容

・本体基板3枚（ベース、メイン基板、キースイッチプレート）

・アナログジョイスティック　(ALPS ALPINE　**RKJXK122400Y**)

・Kailhロープロファイルスイッチ　2個

・丸スペーサーM2×L3.5mm　13個

・六角スペーサーM2×L10mm　2個

・スリムヘッド小ねじ M2x8 三価黒クロメート　5個

・スリムヘッド小ねじ M2x5 三価黒クロメート　2個

・スリムヘッド小ねじ M2x３ 三価黒クロメート　13個

・リードタイプダイオード1N4148　28個+予備

・タクタイルスイッチ（リセット用）

・アナログスティック用サムパッド取付部品

・OLEDシールド用アクリル板

・脚用ウレタンクッション　4個



## キット以外に必要な部品

・Pro Micro （コンスルー付き）

・OLEDモジュール （ピンソケット付き）

・Cherry MX互換スイッチ　26個

・Cherry MX互換スイッチキーキャップ　26個

・Kailhロープロスイッチキーキャップ1.5U　2個

・ジョイコン用サムパッドカバー

#### オプション

・発光ダイオード　YS-SK6812MINI-E　28個

もしくは

・フルカラーシリアルLEDテープ 6個タイプ

※上記は同時使用はできません。製作時にYS-SK6812MINI-Eを使うか、LEDテープで行くか決めてからパーツを集めてください。
YS-SK6812MINI-Eを使う方が難しいですが、見栄えはこちらが優れていると思います。

※これらは**遊舎工房**やamazonなどで購入可能です



## 必要な工具・材料

・はんだごて（温度調整式を推奨）

・はんだ（出来るだけ細いもの。0.6mmと0.3mmがあればgood）

・こて先クリーナー

・はんだ吸取線（なんだ付けを失敗した時などに使用）

・フラックス（はんだ付けする部品に塗布するとハンダ付けが容易になります）

・無水エタノールと綿棒（余分なフラックスを掃除するとき使用）

・精密ドライバー（+）

・ニッパー（ダイオードのリード（足）や使用済み吸取線をカット）

・マスキングテープ（ダイオードなど仮固定用）



## 作り方

#### ※電子部品の多くは取り付ける向きがあります。逆に取り付けると動かなかったり壊れたりします！

#### ※基板にも表裏があります。表に取り付ける部品、裏に付ける部品がありますので注意！

#### ※電子部品（特にLED）は熱に弱いので素早くはんだ付けしましょう！

#### ※複数個所をはんだ付けする部品は、まず1か所目のはんだ付けが終わったら、向きや部品の浮きなどをチェックしてください。はんだ付けが1か所であれば、リカバリは容易です。



### １．ダイオードのはんだ付け

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/diode.jpg)

ダイオードをはんだ付けします。ダイオードには極性（取付方向）があるので、ダイオードについている黒線を目印にします。





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/diode2.jpg)

ダイオードを基板の表面D1～D28にはんだ付けします。足をコの字に曲げて、基板の表面にセットして裏をはんだ付けします。向きはシルク印刷を参考にセットします。（黒線側が四角いパターンになる）





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0401.JPG)

ダイオードを1行ごとにセットしたらマスキングテープで固定すると作業中に外れずに作業しやすくなると思います。





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0405.JPG)

裏面ではんだ付けしたら足をカットします。





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0402.JPG)

はんだ付けが終わったら、念のためダイオードの向きが正しいかどうかチェックしましょう。





### ２．ProMicroの組み立て

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/Promicro.jpg)

コンスル―付きのProMicroにはピンが別に付いている場合が多いですが、今回はコンスルーを使用します。
コンスルーとは基板とProMicroを脱着可能にするソケットです。（ProMicroはUSB端子が取れたりとか意外と壊れることが多いのです；；）



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0408.JPG)

基板の表面にコンスルーを手で差し込みます。**（絶対に基板にはんだ付けしないでください）**
コンスルーの取り付けにも向きがあります。金色の穴が上になるようセットします。
向きも同じになるようにします。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0410.JPG)

コンスルーにProMicroを写真の向きで差し込みます。ProMicroは部品が付いていない方が表になります。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0412.JPG)

コンスルーとProMicroをはんだ付けします。最初に1か所だけはんだ付けして、ProMicroに浮きがないかチェックして残りのピンをはんだ付けしましょう。





### ３．リセットスイッチ、OLEDの取り付け

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0414.JPG)

リセットスイッチを基板表面に差し込み、裏側をはんだ付けします。この部品には極性はありません。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0416.JPG)

OLED取付用のソケットを表面に差し込み、裏面をはんだ付けします。こちらも極性はありません。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0417.JPG)

OLEDソケットにピンを差し込みます。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0419.JPG)

OLEDをピンにはんだ付けします。
OLEDはとても角度がズレやすいので、4ピンを一気にはんだ付けせず、まずは1か所ハンダ付けします。もしOLEDがズレているようでしたら、はんだを溶かし直して位置を調整します。
位置がOKでしたら残りの3ピンをはんだ付けします。





### ４．LEDのはんだ付け（オプション）

本機はYS-SK6812MINI-Eのはんだ付けを推奨しておりますが、LEDは熱に弱くはんだ付けの難易度が比較的高いので、作業難易度が低いLEDテープを使うことも出来るよう設計しました。

ただ、LEDテープを使ったアンダーグロー照明はアクリル板のベースを使ったときにより一層効果を発揮する方法なので、本機のような光を裏面に透過しないキーボードの場合は光り方が弱くなってしまいます；；



また、**YS-SK6812MINI-EとLEDテープの同時使用はできません。**



#### ・LEDテープを使う方法

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0422.JPG)

基板裏面の「GND」「DIN」「+5V」と書かれた端子にLEDテープをセットして、それぞれ対応する端子を写真のようにはんだ付けするだけです。



#### ・YS-SK6812MINI-Eを使う方法

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/LED.jpg)

基板の裏面から、LED取付穴にYS-SK6812MINI-Eをはめ込んで足をはんだ付けしていきます。

LEDは極度に熱に弱いので、温度調整式のはんだごてを使い、270度以下の出来るだけ低温で作業するとトラブルが起こりずらくなります。

フラックスや細いはんだを使うことも推奨です。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/LED2.jpg)

LEDには極性があります。4本のLED足の内、斜めにカットされた足が三角のマークにくるようセットします。

はんだ付けはこて先をLED足に出来るだけ触れさせないようにします。
フラックスを塗ったら、こて先で基板の銀色のパターンを温め、そこにはんだを流し込むと毛細管現象で溶けたハンダがLED足の方に流れ込むと思います。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0438.JPG)

あと2つでゴール。
がーんばれ、がーんばれッ！





28個のLEDをはんだ付け終わったら、ここでファームを焼いてテストしてみると良いと思います。はんだ付けが成功していればLEDが全て赤く光るはずです。

でも、LEDが点灯しなくても大丈夫！
この場合、LEDが破壊されているよりもはんだが上手く回っていないことが多いです。
点灯していないLEDか、その1つ前のLEDのはんだを軽く溶かし直してみて下さい。





### ５．スイッチの取り付け

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0443.JPG)

スリムヘッド小ねじ M2x8を5本、丸スペーサーM2×L3.5mmを5個、写真のようにキープレートにねじ止めします。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0445.JPG)

さらに丸スペーサーM2×L3.5mmを5個使って、基板とキープレートを合体させます。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0509.JPG)

こんな感じに組み立てます（写真撮るの忘れたので、素の基盤を使って再現しましたｗ）





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0512.JPG)

スイッチを穴に差し込んでいきます。
この時、スイッチの足が曲がることがあるので、差し込む前にスイッチの足が真っすぐかどうかチェックしながら作業します。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0447.JPG)


LED照明をつけた場合、スイッチは透明のものを使うと光が綺麗に回ると思います。





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0455.JPG)

スイッチをはんだ付けする時も、2か所をはんだ付けせずに1か所のみはんだ付けしてスイッチの浮き、足折れがないかチェックします。





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0448.JPG)

ジョイスティック周りの2キーは付属のChocロープロファイルスイッチ指定です。
（ジョイスティックの動きに干渉するのを防ぐため）



#### TIPS

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/Choc_mod.jpg)

私の作例写真で、メイン部分にMX互換スイッチとChocスイッチが混在していることがありますが、Chocスイッチの足が基板まで届かないので足を延長しております。
ドリルなど細いものにスズメッキ線を巻き付けて、ループとChoc足をはんだ付けしております。



### ６．OLEDシールド用スペーサーの取り付け

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0456.JPG)

六角スペーサーM2×L10mm　2個をスリムヘッド小ねじ M2x３でねじ止めします。





### ７．ジョイスティックの取り付け

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0459.JPG)

今回、指定部品としてテストで特性が安定していたALPSのRKJXK122400Yを付属しました。

とはいえ、アナログスティックはゲームデバイスの中でも消耗が激しい部品なので、基板のパターンでジョイスティック部分は仕様書よりも大きめの穴を開けて、将来のスティック交換が容易になるよう工夫しております。

（経験上、ジョイスティックは数千時間のプレイで不安定になることが多いです）





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0461.JPG)

ジョイスティックをはんだ付けしたら、丸スペーサーM2×L3.5mm3個をスリムヘッド小ねじ M2x３でねじ止めします。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0468.JPG)

スリムヘッド小ねじ M2x３　8本でベースプレートを本体にねじ止めします。





### ８．完成

![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0471.JPG)

スリムヘッド小ねじ M2x５2本でOLEDシールドのアクリル板を取り付けます。
ジョイスティックにアナログスティック用サムパッド取付部品を押し込みます。緩い場合は接着剤（SuperXなどは弱いです。作者はメタルロックをテスト中）を使ってください。



![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0474.JPG)

裏面に滑り止めの脚用ウレタンクッション　4個を張り付けます。





![](https://github.com/NeoTrinity-FF14/LHP14-Buildguide/blob/main/images/IMG_0473.JPG)

好みのキーキャップ、サムパッドカバーを取り付けたら完成です！

### **お疲れ様でした！！**
