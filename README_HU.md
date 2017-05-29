# Van egy fórumunk
Kérlek ne csinálj újabb hibajelentést GitHub-on. 2-4 héten belül mi le fogjuk zárni ezt a részt.
Ha kérdésed, ötleted van, vagy szeretnél beszélgetni. - https://nfeteam.org/forum. 
Reméljük, tetszeni fog ;)

# ArcticFox
*Az [NFE Team](http://nfeteam.org) egyedi firmware-e Joyetech, Wismec and Eleaf modokhoz*

![](http://i.imgur.com/PqSrmLb.png) ![](http://i.imgur.com/C8Lu9SG.png) ![](http://i.imgur.com/aBhNKxV.png) ![](http://i.imgur.com/rk6gZo8.png) ![](http://i.imgur.com/5mU3FAB.png) ![](http://i.imgur.com/wl8wR8d.png) ![](http://i.imgur.com/s3yNIEf.png)

**A firmware az [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) segítségével [tölthető fel](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) a modra és konfigurálható.**

## Támogatott eszközök:
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

## Korlátozások
A szoftverünk biztonságos működése az egyik fő célunk. Megtartottunk minden gyári korlátozást, mert azt a gyártó NEM "viccből" rakta bele.
Mik ezek a korlátozások?
* Minimum ellenállás (Minden támogatott eszközön)
  * 0.05 Ohm TC üzemmódban
  * 0.1 Ohm VW üzemmódban
* Kimeneti teljesítmény (Eszköz függő)
* Maximum töltő áram (Eszköz függő)
* Maximum kimeneti áram ((Eszköz függő)
* Kimeneti feszültség tartomány (Eszköz függő)

"Eszköz függő" azt jelenti, hogy minden eszköznek van egy saját értéke, amit a gyártó választott ki. Ezt az értéket megtalálod a kézikönyvben vagy a gyártó weboldalán.

**Minden kérés ezen értékek megváltozatására vissza lesz utasítva.**


## Profilok
A fő különbség az eredeti Joyetech firmware-hez képest, hogy a felhasználói felület a DNA-hoz hasonlóan profil alapú és nagyobb hangsúly került a testreszabhatóságra.
A profil a kazán különböző paramétereinek együttese, mint a tekercs anyaga, ellenállása, teljesítmény és hőmérséklet adatok.
8 különböző profil áll rendelkezésre, melyek a NFE Toolbox segítségével hozhatók létre és szerkeszthetők, a kedvenc kazánjainkhoz szabva.

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

A profilok a tekercs ellenállása alapján automatikusan vagy manuálisan válthatók. Az automatikus átkapcsolás használatához csak a "Smart" módot kell engedélyezni, majd csatlakoztatni a kazánt és hozzárendelni a kívánt profilhoz.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

Ha később ezt a kazánt tekerjük a modra, a hozzárendelt profil automatikusan aktiválódik.
Ha a csatlakoztatott kazán ellenállásához nem található korábban hozzárendelt profil, létre kell hoznunk egy újat, vagy hozzárendelhetjük egy már meglévő profilhoz.
Ha manuálisan váltunk egy olyan profilra, amely már rendelkezik korábban mentett ellenállással, de nem passzol az aktuálisan használt kazánhoz, lehetőségünk van frissíteni a profilt, vagy megtartani a korábbi értéket.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)


## Main Screen

![](http://i.imgur.com/ARKJkRS.gif)

A főképernyő szerkesztése eltér az eredeti Joyetech firmware-étől. Szerkeszteni a főképernyőn, az "Edit Main" opcióval lehetséges (tűzgomb négyszeri megnyomása alapesetben). Tűzgomb egyszeri megnyomásával léphetünk a következő szerkeszthető elemre. A kiválasztott értéket, a +/- gombbal lehetséges. Kilépni a tűzgomb 1mp nyomvatartásával lehet.

## Main Menu

Tartsd nyomva a tűz és a plusz gombot 1 másodpercig a menübe való belépéshez

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)

### Profile Menu

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire** - huzal anyaga, TC vagy sem (VW), beállítható standard vagy felhasználó által létrehozott TFR görbe;
* **Coil** - mentett ellenállás;
* **TCR** - az érték szerkeszthető, ha a Joyetech TC algoritmus van kiválasztva egyedi TCR-rel;
* **T. Dom** - hőmérséklet domináns beállítás, TC esetén a főképernyőn egyből a hőmérséklet állítható be;
* **Preheat** - előfűtés VW módhoz, használható egyszerű érték vagy teljesítménygörbe;
* **PI-Reg** - PI szabályzó TC-hez, javítja a teljesítmény és a hőmérséklet stabilitását (helyes beállítás esetén):
     - PI-Reg On/Off - váltás az eredeti Joyetech és a PI szabályzás között;
     - Range - 0..100% - az a hőmérsékletsáv, ahol a PI szabályzó aktív. Ha a beállított érték 0, a szabályzó mindig aktív, ha az érték például 20%, a PI szabályzás akkor kapcsol be, ha a tekercs hőmérséklete elérte a profilban beállított érték 20%-át;
     - P - proporcionális (arányos) tag, minél nagyobb, annál nagyobb a teljesítményváltozás, érzékenyebb a szabályzó. Túl nagy érték esetén a szabályzás instabillá válhat.;
     - I - integráló tag, minél nagyobb, annál simább, annál kevésbé hullámzó a teljesítmény. Érdemes figyelni a túllövésre.
	 
### Screen Menu

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - Mod felébresztése a +/- gombokkal;
* **Logo** - Logó mutatása a főképernyőn;
* **Clock**
     - **Type** - Analóg vagy Digitális óra;
     - **On Main** - Megjelenítés a főképernyőn;
     - **Saver** - Megjelenítés képernyővédőként;
* **Timeouts**
     - **Dim** - Várakozás a képernyő kikapcsolása előtt;
     - **Dim** ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - várakozás a képernyő kikapcsolása előtt lezárt állapotban;
     - **Logo** - Várakozás a logó megjelenítése előtt;
     - **Clock** - Várakozás az óra megjelenítése előtt;
* **Charge**
     - **Type** - Töltési képernyő stílusa, alap vagy bővített;
     - **Add.** - Plusz elem, óra vagy logó;
* **Stealth** - képernyő beállítások Lopakodó módhoz:
     - **Charge** - Töltési képernyő megjelenítése;
     - **Saver** - Képernyővédő megjelenítése;
     - **ClkOnF** - Ha az óra engedélyezve van a kezdő képernyőn, akkor a tűzgomb egyszeri megnyomására megjeleníti azt;
* **Contrast** - kijelző fényerejének megváltoztatása;
* **Skin** - főképernyő stílusának megváltoztatása.

### Settings Menu

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - teljesítmény változtatása 1W léptékkel;
* **Clicks** - kattintásokhoz rendelhető műveletek
     * **2/3/4x tűzgomb megnyomás**:
          - Semmi;
          - Edit Main - a Joyetech eredeti beállítása 3x tűzgombnyomásra;
          - Main Menu - belépés a főmenübe, mint a tűz/+ gombkombinációval;
          - Preheat - aktuális profil előfűtésének beállítása;
          - Profiles - profilválasztó;
          - Edit Profile - belépés a profil menübe;
          - T. Dom - hőmérséklet domináns mód ki/be kapcsolása;
          - Clock - mutassa/rejtse el az órát a főképernyőn;
          - Info - Infó képernyő mutatása;
          - Reset Cnt. - Mutassa a slukk statisztikát a nullázás lehetőségével;
          - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) Bank - Power Bank üzemmód;
          - Coil ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - TC módban az ellenállás lezárása/feloldása;
          - Key ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - Billentyűzár be/ki kapcsolása;
          - Stealth - Lopakodó mód be/ki kapcsolása;
          - Smart On/Off - Smart mód be/ki kapcsolása;
          - LSL - switch light sleep mode on/off;"light sleep" mód ki/be kapcsolása;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - Eszköz lezárása/feloldása (összes gombot lezárja, de a készülék bekapcsolva marad);
          - On/Off - mod ki/be kapcsolása;
     * **5x tűzgomb megnyomás**:
          - On/Off - mod ki/be kapcsolása;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - Eszköz lezárása/feloldása (összes gombot lezárja, de a készülék bekapcsolva marad);
* **Smart** - automatikus profilváltás beállítása:
     - Off/On/Lazy - Smart mód viselkedés, Lazy azt jelenti, hogy csak akkor vált profilt, ha a kazáncsere éber állapotban történik;
     - Range - ellenállás tolerancia;
* **Clock** - valós idejű óra beállítása;
     - Date/Time - dátum és idő beállítása;
     - Adjust Time - idó precíz beállítása 1mp-s léptékkel;
     - LIRC Speed - Beépített X32 kristály nélküli modoknál a LIRC oszcillátor sebességének a beállítása;
* **Expert** - beállítások haladó felhasználóknak:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/pp3TTaR.png)

* **USB**
     - NoSlp - ne lépjen mély alvás módba, USB csatlakozás esetén;
     - Charge - az eszköz töltse az akkumulátort, miközben USB-n csatlakozik (csak több akkumulátoros készülék esetén);
* **BVO** - cellafeszültség offset;
* **BATT** - cellakisülési profil;
* **SHUNT** - ellenállásmérés korrekciója;
* **ChkTCR** - ellenőrizze a tekercs anyagának TCR értékét, az opciót kikapcsolva vastag huzal, nagy fémtömeg esetén megszűnik a "TCR error" hibaüzenet;
* **RCOBC** - számlálók resetelése akkucsere esetén, törli a használati statisztikákat;számlálók resetelése akkucsere esetén, törli a használati statisztikákat;
* **RTC** - Valósidejű óra:
     - LXT - Teljes hardwares támogatás (X32);
     - LIRC - Másodlagos oszcillátpr használata (pontatlan lehet);
     - LSL - Szoftveres emuláció. Több energiát fogyaszthat, mert a mod nem megy valódi mély alvásba, viszont ugyanolyan pontos, mint az RTC-vel rendelkező modok;  
     ***Megjegyzés***: RTC mód váltása után húzd le az USB-t és indítsd újra a modot úgy, hogy kiveszed az akkumulátort kb 30mp-re.
* **TEMP** - panel hőmérsékleti szenzor, Ext - thermistor, Int - MCU;
* **D. Sleep** - Mély alvás(3 perc inaktivitás után) mód:
     - Std - Normál mély alvás;
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - a mod kikapcsolása;
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - a mod zárolása.

### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Avatar RC átalakító és hasonló támogatott. 5 V és 2.1 A eszköz használható. A töltés elkezdéséhez tedd fel az átalakítót, csatlakoztasd az eszközt, és nyomd meg a tűzgombot. Power Bank mód autómatikusan kikapcsol, ha a töltőáram nem éri el az 50 mA-t (A villogó "On" felirat jelzi). A töltés leállításához nyomd meg a tűzgombot.
Power Bank módból kilépni a tűzgomb vagy a + és - gomb hosszanti nyomásával lehet.

### Info Screen

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Rövid HW információ és némi statisztika.

### Köszönet:

* **TBXin** - NFE projekt, és kapcsolódó fejlesztések
* **Zinger** - Grafikák, ötletek, tesztelés
* **ArionWT** - Grafikák, ötletek, tesztelés
* **ClockSelect** - Nagyszerű myevic projek

# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.

# Támogatás:
Ha szeretnéd támogatni a projektet, ezzel segítve a fejlesztésben, akkor itt megteheted egy általad választott összeggel: [támogatás](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE).
