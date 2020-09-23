---
title: Megjelent PC-re a 15048, Mobilra a 15047-es Insider build!
author: Decsi Balázs
type: post
date: 2017-03-05T19:19:39+00:00
excerpt: Péntek este egy újabb frissítéssel lepték meg Redmond-ból az Insider-eket, mind PC-n és mobilon, rengeteg hibát javítva.
url: /2017/03/05/insider-build-pc-15048-mobil-15047/
featured_image: /wp-content/uploads/2017/03/insider.png
instant_articles_submission_id:
  - 1786107708374231
categories:
  - Insider
  - Windows 10
  - Windows 10 Mobile
tags:
  - Build 15047
  - Build 15048
  - Insider Fast
  - Windows 10
  - windows 10 mobile

---
Péntek este egy újabb frissítéssel lepték meg Redmond-ból az Insider-eket, mind PC-n és mobilon. Újdonságokat nem tartalmaznak, viszont annál több hibajavítást kaptunk! Lássuk mit tartalmaznak!

<!--more-->

## Hibajavítások, változások PC-re:

  * Javítva lett a hiba, ami miatt a UWP alkalmazások esetében a csomag nevük jelent meg a címsorban. (Nálam nem javította az új build ezt a hibát.)
  * Javítva lett a hiba ami miatt egyes játékok a tálcára minimalizálva indultak el.
  * Javítva lett a hiba, ami miatt MS Edge-be/ből másolt szóközt tartalmazó URL-k esetén a szóközöket nem cserélte le %20-ra.
  * Javítva lett a hiba ami miatt nem jelent meg a LastPass kiegészítő autómata kitöltés ikonja.
  * Javítva lett a hiba, ami miatt váratlan karakterek illesztődtek be egyes weboldalak esetében MS Edge-ben.
  * Javítva lett a hiba, ami miatt nem lehetett görgetni MS Edge-ben, ha nem volt maximalizálva az ablaka, vagy egy másik monitorra lett áttéve.
  * Finomhangolták az oldalon való keresést MS Edge-ben, így az ablak közepén jelenik meg a keresett elem.
  * Javítva lett laptopok esetében a hiba, ami miatt a fedél lehajtása után nem működik a fényerő szabályozás.
  * Javítva lett a hiba ami miatt nem lehetett bizonyos UWP alkalmazásokban a kereső mezőbe írni.
  * Javítva lett a hiba ami miatt MS Pinyin IME-t használva nem nyílnak meg Cortana keresési eredmények.
  * Javítva lett a hiba ami miatt egyazon telefon értesítései két különböző csoportban jelentek meg a Műveletközpontban.
  * Javítva lett a hiba ami miatt Outlook 2016 üzenet értesítésre kattintva az üzenet nem az előtérben nyílt meg.

## Hibajavítások, változások Mobilra:

  * Ismét megfelelően működik a fizetés és az új kártyák felvétele a Microsoft Wallet app-ban.
  * Ismét az elvártaknak megfelelően működnek MS Edge-ben a videóvezérlő gombok.
  * Javítva lett a hiba, ami miatt az Adathasználat menüpontban a Mobil adatforgalom nem jelent meg.
  * Cortana háttere ismét fekete színű, a korábbi szürke helyett.
  * Javítva lett a hiba, ami miatt egy idő után nem ajánlotta fel a szavak törtlését a személyes szótárból a szövegjavaslatok sáv.
  * Javítva lett a hiba, ami miatt az alkalmazásváltó lassabban nyílt meg a kívántnál.
  * Javítva lett a hiba, ami bizonyos eszközökön vibrálást okozott a Maps alkalmazásban.
  * Javítva lett a hiba, ami miatt a videó idősávon való elmozdulás után visszatért a videó kezdetéhez.
  * Javítva lett a hiba, ami miatt a 2. sim kártyáról nem jelentek meg az értesítések a művelet központban.

## Ismert hibák PC esetében:

  * Aki a korábbi build-ben a hibás registry kulcs miatt a részmegoldást alkalmazta, [EZ][1] alapján újra engedélyezheti az IPV6-ot.
  * Egyes számítógépek képtelenek frissíteni, és 71%-nál visszaállnak az előző build-re. További információ [ITT][2].
  * Symantec/Norton antivírust használók 0x80070228 hibát kaphatnak a build letöltése közben. További információ [ITT][3].
  * Ha további nyelvi csomag is telepítve van a számító gépre, akkor ez a build nem fog települni. Megoldás [ERRE][4] található.
  * Egyes hardver konfigurációk esetén zölden villoghat a Game Bar-on belül a “Live review” ablak közvetítés közben, ám ez csak a közvetítőnél látszik.
  * Hibák léphetnek fel MS Edge-ben ha F12-es eszközt használva böngésszük a honlapokat.
  * Ha meg van nyitva az F12-es fejlesztői eszközök MS Edge-ben majd újra megnyomom az F12, akkor a lap, amihez meg volt nyitva nem kerül az előtérbe, valamint ha nem volt megnyitva, és megnyitom, akkor az sem kerül előtérbe.
  * F12-es eszközt megnyitva az F12 ablaka az aktív MS Edge ablak mögött nyílhat meg.
  * Azok, akik több monitort használnak néha az egyik monitor befagyhat. Ezt újraindítással, vagy a Gépház -> Rendszer -> Kijelző lapon a megjelenítés módját átállítva, majd kiterjesztettre visszaállítva javítható. (Mejg “Windows” + “P” gomb használata egyszerűbb, bár nem tudom működik-e)

## Ismert hibák Mobil esetében:

  * Beszéd csomagokat esetleg nem lehet letölteni ezen a build-en.

Hivatalos blogpost: [blogs.windows.com][5]

 [1]: https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install/build-15042-for-pc-install-hangs-workaround/9c2484c5-9ede-4495-a155-adf5469b4963?tm=1487959098001
 [2]: https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install/install-of-15042-reboots-at-71-to-15031/a640c8f4-b93c-46fb-9aee-4d302f00eadf
 [3]: https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install/pc-build-15046-install-fails-due-to-anti-virus/061cab5a-8e69-45fd-ba16-5da525a1ae1b?tm=1488498251633
 [4]: https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install/pc-build-15046-error-80070228-during-download/71faa97f-6914-4755-8063-c372efa1634a?tm=1488330779488
 [5]: https://blogs.windows.com/windowsexperience/2017/03/03/announcing-windows-10-insider-preview-build-15048-for-pc-and-build-15047-mobile/#2Jsd454vH2EdpPDW.97