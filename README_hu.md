# ArcticFox
*Az [NFE Team](http://nfeteam.org) egyedi firmware-e Joyetech, Wismec and Eleaf modokhoz*

![](http://i.imgur.com/JP4KC8A.png)
![](http://i.imgur.com/E1e7cs1.png)

![](http://i.imgur.com/kYJcp6I.png)
![](http://i.imgur.com/TnqNYK1.png)
![](http://i.imgur.com/0XTV9xD.png)

**A firmware az [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) seg�ts�g�vel [t�lthet� fel](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) a modra �s konfigur�lhat�.**

## T�mogatott eszk�z�k:
### Joyetech:
* eVic VTC Mini
* eVic VTC Dual
* eVic VTwo Mini
* eVic VTwo
* eVic AIO
* eVic Basic
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
* VF Lite
* VF Stout
* VF Classic
* BV Centurion
* La Petite Box

### Eleaf:
* Aster
* iStick Pico 75W
* iStick Pico Mega 80W
* iStick Pico Dual
* iStick TC100W
* iStick TC200W
* iStick iPower 80W

## Profiles
A f� k�l�nbs�g az eredeti Joyetech firmware-hez k�pest, hogy a felhaszn�l�i fel�let a DNA-hoz hasonl�an profil alap� �s nagyobb hangs�ly ker�lt a testreszabhat�s�gra.
A profil a kaz�n k�l�nb�z� param�tereinek egy�ttese, mint a tekercs anyaga, ellen�ll�sa, teljes�tm�ny �s h�m�rs�klet adatok.
8 k�l�nb�z� profil �ll rendelkez�sre, melyek a NFE Toolbox seg�ts�g�vel hozhat�k l�tre �s szerkeszthet�k, a kedvenc kaz�njainkhoz szabva.

![](http://i.imgur.com/UjtY7Ir.png)

A profilok a tekercs ellen�ll�sa alapj�n automatikusan vagy manu�lisan v�lthat�k. Az automatikus �tkapcsol�s haszn�lat�hoz csak a "Smart" m�dot kell enged�lyezni, majd csatlakoztatni a kaz�nt �s hozz�rendelni a k�v�nt profilhoz.

![](http://i.imgur.com/fadryzQ.png)

Ha k�s�bb ezt a kaz�nt tekerj�k a modra, a hozz�rendelt profil automatikusan aktiv�l�dik.
Ha a csatlakoztatott kaz�n ellen�ll�s�hoz nem tal�lhat� kor�bban hozz�rendelt profil, l�tre kell hoznunk egy �jat, vagy hozz�rendelhetj�k egy m�r megl�v� profilhoz.
Ha manu�lisan v�ltunk egy olyan profilra, amely m�r rendelkezik kor�bban mentett ellen�ll�ssal, de nem passzol az aktu�lisan haszn�lt kaz�nhoz, lehet�s�g�nk van friss�teni a profilt, vagy megtartani a kor�bbi �rt�ket.

## Main Menu

Tartsd nyomva a t�z �s a plusz gombot 1 m�sodpercig a men�be val� bel�p�shez

![](http://i.imgur.com/XSWOLDJ.png)

## Profile Menu

![](http://i.imgur.com/HOO0KiF.png) ![](http://i.imgur.com/2UPcLHy.png) ![](http://i.imgur.com/yNH5crk.png) ![](http://i.imgur.com/kc0PYf7.png) ![](http://i.imgur.com/CNzn7vQ.png) ![](http://i.imgur.com/3MHoldt.png)

* **Wire** - huzal anyaga, TC vagy sem (VW), be�ll�that� standard vagy felhaszn�l� �ltal l�trehozott TFR g�rbe;
* **Coil** - mentett ellen�ll�s;
* **TCR** - az �rt�k szerkeszthet�, ha a Joyetech TC algoritmus van kiv�lasztva egyedi TCR-rel;
* **T. Dom** - h�m�rs�klet domin�ns be�ll�t�s, TC eset�n a f�k�perny�n egyb�l a h�m�rs�klet �ll�that� be;
* **Preheat** - el�f�t�s VW m�dhoz, haszn�lhat� egyszer� �rt�k vagy teljes�tm�nyg�rbe;
* **PI-Reg** - PI szab�lyz� TC-hez, jav�tja a teljes�tm�ny �s a h�m�rs�klet stabilit�s�t (helyes be�ll�t�s eset�n):
     - PI-Reg On/Off - v�lt�s az eredeti Joyetech �s a PI szab�lyz�s k�z�tt;
     - Range - 0..100% - az a h�m�rs�klets�v, ahol a PI szab�lyz� akt�v. Ha a be�ll�tott �rt�k 0, a szab�lyz� mindig akt�v, ha az �rt�k p�ld�ul 20%, a PI szab�lyz�s akkor kapcsol be, ha a tekercs h�m�rs�klete el�rte a profilban be�ll�tott �rt�k 20%-�t;
     - P - proporcion�lis (ar�nyos) tag, min�l nagyobb, ann�l nagyobb a teljes�tm�nyv�ltoz�s, �rz�kenyebb a szab�lyz�. T�l nagy �rt�k eset�n a szab�lyz�s instabill� v�lhat.;
     - I - integr�l� tag, min�l nagyobb, ann�l sim�bb, ann�l kev�sb� hull�mz� a teljes�tm�ny. �rdemes figyelni a t�ll�v�sre.

## Screen Menu

![](http://i.imgur.com/6jddZL9.png) ![](http://i.imgur.com/3fRgkGN.png) ![](http://i.imgur.com/FmVjNro.png) ![](http://i.imgur.com/2UYldpC.png)

* **Dim** - mennyi id� alatt halv�nyodjon el a kijelz�;
* **Wake <>** - mod fel�breszt�s +/- gombokkal;
* **Charge** - mutasson plusz inform�ci�t t�lt�s k�zben, cellafesz�lts�g, panel h�m�rs�klete;
* **Logo** - mutassa a log�t a f�k�perny�n;
* **Clock** - �ra be�ll�t�sai:
     - Type - anal�g vagy digit�lis;
     - On Main - mutassa az �r�t a f�k�perny�n;
     - Saver - mutassa az �r�t standby m�dban;
* **Selector** - mutasson plusz profil inform�ci�kat a "Select Profile" k�perny�n;
* **Contrast** - kijelz� f�nyerej�nek v�ltoztat�sa;
* **Skin** - f�k�perny� st�lus�nak megv�ltoztat�sa.

## Settings Menu

![](http://i.imgur.com/aDuSk3n.png) ![](http://i.imgur.com/3JeWUqf.png) ![](http://i.imgur.com/8V1VCeo.png)

* **1 Watt** - teljes�tm�ny v�ltoztat�sa 1 Wattal;
* **Menu** - New - profilv�lt�s a +/- gombok haszn�lat�val, Old - v�lt�s "Edit Main" gombnyom�ssal (3x t�z);
* **Smart** - automatikus profilv�lt�s be�ll�t�sa:
     - On/Off;
     - ellen�ll�s tolerancia;
     - mutassa a profil men�t �j hozz�rendel�s eset�n;
* **Clicks** - 2/3/4 t�zgombnyom�shoz rendelhet� m�veletek:
     - semmi;
     - Edit Main - a Joyetech eredeti be�ll�t�sa 3x t�zgombnyom�sra;
     - Profiles - profilv�laszt�;
     - T. Dom - h�m�rs�klet domin�ns m�d ki/be kapcsol�sa;
     - Clock - mutassa/rejtse el az �r�t a f�k�perny�n;
     - On/Off - mod ki/be kapcsol�sa;
     - LSL - "light sleep" m�d ki/be kapcsol�sa;
     - Main Menu - bel�p�s a f�men�be, mint a t�z/+ gombkombin�ci�val;
     - Preheat - aktu�lis profil el�f�t�s�nek be�ll�t�sa;
     - Edit Profile - bel�p�s a profil men�be;
     - Smart On/Off;
     - Mutassa az info k�perny�t.
* **RTC** - realtime clock be�ll�t�sa;
* **Expert** - be�ll�t�sok halad� felhaszn�l�knak:

![](http://i.imgur.com/UZBrHjJ.png) ![](http://i.imgur.com/7fT0pNi.png) ![](http://i.imgur.com/edejq3z.png) ![](http://i.imgur.com/FoH1vaE.png)

* **USB**
     - NoSlp - ne l�pjen m�ly sleep m�dba, USB csatlakoz�s eset�n;
     - Charge - az eszk�z t�ltse az akkumul�tort, mik�zben USB-n csatlakozik;
* **BVO** - cellafesz�lts�g offset;
* **BATT** - cellakis�l�si profil;
* **SHUNT** - ellen�ll�sm�r�s korrekci�ja;
* **ChkTCR** - ellen�rizze a tekercs anyag�nak TCR �rt�k�t, az opci�t kikapcsolva vastag huzal, nagy f�mt�meg eset�n megsz�nik a "TCR error" hiba�zenet;
* **RCOBC** - sz�ml�l�k resetel�se akkucsere eset�n, t�rli a haszn�lati statisztik�kat;
* **X32** - RTC modul haszn�lja a m�sodlagos 32768 Hz-es oszcill�tort, ha van ilyen a modban;
* **LSL** - Light Sleep Mode, m�sodlagos oszcill�torral nem rendelkez� k�sz�l�kek eset�n pontosabb RTC. N�mi energi�t vesz ig�nybe standby m�dban ez�rt ! figyelmezteti a felhaszn�l�t az akkumul�tor kijelz� mellett;
* **TEMP** - panel h�m�rs�kleti szenzor, Ext - thermistor, Int - MCU


## Info Screen
![](http://i.imgur.com/2QoKfkX.png)

R�vid HW inform�ci� �s n�mi statisztika.

### K�sz�net:
     * TBXin - for NFE Products, ideas and tests
     * Zinger - for graphics, ideas and tests
     * ClockSelect - for great project called myevic

### Ford�totta:
     * balazsk

# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.

# T�mogat�s:
Ha szeretn�d t�mogatni a projektet, ezzel seg�tve a fejleszt�sben, akkor itt megteheted egy �ltalad v�lasztott �sszeggel: [t�mogat�s](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE).
