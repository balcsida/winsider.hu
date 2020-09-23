---
title: Megjelent a 15031-es build PC-re Insider Fast ring-en!
author: Decsi Balázs
type: post
date: 2017-02-09T19:48:02+00:00
url: /2017/02/09/megjelent-a-15031-es-build-pc-re-insider-fast/
tumblr_winsider_permalink:
  - https://winsider.tumblr.com/post/157028812786/megjelent-a-15031-es-build-pc-re-insider-fast
tumblr_winsider_id:
  - 157028812786
instant_articles_submission_id:
  - 1742165179446836
categories:
  - Insider
  - Windows 10

---
Tegnap este megjelent PC-re a 15031-es build. Több újdonságot és több hibajavítást is tartalmaz, ám az ismert hibák száma sem igazán csökkent. Nézzük meg mit tartalmaz tehát ez a frissítés.

<!-- more -->

## Újdonságok:

  * **Kép a képben alkalmazások:** Egyes alkalmazások képesek lesznek arra, hogy kis méretű ablakokban, minden tartalom előtt fussanak tovább, így nem kell háttérbe tenni, és továbbra is használhatóak maradnak.
  * **Dinamikus zárolás:** A számítógép zárolása lehetséges, egy bluetooth-al párosított telefon közelsége alapján. Ha a telefon nem található meg a számítógép közelében (nincs csatlakoztatva) akkor kikapcsolja a Windows a kijelzőt és 30 másodperc múlva zárolja a számítógépet.
  * **Megosztás új ikont kapott.**
  * **Game Bar fejlesztett teljes kijelzős támogatása:** Jelen pillanatban 52 új játék támogatása került be.

## Egyéb újdonságok és javítások:

  * Tencent alkalmazások és játékok újra hiba nélkül futtathatók.
  * Ha nem észlelhető audió kimenet, akkor OOBE során Cortana bemutatkozása nem jelenik meg
  * Javítva lett egy hiba, ami miatt egyes népszerű játékok betöltés során összeomlanak.
  * Game Mode kapcsolója ezentúl az elvárásoknak megfelelően működik, illetve nincs bekapcsolva rendszer szinten alapméretezetten.
  * A kék fény szűrő gyorskapcsolója újra működik.
  * Javítva lett a némitási hiba, amikor SpeechRuntime.exe összeomlása után a start menü megnyitva lett.
  * Minden alkalmazás listából a csempés felületre ismét át lehet húzni alkalmazásokat.
  * A képmetsző az elvárt módon működik ismét.
  * “Fn”+”Pause/Break” billentyű kombináció újra működik.
  * Ablakok tollal való átméretezése normális sebességgel történik, illetve eltérő DPI-s beállítású monitorokon való átméretezés az elvárt módon működik ismét.
  * Microsft Edge-ben sötét témát használva Web Notes ikonja ismét látható
  * 3 ujjas touchpad gesztusok megbízhatóságán javítottak
  * Ismét átnevezhetőek a lemezek a Windows Intézőben
  * Megosztási felület az elvárásoknak megfelelően működik ismét, az ismételt megnyitások után is.
  * Cortana Background Task túlzott erőforrás felhasználását okozó hiba javítva lett

## Ismert hibák

  * Letöltés során 0%-on ragadhat a folyamatjelző sáv, nem kell foglalkozni vele, letöltődik és telepíthető a build.
  * Bár javítva lett a fő oka a Spectrum.exe folyamatos összeomlásának, egyes Insiderek esetében továbbra is fennállhat ez a hiba. Ennek az állapotnak a befejezésére átmeneti megoldás:  Spectrum.exe leállítása, törölni a C:ProgramDataMicrosoftSpectrumPersistedSpatialAnchors mappát és újraindítani a számítógépet.
  * Gépház -> Eszközök lap megnyitása a Gépház összeomlását okozza, bluetooth gyorskapcsolója sem működik.
  * A csatlakozási UX nem indítható a műveletközpontból, Win + K kombinációval és a Gépházból sem.
  * Egyes népszerű játékok minimalizálva indulnak el, a tálcán rákattintva visszahozható.
  * Egyes hardver konfigurációk esetén zölden villoghat a Game Bar-on belül a “Live review” ablak közvetítés közben, ám ez csak a közvetítőnél látszik.
  * Microsoft Edge esetében az F12-es eszközök nem megfelelően működnek.
  * Microsoft Edge egyes fejlesztői funkciója nem megfelelően indul el.
  * Windows Update lapra vállalati kezelésről értesítő szöveg kerülhet ki, még akkor is ha nem kezeli semmilyen szervezet a PC-t. Nem kell megijedni, ez egy hiba miatt írja ki, senki sem kezeli a számítógépet.
  * Egyes PC-ken az audio eszközök véletlenszerűen leállhatnak. Az audioeszköz újraindítása ideiglenesen megoldja ezt a hibát.
  * Egyes esetekben a Műveletközpont üresen jelenhet meg. A tálcát más helyzetbe mozgatva ideiglenesen javítható a hiba
  * Windows Insider Program ikonja nem jelenik meg.

Hivatalos blogpost: [blogs.windows.com][1]

 [1]: https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/