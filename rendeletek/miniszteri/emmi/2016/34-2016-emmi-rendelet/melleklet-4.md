4. melléklet a 34/2016. (XI. 30.) EMMI rendelethez

## Nem iratszintű metaadatok átvételére vonatkozó követelmények

1. A metadata.xml a nem iratszintű metaadatok átvételénél az átvétel általános metaadatai mellett, a besorolási sémához, a besorolási séma egyes kategóriáihoz, az irategyüttesekhez és a nyilvántartott iratokhoz tartalmaz leíró, adminisztratív, fájlleíró és strukturális metaadatokat.

2. A leíró metaadatokra vonatkozó követelmények

2.1. A leíró metaadatokra vonatkozó követelményrendszer értelmezése:

a) A oszlop: A metaadatok szövegszerű megnevezése.

b) B oszlop: A metaadat szerepeltetésére vonatkozó megkötés. Az A oszlop szerinti metaadat megadása kötelező, ha a forrásrendszerben a metaadatra vonatkozó érték szerepel.

c) C oszlop: Az A oszlop szerinti metaadat ismételhetőségére vonatkozó előírás.

d) D oszlop: Az A oszlopban rögzített metaadat használatát segítő, magyarázó leírás.

2.2. Az irategyüttes leírásához használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az irategyüttes azonosítójával. |

| 3 | Metaadat-leírás megnevezés | igen | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos az irategyüttes megnevezésével. |

| 4 | Idő(kör) kezdete | igen | nem | Az iratanyag létrehozásának kezdete. |

| 5 | Idő(kör) vége | igen | nem | Az iratanyag létrehozásának befejezése. |

| 6 | Leírás szintje | igen | nem | Az elektronikus átvételi csomagba foglalt irategyüttes legmagasabb hierarchia szintjének megfelelő azonosító. Lehetséges értékei: „tétel”, amelynek reprezentációja „CLASS”; „gyűjtemény”, amelynek reprezentációja „COLLECTION”; „ügyirat”, amelynek reprezentációja „FILE”; „fond”, amelynek reprezentációja „FONDS”; „egyes irat”, amelynek reprezentációja „ITEM”; „egyéb leírási szint”, amelynek reprezentációja „OTHERLEVEL”; „irategyüttes”, amelynek reprezentációja „RECORDGRP” , illetve „SUBGRP”; „sorozat”, amelynek reprezentációja „SERIES”; „állag”, amelynek reprezentációja „SUBFONDS”; „alsorozat”, amelynek reprezentációja „SUBSERIES”. |

| 7 | Tartalmi összefoglalás | nem | nem | Az elektronikus átvételi csomagba foglalt irategyüttes tartalmára vonatkozó rövid összefoglaló leírás. |

| 8 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 9 | Az iratképző neve | nem | nem | Az elektronikus átvételi csomagban szereplő irategyüttest keletkeztető szervezet megnevezése. Szervezeti változás, más szervezettől való iratátvétel során a nyilvántartásba felvett irat esetén az eredeti iratképzőt kell feltüntetni. |

| 10 | A megőrzés története | nem | nem | Az irategyüttes történetére vonatkozó mindazon információk, amelyek az azonosítás, a hitelesség vagy az értelmezés szempontjából fontosak lehetnek. Ide értendők a leírási egységet érintő tulajdoni változások, a megőrzésért és kezelésért felelős személyi/szervezeti változások, valamint mindazok a beavatkozások, így a rendezés, a konverzió, stb., amelyek kihatottak az ügyirat végleges állapotára és rendezettségére. |

| 11 | A levéltárba kerülés közvetlen forrása | nem | nem | Amennyiben az iratanyag nem az iratképzőtől kerül átadásra, ahol keletkezett, itt kell rögzíteni az átadóra vonatkozó információt. |

| 12 | Részletes tartalmi leírás | nem | nem | Az iratanyag tartalmát, időbeni, térbeli vonatkozásiait részletesen bemutató leírás. |

| 13 | Hozzáférési korlátozások | igen | nem | Az iratanyag tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 14 | Felhasználási korlátozások | igen | nem | Az iratanyag reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 15 | Nyelv | nem | nem | Az iratanyag tartalmában használt nyelvekre vonatkozó leírás. |

| 16 | Eredeti példányok léte és őrzőhelye | nem | nem | Amennyiben az iratátadás során az eredeti iratanyag nem kerül átadásra, csak másolat, akkor itt rögzíthető az eredeti pontos helyére vonatkozó leírás. |

| 17 | Másolatok léte és őrzőhelye | nem | nem | Az átadott iratanyag létező másolatainak pontos helye. |

| 18 | Kapcsolódó leírási egységek | nem | nem | Az átadott iratanyag tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 19 | Leírási szabályok | nem | nem | Az iktatókönyvben vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.3. Az iratképző a nem iktatás típusú, specifikus iratnyilvántartásaiban egyéb, az adott feladatra vonatkozó metaadatokat is tárolhat a 2.2 pontban megjelölteken túl. Az iratátadás során ezeket a metaadatokat is át kell adni a levéltárnak. A 2.2 pontban meghatározott metaadatot a leíró metaadatok specifikációjának megfelelően, minden más adatot, személyekre, szervezetekre, belső hivatkozásokra, címekre vonatkozó és további szöveges, numerikus és dátum formátumú leíró metaadatokat a kiegészítő leíró metaadatokra vonatkozó specifikációnak megfelelően kell átadni.
