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
Mielőtt bármibe is belekezdenénk, az oldal nevében leszögezem, hogy a következő művelet helytelen elvégzése kárt tehet a készülékedben. Esetleges károkért az oldal <span style="text-decoration: underline"><strong>semmilyen felelősséget nem vállal!</strong></span>

A következő leírás azoknak kíván segíteni, akik Windows 10 Mobile operációs rendszert használnak, és a már nem támogatott készüléküket szeretnék a legfrissebb verzióra frissíteni (a cikk írásának időpontjában a hivatalos (Production ring) 15063.540, Slow Ring 15240.0, Fast Ring 15240.0). A cikkben közölt képek segítik a leítak megértését. A szükséges beavatkozás helyét piros vonallal aláhúzva jelöltük.

Első feladatunk, hogy a bekapcsoljuk a fejlesztői lehetőségeket. Ezt a Gépházban az Update & Security (Frissítés & Biztonság) -> For developers () helyen tudjuk megtenni. Itt a harmadik pontot kell kiválasztanunk (Developer mode, Fejlesztői mód). Itt más dolgunk nincs is.

<img loading="lazy" class="aligncenter wp-image-1490" src="https://winsider.hu/wp-content/uploads/2017/08/registry1-1024x768.jpeg" alt="" width="800" height="600" srcset="https://winsider.hu/wp-content/uploads/2017/08/registry1-1024x768.jpeg 1024w, https://winsider.hu/wp-content/uploads/2017/08/registry1-300x225.jpeg 300w, https://winsider.hu/wp-content/uploads/2017/08/registry1-768x576.jpeg 768w" sizes="(max-width: 800px) 100vw, 800px" /> 

Majd&nbsp;Store-ból (Áruházból) telepítsük fel az Interop Tools (Preview) nevű appot:&nbsp;[link][1].

<img loading="lazy" class="aligncenter wp-image-1493" src="https://winsider.hu/wp-content/uploads/2017/08/wp_ss_20170821_0004-576x1024.png" alt="" width="300" height="533" srcset="https://winsider.hu/wp-content/uploads/2017/08/wp_ss_20170821_0004-576x1024.png 576w, https://winsider.hu/wp-content/uploads/2017/08/wp_ss_20170821_0004-169x300.png 169w, https://winsider.hu/wp-content/uploads/2017/08/wp_ss_20170821_0004-768x1365.png 768w, https://winsider.hu/wp-content/uploads/2017/08/wp_ss_20170821_0004.png 1440w" sizes="(max-width: 300px) 100vw, 300px" /> 

A következő dolgunk a &nbsp;letölteni a további szükséges programokat, amik nincsenek fenn az áruházban. Ezen a OneDrive linken éritek el őket, igyekszünk mindig a legfrissebb verziókat itt elérhetővé tenni: [link][2]. Ezeket (ha mindent egyben töltöttünk le, akkor csomagoljuk ki) másoljuk fel a telefonra (belső tároló és SD kártya is jó).

A filekezelőben keressük meg a Dependencies/ARM mappát, majd a benne lévő négy kiegészítőt telepítsük fel. Ezután a Providers mappában lévő két app következik.

<img loading="lazy" class="aligncenter wp-image-1491" src="https://winsider.hu/wp-content/uploads/2017/08/registry2-1024x768.jpeg" alt="" width="600" height="450" srcset="https://winsider.hu/wp-content/uploads/2017/08/registry2-1024x768.jpeg 1024w, https://winsider.hu/wp-content/uploads/2017/08/registry2-300x225.jpeg 300w, https://winsider.hu/wp-content/uploads/2017/08/registry2-768x576.jpeg 768w" sizes="(max-width: 600px) 100vw, 600px" /><img loading="lazy" class="aligncenter wp-image-1492" src="https://winsider.hu/wp-content/uploads/2017/08/registry3-1024x379.jpeg" alt="" width="600" height="222" srcset="https://winsider.hu/wp-content/uploads/2017/08/registry3-1024x379.jpeg 1024w, https://winsider.hu/wp-content/uploads/2017/08/registry3-300x111.jpeg 300w, https://winsider.hu/wp-content/uploads/2017/08/registry3-768x284.jpeg 768w" sizes="(max-width: 600px) 100vw, 600px" /> 

Ha ezzel megvagyunk, akkor indítsuk el az Interop Tools (Preview) nevű programot. A program minden telefonon és minden nyelven csak angolul használható. Az első indítás során először el kell fogadnunk a Licenszmegállapodást (End user license agreement), az &#8220;Agree&#8221; (Beleegyezés) gomb megnyomásával, majd következő oldal az újdonságok (What&#8217;s new?) leírása. Itt a &#8220;Next&#8221; gombbal léphetünk tovább.

<img loading="lazy" class="aligncenter wp-image-1505" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry4-1-1024x768.jpg" alt="" width="600" height="450" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry4-1-1024x768.jpg 1024w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry4-1-300x225.jpg 300w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry4-1-768x576.jpg 768w" sizes="(max-width: 600px) 100vw, 600px" /> 

Ezután engedélyezzük az alkalmazás hozzáféréseit a felhasználói fiókunkhoz. Később ezt meg lehet változtatni, az én tapasztalatom az, hogy mivel az alkalmazás akár a telefonunk téglásítását okozhatja, ezért ez egy védelmi vonalként fogható fel (későbbiekben lesz róla szó miért), személyes adatot nem gyűjt az alkalmazás. A &#8220;Yes&#8221; (Igen) gombra koppintsunk rá. A következő lapon a Registry-hez való hozzáférés módját válasszuk ki, a legördülő menüből válasszuk a &#8220;This device (Through provider extensions)&#8221; lehetőséget a &#8220;Use the selected provider&#8221; gomb megnyomásával.

<img loading="lazy" class="aligncenter wp-image-1506" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-1-1024x512.jpg" alt="" width="600" height="300" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-1-1024x512.jpg 1024w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-1-300x150.jpg 300w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-1-768x384.jpg 768w" sizes="(max-width: 600px) 100vw, 600px" /> 

Ha PIN kóddal vagy Windows Hello-val védve van a készülékünk akkor adjuk meg a kódot, illetve mutassuk meg a telefonunknak a retinánkat. 🙂 A következő lapon a &#8220;Select the best provider automatically&#8221; &nbsp;lehetőséget jelöljük ki (alapméretezetten ezt fogja felajánlani a program, majd nyomjunk rá az &#8220;Ok&#8221; gombra.

<img loading="lazy" class="aligncenter wp-image-1504" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregisrty6-1024x512.jpg" alt="" width="600" height="300" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregisrty6-1024x512.jpg 1024w, https://winsider.hu/wp-content/uploads/2017/08/inkedregisrty6-300x150.jpg 300w, https://winsider.hu/wp-content/uploads/2017/08/inkedregisrty6-768x384.jpg 768w" sizes="(max-width: 600px) 100vw, 600px" /> 

Ha mindent jól csináltunk, akkor az alant látható főképernyő köszön vissza nekünk.

<img loading="lazy" class="aligncenter wp-image-1499" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-576x1024.jpg" alt="" width="300" height="533" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-576x1024.jpg 576w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-169x300.jpg 169w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5-768x1365.jpg 768w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry5.jpg 1440w" sizes="(max-width: 300px) 100vw, 300px" /> 

Felül a három vízszintes vonalra (Hamburger ikon) koppintva a menüt hozhatjuk elő. Válasszuk a &#8220;Registry&#8221; lehetőséget, majd a &#8220;Registry Browser&#8221; menüpontot. Ha mindent jól csináltunk akkor most megjelenik előttünk a telefonunk Registry-jének gyökérkönyvtára.&nbsp;Itt a következő utat kell végigjárnunk: **HKEY\_LOCAL\_MACHINE (HKLM)&nbsp;**–> **SYSTEM&nbsp;**–> **Platform&nbsp;**–> **DeviceTargetingInfo**.

<img loading="lazy" class="aligncenter wp-image-1501" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-1024x1024.jpg" alt="" width="600" height="600" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-1024x1024.jpg 1024w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-150x150.jpg 150w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-300x300.jpg 300w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-768x768.jpg 768w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-32x32.jpg 32w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-50x50.jpg 50w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-64x64.jpg 64w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-96x96.jpg 96w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7-128x128.jpg 128w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry7.jpg 2046w" sizes="(max-width: 600px) 100vw, 600px" /> 

Itt négy értéket kell átírnunk. Fontos, hogy mindenki a saját készülékének megfelelő értékeket válassza, azaz akinek egy SIM-es készüléke van az a Lumia 950XL adatait (&#8220;Egy SIM-es készülékek esetén&#8221;), míg a két SIM-es készülékek tulajdonosai a Lumia 950XL Dual SIM adatait (&#8220;Dual SIM-es készülékek esetén&#8221;)&nbsp;használják.

<img loading="lazy" class="aligncenter wp-image-1497" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry8-576x1024.jpg" alt="" width="300" height="533" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry8-576x1024.jpg 576w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry8-169x300.jpg 169w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry8-768x1365.jpg 768w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry8.jpg 1440w" sizes="(max-width: 300px) 100vw, 300px" /> 

A módosítás előtt érdemes az eredeti értékeket lementeni (képernyőmentés, stb.), hogy ha valami problémába futunk, akkor alaphelyzetbe állítás nélkül vissza tudjuk írni az eredeit értékeket. Természetesen egy alaphelyzetbe állítás, vagy WDRT (Windows Device Recovery Tool) az általunk elvégeztt módosításokat felülírja, és újra el kell végeznünk. Ezeket kell átírnunk a Registry-ben (az adott pontra koppintunk, átírjuk az értéket, majd allul a pipával véglegesíthetjük a módosításokat, a szükséges értékek idézőjelben félkövérrel vannak szedve, a beviteli mezőbe (Registry Value Data) idézőjelek nélkül kell beírni, a bejegyzés típusát (Registry Value Type) a legördülő menüben ne változtassuk meg):

<img loading="lazy" class="aligncenter wp-image-1510" src="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry11-576x1024.jpg" alt="" width="300" height="533" srcset="https://winsider.hu/wp-content/uploads/2017/08/inkedregistry11-576x1024.jpg 576w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry11-169x300.jpg 169w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry11-768x1365.jpg 768w, https://winsider.hu/wp-content/uploads/2017/08/inkedregistry11.jpg 1440w" sizes="(max-width: 300px) 100vw, 300px" /> 

&nbsp;

&#8220;PhoneManufacturer&#8221; = &#8220;**MicrosoftMDG**&#8221;

&#8220;PhoneManufacturerModelName&#8221; = &#8220;**RM-1085_11302**&#8221; (Egy SIM-es készülékek esetén)**; &#8220;****RM-1116_11258**&#8221; (Dual SIM-es készülékek esetén)

&#8220;PhoneModelName&#8221; = &#8220;**Lumia 950 XL**&#8221; (Egy SIM-es készülékek esetén); &#8220;**Lumia 950 XL Dual SIM**&#8221; (Dual SIM-es készülékek esetén)

&#8220;PhoneHardwareVariant&#8221; = &#8220;**RM-1085**&#8221; (Egy SIM-es készülékek esetén), &#8220;**RM-1116**&#8221; (Dual SIM-es készülékek esetén)

Ha mindezeket elvégeztük akkor a Gépház -> Rendszer -> Névjegy oldalon az alábbiakat fogjuk látni (a képernyőkép egy Lumia 930-on készült) és bátran kereshetünk frissítéseket a Windows Update-en keresztül. 🙂

<img loading="lazy" class="aligncenter wp-image-1508" src="https://winsider.hu/wp-content/uploads/2017/08/registry12-576x1024.jpg" alt="" width="300" height="533" srcset="https://winsider.hu/wp-content/uploads/2017/08/registry12-576x1024.jpg 576w, https://winsider.hu/wp-content/uploads/2017/08/registry12-169x300.jpg 169w, https://winsider.hu/wp-content/uploads/2017/08/registry12.jpg 720w" sizes="(max-width: 300px) 100vw, 300px" /> 

Sok sikert mindenkinek!

 [1]: https://www.microsoft.com/hu-hu/store/p/interop-tools-preview/9ntgwlc0d3cs?wa=wsignin1.0&rtc=1
 [2]: https://1drv.ms/f/s!Auqwa8v1qfFSgblVIYx8ojlmekUxiA