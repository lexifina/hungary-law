3. melléklet a 34/2016. (XI. 30.) EMMI rendelethez

## Nem tanúsított iratkezelési szoftverből történő, nem iktatási típusú nyilvántartásból történő, iratszintű metaadatok átvételére vonatkozó követelmények

1. A metadata.xml fájl tartalmára vonatkozó speciális előírások.

1.1. A metadata.xml a nem tanúsított iratkezelési szoftverből történő, nem iktatási típusú nyilvántartásból történő, iratszintű metaadatok átvételénél az átvétel általános metaadatai mellett, a besorolási sémához, a besorolási séma egyes kategóriáihoz, az irategyüttesekhez és a nyilvántartott iratokhoz tartalmaz leíró, adminisztratív, fájlleíró és strukturális metaadatokat.

1.2. Az átadásra kerülő iratanyag metaadatai struktúrájának egyik rétegét az adott nyilvántartás besorolási sémájának megfelelő kategória-hierarchia adja, a másik alapszintű rétegét pedig az egyedi nyilvántartott iratokból képzett irategyüttes az 1. melléklet 2.8.1. alpontjában meghatározott aggregáció-hierarchia.

1.3. A struktúra felépítésénél a besorolási sémából az alkategóriákat már nem tartalmazó legalsó elemeket lehet hozzárendelni a nyilvántartott iratokhoz és irategyüttesekhez.

1.4. A nyilvántartott iratokat közvetlenül tartalmazó irategyüttesekhez már nem rendelhető alsóbb szintű irategyüttes. Csak az irathierarchia legalsó szintű irategyütteseihez lehet nyilvántartott iratokat rendelni.

2. A leíró metaadatokra vonatkozó követelmények

2.1. A leíró metaadatokra vonatkozó követelményrendszer értelmezése:

a) A oszlop: A metaadatok szövegszerű megnevezése.

b) B oszlop: A metaadat szerepeltetésére vonatkozó megkötés. Az A oszlop szerinti metaadat megadása kötelező, ha a forrásrendszerben a metaadatra vonatkozó érték szerepel.

c) C oszlop: Az A oszlop szerinti metaadat ismételhetőségére vonatkozó előírás.

d) D oszlop: Az A oszlopban rögzített metaadat használatát segítő, magyarázó leírás.

2.2. A hierarchiában a besorolási séma leírásához használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos a besorolási séma egyedi azonosítójával. |

| 3 | Metaadat-leírás megnevezés | igen | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos a besorolási séma megnevezésével. |

| 4 | Azonosító | igen | nem | A besorolási séma egyedi azonosítója. Alapértelmezetten: „BSévszám”. |

| 5 | Besorolási séma megnevezése | igen | nem | A besorolási séma szöveges megnevezése. |

| 6 | Irathierarchia szintje | igen | nem | A besorolási sémának a besorolási hierarchiában betöltött helye. Konstans érték: „Besorolási séma”, amelynek reprezentációja „CLASSIFCATION”. |

| 7 | Tartalmi összefoglalás | nem | nem | A besorolási séma tartalmára vonatkozó rövid összefoglaló leírás. |

| 8 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 9 | Készítési idő | igen | nem | A besorolási terv készítésének dátuma. |

2.3. A nyilvántartási hierarchiában a besorolási séma kategóriáinak leírásához használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos a besorolási séma kategória egyedi azonosítójával |

| 3 | Metaadat-leírás megnevezés | igen | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos a besorolási séma kategória megnevezésével |

| 4 | Irathierarchia szintje | igen | nem | A besorolási séma kategóriának a besorolási hierarchiában betöltött helye. Konstans érték: „kategória”, amelynek reprezentációja „CLASS”. |

| 5 | Kategória azonosító | igen | nem | A kategória egyedi azonosítója. |

| 6 | Kategória megnevezése | igen | nem | Szöveg típusú mező. |

| 7 | Készítési idő | igen | nem | A kategória keletkezési dátuma. |

| 8 | Tartalmi összefoglalás | nem | nem | A kategória tartalmára vonatkozó rövid összefoglaló leírás. |

| 9 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 10 | Alapértelmezett megőrzési mód | igen | nem | A megőrzési idő lejárta utáni alapértelmezetten elvégzendő teendő leírása. Lehetséges értékei: „Határidő nélkül megőrzendő”, „Lejárati idő végén felülvizsgálandó”, „Levéltárba adandó”, „Selejtezendő”. |

| 11 | Alapértelmezett megőrzési idő egység | igen | nem | A besorolási séma kategóriához tartozó alapszintű megőrzési idő jellege. Lehetséges értékei: „Napok”, „Hetek”, „Hónapok”, „Évek”. |

| 12 | Alapértelmezett megőrzési idő érték | igen | nem | A besorolási séma kategóriához tartozó alapszintű megőrzési idő értéke. |

2.4. Az irathierarchiában az egyes irategyüttesek leírásához használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az irategyüttes azonosítójával. |

| 3 | Metaadat-leírás megnevezés | igen | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos az irategyüttes megnevezésével. |

| 4 | Irategyüttes azonosító | igen | nem | Az irategyüttes egyedi azonosítója. |

| 5 | Irategyüttes megnevezése | igen | nem | Az irategyüttes szöveges megnevezése. |

| 6 | Irathierarchia szintje | igen | nem | Az irategyüttesnek az irathierarchiában betöltött helye, a leírási szintje. Konstans érték: „Irategyüttes”, amelynek reprezentációja „RECORDGRP”. |

| 7 | Készítési idő | igen | nem | Az irategyüttes létrehozásának időpontja. |

| 8 | Lezárási idő | igen | nem | Az irategyüttes lezárásának időpontja. |

| 9 | Besorolási séma azonosító | nem | nem | Annak a besorolási kategóriának az azonosítója, ahova az irategyüttes be van sorolva. |

| 10 | Besorolás dátuma | nem | nem | A besorolási sémába való besorolás dátuma. |

| 11 | Tárgyszavak | nem | igen | Tárgyszókészletből kiválasztott releváns tárgyszavak. |

| 12 | Az iratképző neve | nem | nem | Az elektronikus átvételi csomagban szereplő irategyüttest keletkeztető szervezet megnevezése. Szervezeti változás, más szervezettől való iratátvétel során a nyilvántartásba felvett irat esetén az eredeti iratképzőt kell feltüntetni. |

| 13 | Idő(kör) kezdete | igen | nem | Az irategyüttes létrehozásának kezdete. Értéke megegyezik a 7. sor Készítési idő metaadat kezdő időpontjával. |

| 14 | Idő(kör) vége | igen | nem | Az irategyüttes létrehozásának vége. Értéke megegyezik a 8. sor Lezárási idő metaadat értékével. |

| 15 | Tartalmi összefoglalás | nem | nem | Az irategyüttes tartalmára vonatkozó rövid összefoglaló leírás. |

| 16 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 17 | Részletes tartalmi leírás | nem | nem | Az irategyüttes tartalmát, időbeni, térbeli vonatkozásait részletesen bemutató leírás. |

| 18 | Földrajzi tárgyszavak | nem | igen | Az irategyütteshez kapcsolódó jellemző földrajzi helyek, települések, címek. |

| 19 | Nyelv | nem | igen | Az irategyüttes tartalmában használt nyelvekre vonatkozó leírás. |

| 20 | A megőrzés története | nem | nem | Az irategyüttes történetére vonatkozó mindazon információk, amelyek az azonosítás, a hitelesség vagy az értelmezés szempontjából fontosak lehetnek. Ide értendők a leírási egységet érintő tulajdoni változások, a megőrzésért és kezelésért felelős személyi/szervezeti változások, valamint mindazok a beavatkozások, így a rendezés, a konverzió, stb., amelyek kihatottak az ügyirat végleges állapotára és rendezettségére. |

| 21 | A levéltárba kerülés közvetlen forrása | nem | nem | Amennyiben az irategyüttes nem az iratképzőtől kerül átadásra, ahol keletkezett, itt kell rögzíteni az átadóra vonatkozó információt. |

| 22 | A leírási egység szerkezete | nem | nem | Az irategyüttes belső elrendezésére, felépítésére vonatkozó információk. |

| 23 | Hozzáférési korlátozások | igen | nem | Az irategyüttes tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 24 | Felhasználási korlátozások | igen | nem | Az irategyüttes reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 25 | Eredeti példányok léte és őrzőhelye | nem | igen | Amennyiben az iratátadás során az eredeti irategyüttes nem kerül átadásra, csak másolat, akkor itt rögzíthető az eredeti pontos helyére vonatkozó leírás. |

| 26 | Másolatok léte és őrzőhelye | nem | igen | Az átadott irategyüttes létező másolatainak pontos helye. |

| 27 | Kapcsolódó leírási egységek | nem | igen | Az átadott irategyüttes tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 28 | Leírási szabályok | nem | nem | Az irategyüttesben vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.5. Az irathierarchiában a nyilvántartott iratok leírásához használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az irat egyedi azonosítójával. |

| 3 | Metaadat-leírás megnevezés | nem | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos a nyilvántartott irat címével. |

| 4 | Iratazonosító | igen | nem | A nyilvántartott irat azonosítója. |

| 5 | Tárgy | igen | nem | A nyilvántartott irat szöveges megnevezése, tárgya. |

| 6 | Irathierarchia szintje | igen | nem | A nyilvántartott iratnak az irathierarchiában betöltött helye, a leírási szintje. Konstans érték: „nyilvántartott irat”, amelynek reprezentációja „RECORD”. |

| 7 | Készítési idő | igen | nem | A nyilvántartott irat keletkezési ideje. |

| 8 | Tárgyszavak | nem | igen | Tárgyszókészlet. |

| 9 | Besorolási séma rekord azonosító | igen | nem | Annak a besorolási kategóriának az azonosítója, ahova az irat be van sorolva. |

| 10 | Besorolás dátuma | igen | nem | A besorolási sémába való besorolás pontos időpontja. |

| 11 | Megőrzési mód | nem | nem | A megőrzési idő lejárta utáni tényleges teendő leírása, amely felülírhatja a besorolási sémában meghatározott megőrzési mód értékét. Lehetséges értékei: „Határidő nélkül megőrzendő”, „Lejárati idő végén felülvizsgálandó”, „Levéltárba adandó”, „Selejtezendő”. |

| 12 | Tényleges megőrzési idő egység | nem | nem | Az ügyirathoz tartozó tényleges megőrzési idő jellege, amely felülírhatja a besorolási sémában meghatározott megőrzési idő egység értékét: „Napok”, „Hetek”, „Hónapok”, „Évek”. |

| 13 | Tényleges megőrzési idő | nem | nem | Az irathoz tartozó megőrzési idő, amely felülírhatja a besorolási sémában meghatározott megőrzési idő értékét. |

| 14 | Ügyazonosító | nem | nem | Ügyazonosító, amennyiben az információ ügykezelő rendszerből érkezik. |

| 15 | Ügykezelő rendszer azonosítója | nem | nem | Az ügykezelő rendszer azonosítója, amennyiben az információ ügykezelő rendszerből érkezik. |

| 16 | Irat státusza | nem | nem | Az iratnak az iratkezelési folyamatban való helyzetét leíró adat. Alapértékei: iktatva, szignálva, törölve, határidőben, elintézett, átmeneti irattárban, központi irattárban, selejtezve, levéltárban. |

| 17 | Mellékletek száma | nem | nem | Az irathoz tartozó mellékletek száma. |

| 18 | Kapcsolódó iratok | nem | igen | A kapcsolódó irat(ok) egyedi azonosítója, amely alapján megállapítható(k) egy adott ügyirattal szerelési kapcsolatban nem lévő, de tárgya szerint kapcsolódó további ügyirat(ok). |

| 19 | Levéltárba adás dátuma | nem | nem |  |

| 20 | Irat helye | nem | nem | Az irat fizikai helye. |

| 21 | Az iratképző neve | nem | nem | A nyilvántartott iratot keletkeztető szervezet megnevezése. Szervezeti változás, más szervezettől való iratátvétel során a nyilvántartásba felvett irat esetén az eredeti iratképzőt kell feltüntetni. |

| 22 | Idő(kör) kezdete | igen | nem | A nyilvántartott irat létrehozásának kezdete. |

| 23 | Idő(kör) vége | igen | nem | A nyilvántartott irat létrehozásának vége. |

| 24 | Tartalmi összefoglalás | nem | nem | A nyilvántartott irat tartalmára vonatkozó rövid összefoglaló leírás. |

| 25 | Megjegyzés | nem | nem |  |

| 26 | Földrajzi tárgyszavak | nem | igen | Az irathoz kapcsolódó jellemző földrajzi helyek, települések, címek. |

| 27 | Nyelv | nem | igen | Az irat tartalmában használt nyelvekre vonatkozó leírás. |

| 28 | A megőrzés története | nem | nem | Az irategyüttes történetére vonatkozó mindazon információk, amelyek az azonosítás, a hitelesség vagy az értelmezés szempontjából fontosak lehetnek. Ide értendők a leírási egységet érintő tulajdoni változások, a megőrzésért és kezelésért felelős személyi/szervezeti változások, valamint mindazok a beavatkozások, így a rendezés, a konverzió, stb., amelyek kihatottak az ügyirat végleges állapotára és rendezettségére. |

| 29 | A levéltárba kerülés közvetlen forrása | nem | nem | Ha a nyilvántartott irat nem az iratképzőtől – ahol keletkezett – kerül átadásra, itt kell rögzíteni az átadóra vonatkozó információt. |

| 30 | A leírási egység szerkezete | nem | nem | A nyilvántarott irat belső elrendezésére, felépítésére vonatkozó információk. |

| 31 | Hozzáférési korlátozások | igen | nem | A nyilvántartott irat tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 32 | Felhasználási korlátozások | igen | nem | A nyilvántartott irat reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 33 | Eredeti példányok léte és őrzőhelye | nem | igen | Amennyiben az iratátadás során az eredeti nyilvántartott irat nem kerül átadásra, csak másolat, akkor itt rögzíthető az eredeti pontos helyére vonatkozó leírás. |

| 34 | Másolatok léte és őrzőhelye | nem | igen | Az átadott nyilvántartott irat létező másolatainak pontos helye. |

| 35 | Kapcsolódó leírási egységek | nem | igen | Az átadott nyilvántartott irat tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 36 | Leírási szabályok | nem | nem | Az iratban vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.6. Az iratképző a nem iktatás típusú, specifikus iratnyilvántartásaiban egyéb, az adott feladatra vonatkozó metaadatokat is tárolhat a 2.1-2.5 pontokban megjelölteken túl. Az iratátadás során ezeket a metaadatokat is át kell adni a levéltárnak. A 2.1-2.5 pontokban meghatározott metaadatot a leíró metaadatok specifikációjának megfelelően, minden más adatot, személyekre, szervezetekre, belső hivatkozásokra, címekre vonatkozó, és további szöveges, numerikus és dátum formátumú leíró metaadatokat a kiegészítő leíró metaadatokra vonatkozó specifikációnak megfelelően kell átadni.

3. Az 1. melléklet 2.8.2. pontja szerinti strukturális divízió elemet kell készíteni valamennyi besorolási séma, kategória, irategyüttes és nyilvántartott irat számára.
