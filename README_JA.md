# We now have a forum
GitHubで新規ISSUEを作成しないで下さい。２～４週間でクローズする予定です。
疑問、提案、会話をしたい場合は - https://nfeteam.org/forum をご利用ください。
気に入ってくれると良いのですが。

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

「デバイスに依存」 とはメーカによって設定されたデバイスの性能に依存するということです。ご利用メーカの製品ホームページで値を確認してください。

**あなたやあなたのデバイスが傷つくことを望んでいません。そのため、これらの制限事項への変更要求は受付けません。**


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


## メインスクリーン

![](http://i.imgur.com/ARKJkRS.gif)

Editing the main screen differs from original Joyetech firmwares. To edit items on main screen, call action "Edit Main" (デフォルトではファイヤーボタン4回クリック). Single Fire button click will switch next available editable item. Edit selected item by pressing regulatory buttons. To exit edit mode hold Fire button for about 1 sec.


## メインメニュー

ファイヤーボタンとプラスボタンを1秒同時押しするとメニューに遷移します。（デフォルト設定の場合）

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)

### プロファイルメニュー

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **ワイヤー** - coil material, temperature sensing or not (VW), can be set to standard or user-defined TFR;
* **コイル** - saved coil resistance;
* **TCR** - value can be edited when selected Joyetech TC algo with custom TCR;
* **T. Dom** - temperature-dominant regulation style;
* **プリヒート** - power control, use preheat or power curve;
* **PI-Reg** - PI Regulator for TC mode, improves power and temperature stabilization:
     - PI-Reg On/Off - switch between stock Joyetech and PI regulation;
     - Range - 0..100% - temperature range when PI regulation becomes active. 0 means that regulator is always on and controls power distribution from start of puff, 20% for example - PI regulator turns on when temperature of coil reached 20% range from profile settings;
     - P - proportional constant, the larger it is, the sharper the power changed;
     - I - integral constant, the larger it is, the settled power distribution is smoother.

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
     ***Note***: after switching RTC mode unplug USB and reboot your box by pulling out batteries for about 30 sec.
* **TEMP** - board temperature sensor, Ext - thermistor, Int - MCU;
* **D. Sleep** - deep sleep (enter after 3 minutes of inactivity) mode:
     - Std - standard deep sleep;
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - switch box to powered off state before going into deep sleep;
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock box before going into deep sleep.

### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Support for Avatar RC adapter and similar. Provides charging devices with a voltage of 5 volts and current up to 2.1 amps. To start charging, put RC adapter on box, connect device and press Fire button. Power Bank mode has auto-off feature when current drain is not exceed 50 mA (indicated by blinking label "On"). To stop charging, press Fire button.
To exit Power Bank mode press and hold Fire button, or regulatory buttons simultaneously.


### Info Screen

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Shows brief hardware information and some stats.

### Many thanks to:

* **TBXin** - for NFE Products and joint development
* **Zinger** - for graphics, ideas and tests
* **ArionWT** - for graphics, ideas and tests
* **ClockSelect** - for great project called myevic

# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.

# Donations:
If you like our project and you want to help in its development, you can [donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) us the amount of money you deem acceptable.
