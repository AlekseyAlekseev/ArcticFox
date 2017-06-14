# フォームが出来ました
GitHubで新規ISSUEを作成しないで下さい。２～４週間でクローズする予定です。
疑問、提案、問い合わせしたい場合は - https://nfeteam.org/forum をご利用ください。

# ArcticFox
*[NFE Team](http://nfeteam.org) はJoyetech, Wismec,  Eleafのデバイス用のカスタムファームウェアを提供しています。*

![](http://i.imgur.com/PqSrmLb.png) ![](http://i.imgur.com/C8Lu9SG.png) ![](http://i.imgur.com/aBhNKxV.png) ![](http://i.imgur.com/rk6gZo8.png) ![](http://i.imgur.com/5mU3FAB.png) ![](http://i.imgur.com/wl8wR8d.png) ![](http://i.imgur.com/s3yNIEf.png)


**ファームウェアの [インストール](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install)、デバイスの設定には [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) をご利用ください**


## サポート対象のデバイス一覧:
### Joyetech:
* eVic VTC Mini
* eVic VTC Dual
* eVic VTwo Mini
* eVic VTwo
* eVic AIO
* eVic Basic
* eVic Primo
* eVic Primo 2.0
* eVic Primo Mini
* eGrip II / Light
* Cuboid Mini
* Cuboid
* Cuboid 200

### Wismec:
* Presa TC75W
* Presa TC100W
* Reuleaux RX75
* Reuleaux RXmini
* Reuleaux RX200
* Reuleaux RX200S
* Reuleaux RX2/3
* Reuleaux RX300
* Predator 228
* VF Lite
* VF Stout
* VF Classic
* BV Centurion
* La Petite Box
* VS Switchbox

### Eleaf:
* Aster
* iStick Pico 75W
* iStick Pico Mega 80W
* iStick Pico Dual
* iStick Pico RDTA
* iStick iPower 80W
* iStick TC100W
* iStick TC200W
* iStick QC 200W

## 制限事項
安全なソフトウェアの利用は私たちの目標の一つです。 我々はメーカーの制限事項に準拠しています。

制限事項は以下となります。
* 最小抵抗値 (すべてのデバイスが対象)
  * 温度管理モードの場合 0.05 オーム
  * VWモードの場合 0.1 オーム
* 出力ワッテージ (デバイスに依存)
* 最大充電電流 (デバイスに依存)
* 出力電流  (デバイスに依存)
* 出力電圧範囲 (デバイスに依存)

「デバイスに依存」 とはメーカによるデバイスの仕様に依存するということです。ご利用メーカの製品ホームページで仕様を確認してください。

**我々はあなたが傷ついたり、ご利用のデバイスが壊れることを望んでいません。そのため、これらの制限事項への変更要求は受付けません。**


## プロファイル
Joyetechのオリジナルファームウェアとの主な違いはユーザーインターフェース（DNAのようなスタイル）とカスタマイズ性です。
プロファイルは使用するアトマイザー、コイルの素材、抵抗値、出力、温度などのパラメーターがセットとなったものです。
NFE Toolboxを使用して好みとマイザーに応じて８つのプロファイルを編集することができます。

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

マニュアルモードにおいてプロファイルは保存されたコイルの抵抗値によって自動切換となります。自動切換を使用するためには「スマートモード」を有効後、アトマイザーを取り付け利用したいプロファイルに割り当ててください。


![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

再度アトマイザーを取り付けた場合、自動的にプロファイルが設定されます。プロファイルにアトマイザーの抵抗値が見つからない場合、新しいプロファイルを選択するか、既存のプロファイルを設定してください。

保存された抵抗値と異なるプロファイルを手動で選択した場合、 選択したプロファイルの設定の更新(Update)か維持(Keep)を選択を求められます。

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)


## メイン画面

![](http://i.imgur.com/ARKJkRS.gif)

Joytechファームウェアと異なるメイン画面を編集してください。メイン画面の項目を編集するためには「Edit Main」を起動(デフォルトではファイヤーボタン4回クリック)して下さい。ファイヤーボタンを一回クリックすると編集可能な項目へ移動します。選択された項目を調整ボタン（＋、－）で編集します。編集モードを終了するには約1秒ファイヤーボタンを押し続けて下さい。

## メインメニュー

ファイヤーボタンとプラスボタンを1秒同時押しするとメニューに遷移します。（デフォルト設定の場合）

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)

### プロファイルメニュー

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire(ワイヤー)** - コイルの素材, 温度管理かVW, 標準化、ユーザー設定のTFRが設定できます。
* **Coil（コイル）** - コイルの抵抗を保存できます。
* **TCR** - value can be edited when selected Joyetech TC algo with custom TCR;
* **T. Dom** - 温度郵政の調整スタイル
* **プリヒート（Preheat）** - パワー調整, プリヒートかパワーカーブを使用
* **PI-調整（PI-Reg）** - 温度管理用のPI調整です、パワーと温度管理の安定を改善します。
     - PI-Reg On/Off - Joyetech方式とPI調整の切り替え
     - Range - 0..100% - PI調整が有効時の温度範囲。0 は常時調整、パフ開始時からのパワー供給コントロールすることを意味します。 20%は例えば - コイル温度がプロファイル設定の20％に到達時点でPI 調整が有効になります。
     - P - 比例定数、値が大きければよりシャープにパワーが変わります。
     - I - 積分定数、値が大きければ常時出力が滑らかになります。

### 画面メニュー

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - 調整ボタンを押すことによってモッドを起動するか
* **Logo** - メイン画面にロゴを表示するか
* **Clock**
     - **Type** - アナログかデジタル
     - **On Main** - メイン画面に時計を表示するか
     - **Saver** - 待機モードで時計を表示するか
* **Timeouts**
     - **Dim** - 画面オフまでの待機時間
     - **Dim** ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - ロック状態での画面オフまでの待機時間
     - **Logo** - ロゴ表示までの待機時間
     - **Clock** - 時計表示までの待機時間
* **Charge**
     - **Type** - 充電中の画面タイプ、 標準のみか追加情報を含めるか
     - **Add.** - extra item, 時計かロゴ
* **Stealth** - ステルスモード時の画面設定
     - **Charge** - ステルスモード中に充電画面を表示するか
     - **Saver** - ステルスモード中にスクリーンセーバーを表示するか
     - **ClkOnF** - オプションが有効な場合、メイン画面に時計を表示するか。ファイヤーボタンを1回押すと時計が表示されます。
* **Contrast** - 画面に輝度変更
* **Skin** - メイン画面のスタイルを変更

### 設定メニュー

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - 1ワット単位でパワーを調整するか
* **Clicks** - アクションの割り当てをします
     * **2/3/4 Fire button clicks**:
          - None - 何もしない
          - Edit Main - Joyetechのデフォルトは3クリック
          - Main Menu - メインメニューに遷移します。 ファイヤーボタンと+ボタン同時押しと同じ
          - Preheat - 有効なプロファイルのプリヒートを設定
          - Profiles - プロファイルを選択する
          - Edit Profile - プロファイルメニューへ遷移
          - T. Dom - temperature-dominant on/off
          - Clock - メイン画面に時計を表示するか
          - Info - 情報画面を表示
          - Reset Cnt. - 情報画面にshow vaping stats info screen with opportunity to reset counters;
          - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) Bank - パワーバンクモードへ移行
          - Coil ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - コイル抵抗ロックのon/off (温度管理モード用);
          - Key ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - キーロックのon/off;
          - Stealth - ステルスモードのon/off
          - Smart On/Off - スマートモードのon/off
          - LSL - スリープモードのon/off
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - デバイスロックのon / off (全ボタンをロック but leave mod powered on)
          - On/Off - モッド本体のon/off
     * **5 Fire button clicks**:
          - On/Off - モッド本体のon/off
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock all buttons but leave mod powered on;
* **Smart** - 自動的にプロファイル設定を切換えます
     - Off/On/Lazy - スマートモードの動作設定。 LazyはBoXが有効時アトマイザーを変更した場合、自動でプロファイルが変更されます。
     - Range - 抵抗許容誤差
* **Clock** - 時計調整
     - Date/Time - 現在日時を設定します
     - Adjust Time - 1秒単位で時間を微調整します
     - LIRC Speed - 速度調整of internal imprecise oscillator used on モッド基板上の32768Hz水晶体なしで
* **Expert** - 上級者向けの設定

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/pp3TTaR.png)

* **USB**
     - NoSlp - do not enter deep sleep mode while connected to USB - may lead to self-discharging multi-cells boxes after charging stops;
     - Charge - デバイスがUSBに接続されると充電を開始します。 - 複数電池対応デバイスのみ使用可能
* **BVO** - バッテリー電圧のオフセット
* **BATT** - バッテリー放電のプロファイル
* **SHUNT** - オームメーターの訂正
* **ChkTCR** - コイル素材のTCRチェック、 このオプションをオフにすると重いコイルのTCRエラーが低減されます。switching this option to off can eliminate TCR Error on heavy coils;
* **RCOBC** - バッテーリー交換時にカウンターをリセットし統計情報を削除。
* **RTC** - リアルタイム時刻モードRealtime Clock mode:
     - LXT - full hardware support;
     - LIRC - inaccurate secondary oscillator;
     - LSL - software mode. It takes some more energy in standby mode, but provides more accurate results on boxes without hardware RTC implementation;  
     ***Note***: after switching RTC mode unplug USB and reboot your box by pulling out batteries for about 30 sec.
* **TEMP** - board temperature sensor, Ext - thermistor, Int - MCU;
* **D. Sleep** - deep sleep (enter after 3 minutes of inactivity) mode:
     - Std - standard deep sleep;
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - switch box to powered off state before going into deep sleep;
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock box before going into deep sleep.

### パワーバンク

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Support for Avatar RC adapter and similar. Provides charging devices with a voltage of 5 volts and current up to 2.1 amps. To start charging, put RC adapter on box, connect device and press Fire button. Power Bank mode has auto-off feature when current drain is not exceed 50 mA (indicated by blinking label "On"). To stop charging, press Fire button.
To exit Power Bank mode press and hold Fire button, or regulatory buttons simultaneously.


### 情報画面

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

ハードウェア情報、統計データを表示します。

### Many thanks to:

* **TBXin** - for NFE Products and joint development
* **Zinger** - for graphics, ideas and tests
* **ArionWT** - for graphics, ideas and tests
* **ClockSelect** - for great project called myevic

# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.

# Donations:
If you like our project and you want to help in its development, you can [donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) us the amount of money you deem acceptable.
