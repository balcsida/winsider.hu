---
title: 'Megjelent a 15063-as Build Insider Fast-ra (PC & Mobile)'
author: Decsi Balázs
type: post
date: 2017-03-23T10:51:57+00:00
url: /2017/03/23/build-15063-insider-fast-pc-mobile/
categories:
  - Insider
  - Windows 10
  - Windows 10 Mobile
tags:
  - Build 15063
  - Insider Fast
  - Windows 10
  - windows 10 mobile

---
![](/wp-content/uploads/2017/03/build15063.jpg)

A hét jól indult, hiszen hétfőről keddre virradó éjszaka elérhetővé tették a címben említett előzetest. Ez egy várva várt frissítés (főleg mobilos szemszögből) hiszen egy nagyon idegesítő hibát is javított. Megjegyzendő, hogy PC-n (ismét) eltűnt a vízjel a jobb alsó sarokkból valamit, az &#8220;időzített bomba&#8221; (licensz lejárata) is, ahogy a fenti képen látható, ami erősen utalhat rá, hogy ez lesz az RTM verzió. (Ezt tovább erősítheti az, hogy egyes Release Preview körön lévő emberek is megkapták ezt a verziót. Jelenleg ezt sem megerősíteni sem cáfolni nem tudom, mert nem rendelkezem RP körön lévő eszközzel. Kommentekben várjuk a tapasztalataitokat ezzel kapcsolatban.) Lássuk mit kapunk ebben a buildben:

<!--more-->

### Javítások és változások PC esetében:

  * Javítva lett a hiba, ami miatt a Microsoft Edge befagyását okozta.
  * Javítva lett a hiba, ami esetében nem települtek a lokalizált file-ok és registry bejegyzések, ha .Net Framwork 3.5-ös verziója  engedélyezve lett.

### Ismert hibák a PC-s verzió esetében:

  * 14393-as buildről az egyenes frissítési lehetőség szerdától (március 22) él.
  * Nem lehet letölteni egyéb nyelvi csomagokat. A korábban letöltötteket ez nem befolyásolja.
  * Ha a telepítés közben 8024a112 hibát dob a rendszer, manuálisan indítsd újra. Ha újraindítás közben úgy tűnik megfagyott, akkor kapcsold ki a számítógépet, majd újra be. A telepítés folytatódni fog.
  * Egyes Insiderek esetében a “Some updates were cancelled. We’ll keep trying in case new updates become available” hiba jelent meg Windows Update-ben. A következő registry kulcsot kell törölni a hiba javításához: “HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate\Auto Update\RequestedAppCategories\8b24b027-1dee-babb-9a95-3517dfb9c552”  
    További információ [ITT][1] található
  * Egyes alkalmazások nem indulnak el a hirdetési azonosító hibája miatt. Ez továbbfrissítve is megmarad. A következő registry kulcs törlésével megoldható: “HKCU\Software\Microsoft\Windows\CurrentVersion\AdvertisingInfo”
  * Egy hiba miatt nem értesít a rendszer, ha egyéb frissítés miatt újra kell indítani a számítógépet.
  * Egyes hardver konfigurációk esetén zölden villoghat a Game Bar-on belül a “Live review” ablak közvetítés közben, ám ez csak a közvetítőnél látszik.

### Változások és javítások mobil esetében:

  * Javítva lett a hiba, ami miatt egyes beépített alkalmazások  nem indultak el, valamint áruházból nem lehetett frissítéseket telepíteni. (Szerk.: Ez csak HR utánjavult meg nekem.)
  * Javítva lett az alkalmazások háttérfolyamatainak futását megakadályozó hiba.
  * Javítva lett az üzenetek elvesztését okozó hiba.
  * Beszéd csomagokat ismét az elvártak szerint le lehet tölteni.
  * Javítva lett bizonyos autók esetén a Bluetooth kapcsolat hibája.
  * ### Javítva lett az alapméretezett APN módosításának hibája

### Ismert hibák mobil esetében:

  * Az egyenes frissítés nem lehetséges Évfordulós Frissítésről. Először a 15055-ös build fog települni, utána pedig a 16063-as.
  * MS Edge-ben egyes Insider-ek esetében folyamatosan újratöltődhetnek a lapok.
  * Bluetooth kapcsolódási gondok léphetnek fel egyes Insider-eknél, valamint új bluetooth eszközt sem tudnak hozzáadni a készülékükhöz.

 [1]: https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install/pc-build-install-some-update-were-cancelled/22d428c1-7ce8-4d12-b7bf-2e21c08c0549?tm=1489615923416