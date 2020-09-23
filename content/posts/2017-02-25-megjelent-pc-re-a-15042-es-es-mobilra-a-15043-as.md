---
title: Megjelent PC-re a 15042-es és mobilra a 15043-as build! (Insider Fast)
author: Decsi Balázs
type: post
date: 2017-02-25T10:42:15+00:00
url: /2017/02/25/megjelent-pc-re-a-15042-es-es-mobilra-a-15043-as/
tumblr_winsider_permalink:
  - https://winsider.tumblr.com/post/157688460736/megjelent-pc-re-a-15042-es-és-mobilra-a-15043-as
tumblr_winsider_id:
  - 157688460736
instant_articles_submission_id:
  - 257268508057644
categories:
  - Insider
tags:
  - Insider Fast
  - Windows 10
  - windows 10 mobile

---
Tegnap este a Microsoft kiadta a két rendszer verziót. Mivel korábban feature complete-nek (funkció teljesnek, azaz új funkciók már nem kerülnek be a rendszerbe) nyilvánította a cég az alkotói frissítést, ezért már csak hibajavítások érkeztek a rendszerhez. Viszont abból egy eléggé hosszú listát kaptunk. Lássuk mik a főbb hibajavítások és finomhangolások.

## **Frissítés**

A build PC-re úgy jött ki, hogy 32-bit-es rendszereken nem lehet frissíteni, ám időközben megoldották a hibát, így a 32-bit-es Windows 10-el rendelkező felhasználók is képesek az új build-et telepíteni!

<!--more-->

<!-- more -->

## Újdonságok (PC)

  * **Új Cortana animáció az első indításkori beállítások során**
  * **Flash beépülő aktiválására felhívás:** A 15002-es build-ben lett bevezetve, hogy az Adobe Flash beépülőkre épülő felületek alapméretezetten csak kattintásra induljanak el. A link sávba egy új üzenetet helyeztünk el, ami tisztába teszi, hogy a Flash tartalmak blokkolva lettek.
  * **Fejlesztett olvasási élmény Microsoft Edge-ben:** Rengeteg visszajelzés érkezett, amiből egyeseket megvalósítottak. Ilyen például a könyv ikon a lapfüleken, illetve egyes hangoskönyv lehetőségeken is fejlesztettek

## Egyéb fejlesztések és hibajavítások (PC)

  * Javítva lett a Bluetooth-al kapcsolatos hiba, valamint ismét használható a Gépház -> Eszközök lap
  * Javítva lett a Műveletközpont hibája, ami miatt üresen jelent meg
  * Javítva lett egy egész sereg Microsoft Edge-el kapcsolatos hiba. A teljesség igénye nélkül: legördülő listák, jelszavak, előképek, honlapra való navigálás, beillesztés ismét az elvárásoknak megfelelően működnek.
  * Javítva lett a hiba, ami egyes készülékek esetében kék halált okozott, ha hibernálásból fel lett ébresztve a rendszer
  * Javítva lett néhány Windows Ink-el kapcsolatos hiba.
  * Javítva lett az új görgetősáv animációjának beragadása.
  * Javítva lett a hiba, ami az exploler.exe összeomlását okozta, ISO file-on történő dupla klikk miatt.
  * Javítva lett a hiba, ami miatt nem kapcsolt be/ki a kék fény szűrő, ha az előre beállított időpont alatt alvóállapotba volt a számítógép.

## Egyéb fejlesztések és hibajavítások (Mobil)

  * Javítva lett a Bluetooth-al kapcsolatos hiba, valamint ismét használható a Gépház -> Eszközök lap
  * Ismét használható a Continuum vezeték nélküli kijelzővel
  * Javítva lett a hiba, ami a képernyő elforgatást megakadályozta
  * Javítva lett a hiba, ami az élő csempék frissítését megakadályozta
  * Az eszközre történő másolás ismét elvárásoknak megfelelően működik
  * Javítva lett a hiba, ami egy társított alkalmazás megnyitása miatt a Microsoft Edge összeomlását okozta és az app pedig nem nyílt meg
  * Javítva lett a hiba, ami a személyes szótárt törtlődését okozta.
  * Javítva lett a frissítés letöltésének hibája, amikor letöltés közben kikapcsolták a Wifi-t, majd ismét kapcsolódva nem folytatta a letöltést.

## Ismert hibák (PC)

  * Egyes gépek nem képesek frissíteni egy hibás registry kulcs miatt. A megoldást [ITT][1] találjátok hozzá.
  * Bár javítva lett a fő oka a Spectrum.exe folyamatos összeomlásának, egyes Insiderek esetében továbbra is fennállhat ez a hiba. Ennek az állapotnak a befejezésére átmeneti megoldás:  Spectrum.exe leállítása, törölni a C:ProgramDataMicrosoftSpectrumPersistedSpatialAnchors mappát és újraindítani a számítógépet.
  * Egyes népszerű játékok minimalizálva indulnak el, a tálcán rákattintva visszahozható.
  * Egyes hardver konfigurációk esetén zölden villoghat a Game Bar-on belül a “Live review” ablak közvetítés közben, ám ez csak a közvetítőnél látszik.
  * Microsoft Edge esetében az F12-es eszközök nem megfelelően működnek.
  * Windows Insider Program ikonja nem jelenik meg.
  * Windows Hello arcfelismerés egyes esetekben nem működik a zárképernyőn, “A kamera nem indítható” hibaüzenettel.
  * +1: Egyes esetekben Microsoft Edge és/vagy a tálca nem reagál. Ebben az esetben a Feladatkezelőben(Ctrl + Shift + Esc)be kell zárni a Microsoft Edge-et és az exploler.exe-t újra kell indítani.

## Ismert hibák (Mobil)

  * Beszéd csomagokat nem lehet letölteni ezen a build-en.
  * A Pénztárca alkalmazásban nem lehet új kártyát felvenni, és nem lehet fizetni meglévő kártyákkal.

Hivatalos blogpost: [blogs.microsoft.com][2]

 [1]: https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install/build-15042-for-pc-install-hangs-workaround/9c2484c5-9ede-4495-a155-adf5469b4963?tm=1487959098001
 [2]: https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/#kQ5AEZr3uIb6ZM6j.97