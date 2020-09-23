---
title: Miért ilyen régi a legtöbb Windows driver?
author: Balogh János
type: post
date: 2017-03-01T20:54:41+00:00
excerpt: Szemfüles Windows felhasználók észrevehették már, hogy a Microsoft driver-ek régi, 2006-os dátummal rendelkeznek. Cikkünkben elmondjuk, mi ennek az oka.
url: /2017/03/01/miert-regiek-a-windows-driverek/
featured_image: /wp-content/uploads/2017/03/driver-cover.png
instant_articles_submission_id:
  - 1607291615966871
categories:
  - Windows 10
tags:
  - driver
  - windows

---
Szemfüles Windows felhasználók biztosan észrevették már, hogy a Microsoft driverei igencsak régi dátummal rendelkeznek. Egészen pontosan 2006.06.21. a dátumozás rajtuk.

<img loading="lazy" class="aligncenter wp-image-211 size-medium" src="https://winsider.hu/wp-content/uploads/2017/02/driver-262x300.png" alt="Képernyőfotó egy Microsoft-os driverről, amin látszódik az ominózus, 2006-os dátum" width="262" height="300" srcset="https://winsider.hu/wp-content/uploads/2017/02/driver-262x300.png 262w, https://winsider.hu/wp-content/uploads/2017/02/driver.png 398w" sizes="(max-width: 262px) 100vw, 262px" /> 

Bár a verziószám időről időre növekszik, de a dátum változatlan. Még akkor is, ha azok olyan funkciókat valósítanak meg, amik **garantáltan** nem léteztek még abban az évben. Talán a Microsoft mérnökei majd egy évtizeddel előre fejlesztenek? Nem! Ennek oka egészen más.

Zac Lockard, a Microsoft egyik fejlesztője válaszolta meg a kérdést.  
Amikor a Windows egy eszközhöz keresi a megfelelő driver-t, a lehetséges eszközmeghajtókat bizonyos kritériumok alapján rangsorolja.  
Amennyiben egy driver tökéletesen megfelel az eszköz Hardware ID-je alapján (tehát pontosan ehhez az eszközhöz készült), akkor az lesz a legnagyobb prioritású driver az eszközhöz.  
Ha több ilyen tökéletes egyezésű driver is szóba jöhet, akkor ezek közül a legfrisebb dátumozásút választja a Windows. Ha még mindig több driver jöhet szóba, akkor a legnagyobb fájlverziójú drivert fogja választani a rendszer. Mégis mire jó ez az egész válogatás?

<!--more-->

Képzeljük el, mi lenne akkor, ha a Windows driver-ek dátumozása megfelelne a valóságnak, azaz minden új Windows build egyre újabb dátumú eszközmeghajtókkal jönne. Vegyük például azt az esetet, hogy a Windows 10 RTM kiadásáról átállunk a Redstone kiadásra.  
Eközben egyes hardware elemeinkhez feltelepítettük a gyártó által adott driver-t, de az nem adott ki új verziót a Redstonehoz. (Miért is tenné?)  
Ekkor a keresési kritériumoknak megfelelően a Windows a saját driverét részesítené előnyben, hiszen az új build frissebb dátumú. Így tehát a Windows saját driver-e felülírná a korábban feltelepített, gyártó által adott meghajtóprogramot.  
Ugyanakkor, amennyiben a jelenlegi driver is egy Microsoft által kiadott verzió, akkor az újabbat fogja használni a rendszer, mivel ekkor a dátum egyezés miatt a nagyobb verziószámút, tehát az újabbat fogja telepíteni a Windows.

## Oké, de miért éppen 2006?

A 2006-os dátumozással a Microsoft elérte, hogy a jelenlegi Windows verziók is előnyben részesítik az eszközgyártók által kiadott drivereket amennyiben azok a Vista, vagy az azt követő verziókhoz készültek. Láthatunk néhány 2009-es Microsoft drivert is, ennek az oka pedig az, hogy csak a Windows 7, vagy újabb verziókhoz készült drivereket fogadja el a sajátjai helyett a Windows. Emögött néhány, a 7-es Windowsban bevezetett változtatás áll.  
Remélhetőleg ezzel sikerült megnyugtatóan megválaszolni egy érdekes kérdést. Idézve Zac-et:

> Ez egy fantasztikus példája annak, hogy néha az őrültségnek és jelentéktelennek tűnő dolgok milyen hasznosak, és okkal léteznek.

Forrás: <a href="https://blogs.msdn.microsoft.com/oldnewthing/20170208-00/?p=95395" target="_blank">The Old New Things Blog</a>