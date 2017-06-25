<!-- 
# We now have a forum
Please do not create new issues on GitHub. We will close this possibility in a 2-4 weeks.
If you have questions or suggestions or you just want to talk - https://nfeteam.org/forum. 
We are hoping that you will like it ;)

# ArcticFox
*[NFE Team](http://nfeteam.org) presents custom Firmware for Joyetech, Wismec and Eleaf battery mods*

![](http://i.imgur.com/PqSrmLb.png) ![](http://i.imgur.com/C8Lu9SG.png) ![](http://i.imgur.com/aBhNKxV.png) ![](http://i.imgur.com/rk6gZo8.png) ![](http://i.imgur.com/5mU3FAB.png) ![](http://i.imgur.com/wl8wR8d.png) ![](http://i.imgur.com/s3yNIEf.png)

**Use [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) for [installing](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) firmware and configuring your device.**
-->

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

<!-- 
## Limitations
The safe use of our software it's one of our main goals. We retain all factory restrictions, because the device manufacturer did NOT make them "just for fun".
What are the limitations?
* Minimal Resistance (For all supported devices)
  * 0.05 Ohm for Temperature Control mode
  * 0.1 Ohm for Vari-Watt mode
* Output Wattage (Depending on the device)
* Maximum Charging Current (Depending on the device)
* Maximum Output Current (Depending on the device)
* Output Voltage Range (Depending on the device)

"Depending on the device" means that each device has its own values, which are choosen by the manufacturer. You can find this values on the product page of your manufacturer's website.

**All requests to change these values will be rejected as we don't want you to hurt yourself or your device.**
-->

## 制限事項
安全なソフトウェアは目標の一つで、 メーカーの制限事項に準拠しています。

制限事項は以下となります。
* 最小抵抗値 (すべてのデバイスが対象)
  * 温度管理モードの場合 0.05 オーム
  * VWモードの場合 0.1 オーム
* 出力ワッテージ (デバイスに依存)
* 最大充電電流 (デバイスに依存)
* 出力電流  (デバイスに依存)
* 出力電圧範囲 (デバイスに依存)

「デバイスに依存」 とはメーカによるデバイスの仕様に依存するということです。ご利用メーカの製品ホームページで仕様を確認してください。

**我々はあなたが怪我をしたり、ご利用のデバイスが壊れることを望んでいません。そのため、これらの制限事項への変更要求は受付けません。**

<!--
## Profiles
The main difference is the profile based user interface, so to say, the DNA-style, and the larger focus on customization than original Joyetech firmware.
Profile is the set of parameters of used atomizer, such as coil material, resistance, power and temperature values.
The user have 8 profiles which can be edited with NFE Toolbox, and which can be assigned to his favourite atomizers.

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

Profiles can be switched automatically, based on saved coil resistance, and in manual mode. All you need to use the automatic switch is to enable "Smart" mode, install atomizer and assign them to the desired profile.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

When you re-install this atomizer later, assigned profile will be activated automatically.
If resistance of installed atomizer is not found in profiles, you'll be prompted to select new profile or re-assign existing.

When you switching manually to profile that have saved resistance mismatch, you'll be prompted to update or keep settings of selected profile.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)
-->

## プロファイル
元のJoyetechファームウェアとの主な違いはユーザーインターフェース（DNAのようなスタイル）とカスタマイズ性です。
プロファイルは使用するアトマイザー、コイルの素材、抵抗値、出力、温度などのパラメーターがセットとなったものです。
NFE Toolboxを使用して好みとマイザーに応じて８つのプロファイルを割り当てることができます。

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

プロファイルは保存されたコイルの抵抗値による自動切換えか手動での切換が可能です。自動切換を使用するためには「スマートモード」を有効後、アトマイザーを取り付け利用したいプロファイルに割り当ててください。


![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

再度アトマイザーを取り付けた場合、自動的にプロファイルが設定されます。プロファイルにアトマイザーの抵抗値が見つからない場合、新しいプロファイルを選択するか、既存のプロファイルを設定してください。

保存された抵抗値と異なるプロファイルを手動で選択した場合、 選択したプロファイルの設定の更新(Update)か維持(Keep)を選択を求められます。

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)

<!--
## Main Screen

![](http://i.imgur.com/ARKJkRS.gif)

Editing the main screen differs from original Joyetech firmwares. To edit items on main screen, call action "Edit Main" (4 Fire button clicks by default). Single Fire button click will switch next available editable item. Edit selected item by pressing regulatory buttons. To exit edit mode hold Fire button for about 1 sec.


## Main Menu

Hold Fire and Plus buttons (by default) for a 1 second to enter menu.

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)
-->

## メイン画面

![](http://i.imgur.com/ARKJkRS.gif)

メイン画面の設定は元のJoytechファームウェアと異なります。メイン画面の項目を編集するためには「Edit Main」を起動(デフォルトではファイヤーボタン4回クリック)して下さい。ファイヤーボタンを一回クリックすると編集可能な項目へ移動します。選択された項目を調整ボタン（＋、－）で編集します。編集モードを終了するには約1秒ファイヤーボタンを押し続けて下さい。

## メインメニュー

ファイヤーボタンとプラスボタンを1秒同時押しするとメニューに遷移します。（デフォルト設定の場合）

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)

<!--
### Profile Menu

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire** - coil material, temperature sensing or not (VW), can be set to standard or user-defined TFR;
* **Coil** - saved coil resistance;
* **TCR** - value can be edited when selected Joyetech TC algo with custom TCR;
* **T. Dom** - temperature-dominant regulation style;
* **Preheat** - power control, use preheat or power curve;
* **PI-Reg** - PI Regulator for TC mode, improves power and temperature stabilization:
     - PI-Reg On/Off - switch between stock Joyetech and PI regulation;
     - Range - 0..100% - temperature range when PI regulation becomes active. 0 means that regulator is always on and controls power distribution from start of puff, 20% for example - PI regulator turns on when temperature of coil reached 20% range from profile settings;
     - P - proportional constant, the larger it is, the sharper the power changed;
     - I - integral constant, the larger it is, the settled power distribution is smoother.
-->

### プロファイルメニュー

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire(ワイヤー)** - コイルの素材, 温度管理かVW, 標準か指定のTFRが設定できます。
* **Coil（コイル）** - 保存したコイル抵抗値。
* **TCR** - カスタムTCRでJoyetech TC algoを選択すると値を編集できます。
* **T. Dom** - 温度優先調整方式。
* **Preheat** - パワー調整, プリヒートかパワーカーブ。
* **PI-Reg** - 温度管理用のPI調整。出力と温度管理の安定性を改善します。
     - PI-Reg On/Off - Joyetech方式とPI調整の切り替え。
     - Range - 0..100% - PI調整が有効となる温度範囲。0 は常時調整、パフ開始時からの出力コントロールすることを意味します。 20%は例えば - コイル温度がプロファイル設定の20％に到達時点でPI 調整が有効になります。
     - P - 比例定数、値が大きければより出力が急激に変わります。
     - I - 積分定数、値が大きければ固定の出力分布が滑らかになります。

<!--

### Screen Menu

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - waking mod up by pressing regulatory buttons;
* **Logo** - show logo on main screen;
* **Clock**
     - **Type** - analog or digital;
     - **On Main** - show clock on main screen;
     - **Saver** - show clock in standby mode;
* **Timeouts**
     - **Dim** - idle time before the screen turns off;
     - **Dim** ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - idle time before the screen turns off in locked state;
     - **Logo** - idle time before displaying logo;
     - **Clock** - idle time before displaying clock;
* **Charge**
     - **Type** - charging screen type, standard or with additional information;
     - **Add.** - extra item, clock or logo;
* **Stealth** - settings for screen in Stealth Mode:
     - **Charge** - charging screen will be shown in Stealth Mode;
     - **Saver** - screen saver will be shown in Stealth Mode;
     - **ClkOnF** - when Clock on Main Screen option is enabled, clock will be shown immediately on single Fire click;
* **Contrast** - adjust brightness of display;
* **Skin** - change main screen style.
-->


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
     - **Add.** - 追加項目、時計かロゴ
* **Stealth** - ステルスモード時の画面設定
     - **Charge** - ステルスモード中に充電画面を表示するか
     - **Saver** - ステルスモード中にスクリーンセーバーを表示するか
     - **ClkOnF** - オプションが有効な場合、メイン画面に時計を表示するか。ファイヤーボタンを1回押すと時計が表示されます。
* **Contrast** - 画面の明るさを変更
* **Skin** - メイン画面のスタイルを変更

<!--
### Settings Menu

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - increment/decrement power by 1,0 Watt;
* **Clicks** - actions assigned on
     * **2/3/4 Fire button clicks**:
          - None;
          - Edit Main - Joyetech default 3-clicks action;
          - Main Menu - enter Main Menu, the same as Fire + ;
          - Preheat - preheat settings for active profile;
          - Profiles - Profiles Selector;
          - Edit Profile - enter Profile Menu;
          - T. Dom - temperature-dominant on/off;
          - Clock - show/hide clock on main screen;
          - Info - show Info Screen;
          - Reset Cnt. - show vaping stats info screen with opportunity to reset counters;
          - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) Bank - switch box to Power Bank mode;
          - Coil ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - switch coil resistance lock on/off (for TC modes);
          - Key ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - switch Keylock on/off;
          - Stealth - switch Stealth Mode on/off;
          - Smart On/Off - switch Smart Mode on/off;
          - LSL - switch light sleep mode on/off;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - switch Device Lock on / off (lock all buttons but leave mod powered on);
          - On/Off - switch mod on/off;
     * **5 Fire button clicks**:
          - On/Off - switch mod on/off;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock all buttons but leave mod powered on;
* **Smart** - automatic switching profiles settings:
     - Off/On/Lazy - Smart Mode behavior setting, Lazy means that profile can be switched automatically only on atomizer change while the box is in active state;
     - Range - resistance tolerance;
* **Clock** - realtime clock setup;
     - Date/Time - set current date and time;
     - Adjust Time - precise adjusting time by 1 second step;
     - LIRC Speed - adjusting speed of internal imprecise oscillator used on boxes without external 32768 Hz crystal on board;
* **Expert** - settings for advanced users:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/pp3TTaR.png)
-->


### 設定メニュー

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - 1ワット単位でパワーを調整するか
* **Clicks** - アクションの割り当てをします
     * **ファイヤーボタン クリック数 2/3/4**:
          - None - 何もしない
          - Edit Main - Joyetechのデフォルトは3クリック
          - Main Menu - メインメニューに遷移します。 ファイヤーボタンと+ボタン同時押しと同じ
          - Preheat - 有効なプロファイルのプリヒートを設定
          - Profiles - プロファイルを選択する
          - Edit Profile - プロファイルメニューへ遷移
          - T. Dom - 温度優先 on/off
          - Clock - メイン画面に時計を表示するか
          - Info - 情報画面を表示
          - Reset Cnt. - カウンターをリセット可能なVaping統計情報画面を表示する。
          - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) Bank - パワーバンクモードへ移行
          - Coil ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - コイル抵抗ロックのon/off (温度管理モード用);
          - Key ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - キーロックのon/off;
          - Stealth - ステルスモードのon/off
          - Smart On/Off - スマートモードのon/off
          - LSL - ライトのスリープモードのon/off
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - デバイスロックのon / off (全ボタンをロック but leave mod powered on)
          - On/Off - モッド本体のon/off
     * **5 Fire button clicks**:
          - On/Off - モッド本体のon/off
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - すべてのボタンをロックしますが、電源はオンのままです。
* **Smart** - 自動的にプロファイル設定を切換えます
     - Off/On/Lazy - スマートモードの動作設定。 LazyはBoXが有効時アトマイザーを変更した場合、自動でプロファイルが変更されます。
     - Range - 抵抗の許容差
* **Clock** - 時計調整
     - Date/Time - 現在日時を設定します
     - Adjust Time - 1秒単位で時間を微調整します
     - LIRC Speed - 基板上に32768Hz水晶振動子を搭載していないデバイスの発振器の速度を調整します。
* **Expert** - 上級者向けの設定

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/pp3TTaR.png)

<!--
* **USB**
     - NoSlp - do not enter deep sleep mode while connected to USB - may lead to self-discharging multi-cells boxes after charging stops;
     - Charge - device is charging batteries while connected to USB - for multi-cells boxes only;
* **BVO** - batteries voltages offset;
* **BATT** - battery discharge profile;
* **SHUNT** - Ohm-meter correction;
* **ChkTCR** - check coil material TCR, switching this option to off can eliminate TCR Error on heavy coils;
* **RCOBC** - Reset Counters on Battery Change, clear vaping statistics;
* **RTC** - Realtime Clock mode:
     - LXT - full hardware support;
     - LIRC - inaccurate secondary oscillator;
     - LSL - software mode. It takes some more energy in standby mode, but provides more accurate results on boxes without hardware RTC implementation;  
     ***注意***: after switching RTC mode unplug USB and reboot your box by pulling out batteries for about 30 sec.
* **TEMP** - board temperature sensor, Ext - thermistor, Int - MCU;
* **D. Sleep** - deep sleep (enter after 3 minutes of inactivity) mode:
     - Std - standard deep sleep;
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - switch box to powered off state before going into deep sleep;
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock box before going into deep sleep.
-->

* **USB**
     - NoSlp - USB接続時にスリープモードに移行しません。 - 充電停止後に複数電池の自己放電となる可能性があります。
     - Charge - デバイスがUSBに接続中充電を開始します。 - 複数電池対応デバイスのみ使用可能
* **BVO** - バッテリー電圧のオフセット
* **BATT** - バッテリー放電のプロファイル
* **SHUNT** - オームメーターの補正
* **ChkTCR** - コイル素材のTCRチェック、 このオプションをオフにすると重いコイルのTCRエラーが低減されます。
* **RCOBC** - バッテーリー交換のカウンターをリセットし統計情報を削除。
* **RTC** - リアルタイム時刻モード
     - LXT - 完全なハードウェアサポート。
     - LIRC - 不正確な発振器。
     - LSL - ソフトウェアモード。スタンバイモードで電力を消費しますが、リアルタイムクロック未搭載のデバイスでより正確な時刻となります。
     ***注意***: リアルタイム時刻モードに変更後はUSBを抜き、電池を30秒間抜いた後再起動してください。
* **TEMP** - 温度センサー種別、Ext - サーミスタ(thermistor), Int - MUC温度センサー
* **D. Sleep** - ディープスリープモード (3分の未操作で移行します)。
     - Std - 標準ディープスリープ
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - ディープスリープ前に電源を切ります。
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - ディープスリープ前にロックします。

<!-- 

### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Support for Avatar RC adapter and similar. Provides charging devices with a voltage of 5 volts and current up to 2.1 amps. To start charging, put RC adapter on box, connect device and press Fire button. Power Bank mode has auto-off feature when current drain is not exceed 50 mA (indicated by blinking label "On"). To stop charging, press Fire button.
To exit Power Bank mode press and hold Fire button, or regulatory buttons simultaneously.


### Info Screen

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Shows brief hardware information and some stats.
-->

### パワーバンク

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Avatar RC adapter等をサポートしています。5ボルト、最大2.1アンペアでデバイスに充電できます。充電を開始するためには、RC adapter接続後、デバイスに接続しファイヤーボタンを押します。パワーバンクモードは、出力電流が50mA以下となった場合（「On」が点滅）自動オフとなります。充電を停止する場合、ファイヤーボタンを押して下さい。
パワーバンクモードを終了する場合、ファイヤーボタンか調整ボタン（＋、－）をしばらく押して下さい。


### 情報画面

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

ハードウェア情報、統計データを表示します。

### 感謝:

* **TBXin** - NFE製品および共同開発用
* **Zinger** - グラフィックス、アイデア、テスト
* **ArionWT** - グラフィックス、アイデア、テスト
* **ClockSelect** - 素晴らしいmyevicプロジェクト

<!-- 
# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.
-->

# 免責事項:

使用可能なファームウェアとして配布していますが保証はありません。通常用途、特定用途は保証されますが、それ以外のあらゆる保証はありません。ファームウェアの品質および性能に関するリスクは全てご自身で負って下さい。

<!-- 
# Donations:
If you like our project and you want to help in its development, you can [donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) us the amount of money you deem acceptable.
-->

# 寄付:
このプロジェクトに賛同し支援する場合、 できる範囲での[寄付](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE)をお願いします。