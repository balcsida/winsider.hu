---
title: Windows 10 Mobile Registry módosítása nem támogatott készülékek frissítése érdekében.
author: Decsi Balázs
type: post
date: 2017-08-24T20:50:23+00:00
excerpt: A következő leírás azoknak kíván segíteni, akik Windows 10 Mobile operációs rendszert használnak, és a már nem támogatott készüléküket szeretnék a legfrissebb verzióra frissíteni
url: /2017/08/24/windows-10-mobile-registry-modositasa/
categories:
  - Insider
  - Mobile
  - Szoftver, App
  - Windows 10 Mobile
tags:
  - windows 10 mobile

---
Mielőtt bármibe is belekezdenénk, az oldal nevében leszögezem, hogy a következő művelet helytelen elvégzése kárt tehet a készülékedben. Esetleges károkért az oldal **semmilyen felelősséget nem vállal!**

A következő leírás azoknak kíván segíteni, akik Windows 10 Mobile operációs rendszert használnak, és a már nem támogatott készüléküket szeretnék a legfrissebb verzióra frissíteni (a cikk írásának időpontjában a hivatalos (Production ring) 15063.540, Slow Ring 15240.0, Fast Ring 15240.0). A cikkben közölt képek segítik a leítak megértését. A szükséges beavatkozás helyét piros vonallal aláhúzva jelöltük.

Első feladatunk, hogy a bekapcsoljuk a fejlesztői lehetőségeket. Ezt a Gépházban az Update & Security (Frissítés & Biztonság) -> For developers () helyen tudjuk megtenni. Itt a harmadik pontot kell kiválasztanunk (Developer mode, Fejlesztői mód). Itt más dolgunk nincs is.

![](/wp-content/uploads/2017/08/registry1-1024x768.jpeg)

Majd Store-ból (Áruházból) telepítsük fel az Interop Tools (Preview) nevű appot: [link][1].

![](/wp-content/uploads/2017/08/wp_ss_20170821_0004-576x1024.png)

A következő dolgunk a letölteni a további szükséges programokat, amik nincsenek fenn az áruházban. Ezen a OneDrive linken éritek el őket, igyekszünk mindig a legfrissebb verziókat itt elérhetővé tenni: [link][2]. Ezeket (ha mindent egyben töltöttünk le, akkor csomagoljuk ki) másoljuk fel a telefonra (belső tároló és SD kártya is jó).

A filekezelőben keressük meg a Dependencies/ARM mappát, majd a benne lévő négy kiegészítőt telepítsük fel. Ezután a Providers mappában lévő két app következik.

![](/wp-content/uploads/2017/08/registry2-1024x768.jpeg)![](/wp-content/uploads/2017/08/registry3-1024x379.jpeg)

Ha ezzel megvagyunk, akkor indítsuk el az Interop Tools (Preview) nevű programot. A program minden telefonon és minden nyelven csak angolul használható. Az első indítás során először el kell fogadnunk a Licenszmegállapodást (End user license agreement), az “Agree” (Beleegyezés) gomb megnyomásával, majd következő oldal az újdonságok (What’s new?) leírása. Itt a “Next” gombbal léphetünk tovább.

![](/wp-content/uploads/2017/08/inkedregistry4-1-1024x768.jpg)

Ezután engedélyezzük az alkalmazás hozzáféréseit a felhasználói fiókunkhoz. Később ezt meg lehet változtatni, az én tapasztalatom az, hogy mivel az alkalmazás akár a telefonunk téglásítását okozhatja, ezért ez egy védelmi vonalként fogható fel (későbbiekben lesz róla szó miért), személyes adatot nem gyűjt az alkalmazás. A “Yes” (Igen) gombra koppintsunk rá. A következő lapon a Registry-hez való hozzáférés módját válasszuk ki, a legördülő menüből válasszuk a “This device (Through provider extensions)” lehetőséget a “Use the selected provider” gomb megnyomásával.

![](/wp-content/uploads/2017/08/inkedregistry5-1-1024x512.jpg)

Ha PIN kóddal vagy Windows Hello-val védve van a készülékünk akkor adjuk meg a kódot, illetve mutassuk meg a telefonunknak a retinánkat. 🙂 A következő lapon a “Select the best provider automatically”  lehetőséget jelöljük ki (alapméretezetten ezt fogja felajánlani a program, majd nyomjunk rá az “Ok” gombra.

![](/wp-content/uploads/2017/08/inkedregisrty6-1024x512.jpg)

Ha mindent jól csináltunk, akkor az alant látható főképernyő köszön vissza nekünk.

![](/wp-content/uploads/2017/08/inkedregistry5-576x1024.jpg)

Felül a három vízszintes vonalra (Hamburger ikon) koppintva a menüt hozhatjuk elő. Válasszuk a “Registry” lehetőséget, majd a “Registry Browser” menüpontot. Ha mindent jól csináltunk akkor most megjelenik előttünk a telefonunk Registry-jének gyökérkönyvtára.
Itt a következő utat kell végigjárnunk: **HKEY\_LOCAL\_MACHINE (HKLM) **–> **SYSTEM **–> **Platform **–> **DeviceTargetingInfo**.

![](/wp-content/uploads/2017/08/inkedregistry7-1024x1024.jpg)

Itt négy értéket kell átírnunk. Fontos, hogy mindenki a saját készülékének megfelelő értékeket válassza, azaz akinek egy SIM-es készüléke van az a Lumia 950XL adatait (“Egy SIM-es készülékek esetén”), míg a két SIM-es készülékek tulajdonosai a Lumia 950XL Dual SIM adatait (“Dual SIM-es készülékek esetén”) használják.

![](/wp-content/uploads/2017/08/inkedregistry8-576x1024.jpg)

A módosítás előtt érdemes az eredeti értékeket lementeni (képernyőmentés, stb.), hogy ha valami problémába futunk, akkor alaphelyzetbe állítás nélkül vissza tudjuk írni az eredeit értékeket. Természetesen egy alaphelyzetbe állítás, vagy WDRT (Windows Device Recovery Tool) az általunk elvégeztt módosításokat felülírja, és újra el kell végeznünk. Ezeket kell átírnunk a Registry-ben (az adott pontra koppintunk, átírjuk az értéket, majd allul a pipával véglegesíthetjük a módosításokat, a szükséges értékek idézőjelben félkövérrel vannak szedve, a beviteli mezőbe (Registry Value Data) idézőjelek nélkül kell beírni, a bejegyzés típusát (Registry Value Type) a legördülő menüben ne változtassuk meg):

![](/wp-content/uploads/2017/08/inkedregistry11-576x1024.jpg)

“PhoneManufacturer” = “**MicrosoftMDG**”

“PhoneManufacturerModelName” = “**RM-1085_11302**” (Egy SIM-es készülékek esetén)**; “****RM-1116\_11258**” (Dual SIM-es készülékek esetén)

“PhoneModelName” = “**Lumia 950 XL**” (Egy SIM-es készülékek esetén); “**Lumia 950 XL Dual SIM**” (Dual SIM-es készülékek esetén)

“PhoneHardwareVariant” = “**RM-1085**” (Egy SIM-es készülékek esetén), “**RM-1116**” (Dual SIM-es készülékek esetén)

Ha mindezeket elvégeztük akkor a Gépház -> Rendszer -> Névjegy oldalon az alábbiakat fogjuk látni (a képernyőkép egy Lumia 930-on készült) és bátran kereshetünk frissítéseket a Windows Update-en keresztül. 🙂

![](/wp-content/uploads/2017/08/registry12-576x1024.jpg)

Sok sikert mindenkinek!

 [1]: https://www.microsoft.com/hu-hu/store/p/interop-tools-preview/9ntgwlc0d3cs?wa=wsignin1.0&rtc=1
 [2]: https://1drv.ms/f/s!Auqwa8v1qfFSgblVIYx8ojlmekUxiA