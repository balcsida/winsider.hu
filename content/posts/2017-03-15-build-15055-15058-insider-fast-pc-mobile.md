---
title: 'Megjelent a 15055-ös build Insider Fast Ringen (PC & Mobile) és a 15058-as build PC-n!'
author: Decsi Balázs
type: post
date: 2017-03-15T19:35:04+00:00
url: /2017/03/15/build-15055-15058-insider-fast-pc-mobile/
featured_image: /wp-content/uploads/2017/03/insider.png
instant_articles_submission_id:
  - 352800078448322
categories:
  - Insider
  - Windows 10
  - Windows 10 Mobile
tags:
  - Insider Fast
  - Mobil
  - PC
  - Windows 10
  - windows 10 mobile

---
_**Szerkesztői megjegyzés:** Egyetemi elfoglaltság miatt nem sikerült időben megírni a magyar összefoglalót időben, ezért most együtt lesz az utolsó két frissítés tárgyalva._

Péntek este a redmondi óriás kiadta a tesztelőinek a következő Windows 10 iterációnak (Alkotói Frissítés) újabb előzetes verzióját. Ami a legfontosabb változás, hogy a verzió szám hivatalosan is változott, tehát az alkotói frissítés a 1703-as verziószámot kapja.

Ezen felül kedd éjszaka a megörvendeztettek minket még egy előzetessel, ám ez egyelőre csak PC-re érhető el. Mivel közel végleges már a rendszer, csak hibajavításokat kaptunk mindkét esetben. Lássuk mik ezek:

<!--more-->

## Build 15055:

### Változások és hibajavítások PC verzió esetében:

  * Symantec/Norton antivírust használóknak jó hír, hogy a frissítés során nem fognak hibába ütközni, viszont ahhoz, hogy telepíteni tudják a 15055-ös frissítést a legfrissebb verzióval kell rendelkezniük a fenti antivírussal.
  * Telepítés közben nem fog hibára futni 71%-nál.
  * Ha rendelkezel egyéb nyelvi csomagokkal telepítés előtt nem kell eltávolítani őket.
  * Javítva lett a hiba, ha egy elgépelt szavon van jobb klikkelés után a &#8220;context menü&#8221; rossz helyen vagy az aktív ablak mögött jelent meg.
  * Microsoft Edge-ben a Továbbítás másik eszközre opciót használva ismét megnyílik a Csatlakozás sáv.
  * Javítva lett a hiba, ami miatt link megnyitása vagy beillesztése után lefagyott az MS Edge
  * Javítva lett a hiba, ami miatt a képernyőn maradt az előnézeti képe egy lapnak, akár még a bezárása után is.
  * Javítva lett a hiba, ami miatt az oldalakat le akarta tölteni az MS Egde, nem pedig megnyitni, ha a uBlock Origin kiegészítő aktív volt.
  * Ismét használható a Webjegyzet funkció szövegbeviteli része érintőképernyős használat esetén.
  * Ismét be lehet csukni minden hiba nélkül lapokat MS Edge-ben &#8220;CTRL + W&#8221;-t használva.
  * Javítva lettek a szövegbeillesztési hibák MS Edge-ben.
  * Javítva lett a hiba, ami miatt ha MS Edge ablaka volt előtérben a touchpad-del és a billentyűzettel való navigálás rendszeresen befagyott néhány másodpercre.
  * A több monitoros megjelenítés ismét elvárás szerint működik.
  * Javítva lett a Groove zene lejátszási hibája, ami miatt méretváltást nem követte a felülete.
  * Javítva lett a tálcán az alkalmazások előnézeti képének hibája
  * Javítva lett egyes USB-s tápellátású monitorokon a befagyó óra hiba
  * Javítva lett az akkumulátor felugró felületének összeomlása a második klikkelés után.
  * Javítva lett a OneDrive.exe indokolatlanul magas processzor használata
  * Ismét be lehet illeszteni azokat a szövegeket, amiket felfüggesztett UWA alkalmazásokból másoltak ki.
  * Javítva lett a hiba, ami miatt nem voltak felfedezhetők bizonyos eszközök Bluetooth-on keresztül.
  * Javítva lett a nyomtatás hibája UWA alkalmazások esetében.
  * Javítva lett a további beállítások szöveg egyes esetekben szürke színnel való megjelenítése.
  * Javítva lett a hiba ami miatt a Defender értesítéseire kattintva nem nyílt meg a program.
  * Javítva lett a Microsoft Visual C++ keretrendszer hibás működése egyes Insider-ek esetében.

### Ismert hibák PC esetében:

  * Egyes gépek nem tudnak 15002 és nagyobb verzióra frissülni egy hiba miatt.
  * Egyes alkalmazások nem indulnak el a Hirdetési azonosító hibája miatt. Ez a későbbi frissítések esetén is megmarad. A következő registry kulcs törlésével megoldható: &#8220;HKCU\Software\Microsoft\Windows\CurrentVersion\AdvertisingInfo&#8221;
  * Egy hiba miatt egyes beépített alkalmazások nem futtathatók, valamint frissítések nem telepíthetők az Áruházból. Ilyen esetben az alkalmazást alaphelyzetbe kell állítani, második esetben letörölni majd ismét telepíteni.
  * Egy hiba miatt nem értesít a rendszer, ha egyéb frissítés miatt újra kell indítani a számítógépet.
  * Egyes UWA alkalmazások esetében a címsorban továbbra is a csomagnevük jelennek meg.
  * Egyes hardver konfigurációk esetén zölden villoghat a Game Bar-on belül a “Live review” ablak közvetítés közben, ám ez csak a közvetítőnél látszik.
  * Hibák léphetnek fel MS Edge-ben ha F12-es eszközt használva böngésszük a honlapokat.
  * Ha meg van nyitva az F12-es fejlesztői eszközök MS Edge-ben majd újra megnyomom az F12, akkor a lap, amihez meg volt nyitva nem kerül az előtérbe, valamint ha nem volt megnyitva, és megnyitom, akkor az sem kerül előtérbe.
  * Surface Pro 3 esetében, ha SD kártya csatlakoztatva van a géphez frissítés nem telepíthető. A frissítés idejére el kell távolítani, majd utána ismét lehet csatlakoztatni.

### Változások és hibajavítások Mobil esetében:

  * Javítva lett a hiba ami miatt miatt a hangerő állítás nem működött tovább Grove Zene esetében egy végponti változás után (mint például fejhallgató bedugása).
  * Fejlesztettünk a beszéd megbízhatóságán, valamint javítottuk Cortana csatlakozási hibáját.
  * Javítva lett a hiba ami miatt a többkörös beszélgetések Cortana-val nem működtek.

### Ismert hibák Mobil esetében:

  * Egy hiba miatt egyes alkalmazások háttér folyamatai nem futnak le (ilyen pl a OneDrive fotó szinkronizációja).
  * Ha váratlanul újraindul a készüléked elveszhetnek a híváslista, üzenet és e-mail előzményeid.
  * Egyes beépített alkalmazások nem indíthatóak el és a frissítések sem telepíthetők Áruházból. Újratelepítéssel a frissítések telepíthetők, ám a másik hibára nincs jelenleg megoldás. A következő build-ben ezek javítva lesznek.
  * Beszéd csomagokat esetleg nem lehet letölteni ezen a build-en.
  * MS Edge-ben egyes Insider-ek esetében folyamatosan újratöltődhetnek a lapok.

## Build 15058:

### Változások és hibajavítások:

  * Javítva lett a beépített alkalmazások indítási hibája, valamint ismét lehet frissítéseket telepíteni az Áruházból.
  * Javítva lett a címsorban lévő név hibás megjelenítése.
  * Javítva lett a hiba, ami miatt visszalépett az előző oldalra az MS Edge, ha át lett méretezve, vagy rögzítve a képernyő szélére.
  * Javítva lett a hiba, ami miatt az egér mutatója teljes kijelzős videó lejátszás közben nem tűnik el MS Edge-ben
  * Javítva lett a hiba, ami miatt összeomlott a Gépház, ha a Wi-Fi beállításokat a Gépházból nyitottuk meg.
  * Javítva lett a hiba, ami miatt a fiók zárolása után ismét bejelentkezve az összes megnyitott alkalmazás és dokumentum bezáródott vagy hibajelzéssel nem lehetett bejelentkezni a fiókba.
  * Javítva lett a hiba, ami miatt, egy titkosított PDF file átnevezése után visszaállt az MS Edge alapméretezett PDF olvasó alkalmazásnak.
  * Javítottuk a videó lejátszás minőségét a cél eszközön, ha vezetéknélküli Miracast kapcsolaton keresztül egy magas DPI beállítású PC-ről egy másik magas DPI beállítású eszközre van kiküldve a kép.

### Ismert hibák:

  * Egyes gépek nem tudnak 15002 és nagyobb verzióra frissülni egy hiba miatt.
  * Egyes alkalmazások nem indulnak el a hirdetési azonosító hibája miatt. Ez továbbfrissítve is megmarad. A következő registry kulcs törlésével megoldható: &#8220;HKCU\Software\Microsoft\Windows\CurrentVersion\AdvertisingInfo&#8221;
  * Egy hiba miatt nem értesít a rendszer, ha egyéb frissítés miatt újra kell indítani a számítógépet.
  * Egyes hardver konfigurációk esetén zölden villoghat a Game Bar-on belül a “Live review” ablak közvetítés közben, ám ez csak a közvetítőnél látszik.
  * Hibák léphetnek fel MS Edge-ben ha F12-es eszközt használva böngésszük a honlapokat cross-origin iframes-el.