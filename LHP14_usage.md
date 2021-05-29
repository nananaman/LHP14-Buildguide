## 動作テスト
LHP14はQMK firmwareという、キーボード用のオープンソースファームウェアで動作します。  
私はwindows10でQMK MSYSとQMK Toolboxを使っておりますので、こちらを使った手順で説明します。
<br>
<br>
<br>

### １．QMK-MSYSのセットアップ

・[公式サイト](https://msys.qmk.fm/)からLatest versionのQMK_MSYS.exeをダウンロードし実行します。
　DL時、警告のメッセージが出る場合がありますが、何とか頑張ってダウンロードしましょう。

・QMK MSYSを起動します。 
　黒い画面が開き、＄が出たら、qmk setupと打ち込み、エンターを押します。

・設問が出ますが全てy(es)で答えます。

・cloning into...　と出てファイルのアップデートが始まりますが、終わるまで待ちます。

・QMK is ready to goと出て、＄の横にカーソルが出てきたらQMK MSYSセットアップ完了です！
<br>
<br>
<br>

### ２．QMK Toolboxのインストール

・[公式サイト](https://github.com/qmk/qmk_toolbox/releases)からqmk_toolbox_install.exeをダウンロードし実行します。
<br>
<br>
<br>
### ３．テストファームの書き込み

・[LHP14ファームウェア置き場](https://github.com/NeoTrinity-FF14/LHP14-firmware)からLHP14のファームウェアをダウンロードします。Codeと書いた緑のボタンを押し、Zipファイルをダウンロード、解凍します。

・C:\Users\ユーザー名\qmk_firmware\keyboards\に、LHP14フォルダをフォルダごとコピーしてください。

・QMK Toolboxを起動します。

・右上にあるAuto-Flashをチェックします。

・LHP14フォルダ内のLHP14_Test.hexをQMK Toolboxにドラッグ＆ドロップします。

・PCにLHP14をつなぎ、LHP14のリセットボタンを押します。
<br>
<br>
<br>
### 4．動作テスト

・テストファームを書き込むとOLEDが光り、LEDが赤く光ります。

・キーを押して、文字が出てくれば正常。（3行7列はジョイスティック押下、4行1列はレイヤーがKEY TEST・RGBLEDTESTに切り変わります。各キーの割り当ては\LHP14\keymaps\Test\のkeymap.cを参照してください）

・4行1列目のキーを押し、RGB LED TESTに切り替えてください。2行1列目のキーを押すとLEDの発光パターンが切り替わっていきます。2行２列目のキーでLEDをリセットして全て赤に変わります。

・windowsコントロールパネル→ハードウェアとサウンド→デバイスとプリンタ→LHP14を右クリックでゲームコントローラーの設定→LHP14のプロパティでジョイスティックのテスト。ジョイスティック押し下げでボタン１が反応すればOK。
<br>
<br>
### お疲れ様でした。上手く動きましたか？？　

