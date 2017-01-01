2. melléklet a 34/2016. (XI. 30.) EMMI rendelethez

## Iratkezelési szoftverből történő iktatási nyilvántartással történő átvételre vonatkozó követelmények

1. A metadata.xml fájl tartalmára vonatkozó speciális előírások

1.1. A metadata.xml az iratkezelési szoftverből történő iktatási nyilvántartással való átvétel során az elektronikus átvételi csomag általános metaadatai mellett az irattári tervhez, az irattári tételekhez, az iktatókönyvekhez, az ügyiratokhoz, nyilvántartott iratokhoz is tartalmaz leíró, adminisztratív, fájlleíró és strukturális metaadatokat.

2. A leíró metaadatokra vonatkozó követelmények

2.1. A leíró metaadatokra vonatkozó követelményrendszer értelmezése:

a) A oszlop: A metaadatok szövegszerű megnevezése.

b) B oszlop: A metaadat szerepeltetésére vonatkozó megkötés. Az A oszlop szerinti metaadat megadása kötelező, ha a forrásrendszerben a metaadatra vonatkozó érték szerepel.

c) C oszlop: Az A oszlop szerinti metaadat ismételhetőségére vonatkozó előírás.

d) D oszlop: Az A oszlopban rögzített metaadat használatát segítő, magyarázó leírás.

2.2. Az iktatási hierarchiában az irattári terv leírásához használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az irattári terv egyedi azonosítójával. |

| 3 | Metaadat-leírás megnevezés | igen | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos az irattári terv megnevezésével. |

| 4 | Azonosító | igen | nem | Az irattári terv egyedi azonosítója Alapértelmezetten: „ITévszám”. |

| 5 | Irattári terv megnevezése | igen | nem | A szerv elsődleges besorolási sémájának a szöveges megnevezése. |

| 6 | Irathierarchia szintje | igen | nem | Az irattári tervnek a besorolási hierarchiában betöltött helye. Konstans érték: „Irattári terv”, amelynek reprezentációja „CLASSIFICATION”. |

| 7 | Tartalmi összefoglalás | nem | nem | Az irattári tervre vonatkozó rövid összefoglaló leírás. |

| 8 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 9 | Készítési idő | igen | nem | Az irattári terv készítésének dátuma. |

| 10 | Érvényességi idő kezdete | igen | nem | Az irattári terv érvényességi idejének kezdete. Alapértelmezetten azonos az átadott iratanyag időkörének kezdetével. Amennyiben az irattári terv egyes tételei az átadásra kerülő irategyüttes időköre alatt megváltoztak, vagy új irattári terv került elfogadásra, akkor a módosításokat az egyes tételek érvényességi idejének megfelelő beállításával kell jelölni úgy, hogy a tételek továbbra is egy egységes, egyetlen gyökérelemmel rendelkező irattári tervet alkossanak. Egyetlen elektronikus átvételi csomagban sem szerepelhet több irattári terv. |

| 11 | Érvényességi idő vége | igen | nem | Az irattári terv érvényességi idejének vége. Alapértelmezetten azonos az átadott iratanyag időkörének végével. Amennyiben az irattári terv egyes tételei az átadásra kerülő irategyüttes időköre alatt megváltoztak, vagy új irattári terv került elfogadásra, akkor a módosításokat az egyes tételek érvényességi idejének megfelelő beállításával kell jelölni úgy, hogy a tételek továbbra is egy egységes, egyetlen gyökérelemmel rendelkező irattári tervet alkossanak. Egyetlen elektronikus átvételi csomagban sem szerepelhet több irattári terv. |

2.3. Az iktatási hierarchiában az irattári tételekhez használt leíró metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az irattári tételszámmal. |

| 3 | Metaadat-leírás megnevezés | nem | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos az irattári tétel megnevezésével. |

| 4 | Irathierarchia szintje | igen | nem | Az irattári tételnek a besorolási hierarchiában betöltött helye. Konstans érték: „Irattári tétel”, amelynek reprezentációja: „CLASS”. |

| 5 | Irattári tételszám | igen | nem | Az irattári tétel azonosítója. Főszám/alszámos iktatás esetén az ügyirathoz (főszámhoz) kell rendelni az irattári tételt, amelynek megőrzési előírásai alapértelmezetten az ügyirat valamennyi nyilvántartott iratára (alszámára) egységesen érvényesek. Sorszámos iktatás esetén az irattári tételt közvetlenül az egyedi nyilvántartott irathoz kell rendelni. Az ügyiratokhoz vagy egyedi nyilvántartott iratokhoz csak olyan irattári tétel rendelhető, amelynek már nincsenek rész irattári tételei. |

| 6 | Irattári tételszám megnevezése | igen | nem |  |

| 7 | Készítési idő | igen | nem | Az irattári tétel keletkezési dátuma. |

| 8 | Tartalmi összefoglalás | nem | nem | Az irattári tétel tartalmára vonatkozó rövid összefoglaló leírás. |

| 9 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 10 | Érvényességi idő kezdete | igen | nem | Az irattári tétel érvényességi idejének kezdete. Alapértelmezetten minden irattári tétel érvényességi ideje azonos az adott elektronikus átvételi csomagban átadott teljes iratanyag időkörének kezdetével és végével. Amennyiben az irattári terv egyes tételei az átadásra kerülő irategyüttes időköre alatt megváltoztak, vagy új irattári terv került elfogadásra, akkor a módosításokat az egyes tételek érvényességi idejének megfelelő beállításával kell jelölni úgy, hogy a tételek továbbra is egy egységes, egyetlen gyökérelemmel rendelkező irattári tervet alkossanak. Egyetlen elektronikus átvételi csomagban sem szerepelhet több irattári terv. |

| 11 | Érvényességi idő vége | igen | nem | Az irattári tétel érvényességi idejének vége. Alapértelmezetten minden irattári tétel érvényességi ideje azonos az adott elektronikus átvételi csomagban átadott teljes iratanyag időkörének kezdetével és végével. Amennyiben az irattári terv egyes tételei az átadásra kerülő irategyüttes időköre alatt megváltoztak, vagy új irattári terv került elfogadásra, akkor a módosításokat az egyes tételek érvényességi idejének megfelelő beállításával kell jelölni úgy, hogy a tételek továbbra is egy egységes, egyetlen gyökérelemmel rendelkező irattári tervet alkossanak. Egyetlen elektronikus átvételi csomagban sem szerepelhet több irattári terv. |

| 12 | Alapértelmezett megőrzési mód | igen | nem | A megőrzési idő lejárta utáni alapértelmezetten elvégzendő teendő leírása. Lehetséges értékei: „Határidő nélkül megőrzendő”, „Lejárati idő végén felülvizsgálandó”, „Levéltárba adandó”, „Selejtezendő”. |

| 13 | Alapértelmezett megőrzési idő egység | igen | nem | Az irattári tételhez tartozó alapszintű megőrzési idő jellege. Lehetséges értékei: „Napok”, „Hetek”, „Hónapok”, „Évek”. |

| 14 | Alapértelmezett megőrzési idő érték | igen | nem | Az irattári tételhez tartozó alapszintű megőrzési idő értéke. |

2.4. Az iktatási hierarchiában az iktatókönyvekhez használt leíró metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az iktatókönyv egyedi azonosítójával. |

| 3 | Metaadat-leírás megnevezés | nem | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos az iktatókönyv megnevezésével. |

| 4 | Iktatókönyv azonosítója | igen | nem | Az iktatókönyv egyedi azonosítója. Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító. |

| 5 | Iktatókönyv megnevezése | igen | nem | Az iktatókönyvhöz kötődő, az átadó iratkezelési szabályzata alapján meghatározott szöveges megnevezés. |

| 6 | Irathierarchia szintje | igen | nem | Az iktatókönyvnek az irathierarchiában betöltött helye, a leírási szintje. Iktatókönyv esetében konstans érték: „Iktatókönyv”, amelynek reprezentációja: „REGISTER”. |

| 7 | Iktatókönyv nyitásának dátuma | igen | nem | Az adott iktatókönyv elektronikus iktatókönyvben történő létrehozásának, megnyitásának időpontja. |

| 8 | Iktatókönyv lezárásának időpontja | igen | nem | Az adott iktatókönyv elektronikus iktatókönyvben történő lezárásának időpontja. |

| 9 | Az iratképző neve | igen | nem | Az elektronikus átvételi csomagban szereplő iktatókönyvet keletkeztető szervezet megnevezése. |

| 10 | Idő(kör) kezdete | igen | nem | Az iktatókönyv iratanyaga létrehozásának kezdete. Alapértelmezetten az iktatókönyvben szereplő ügyiratok keletkezési évének január elseje. |

| 11 | Idő(kör) vége | igen | nem | Az iktatókönyv iratanyaga létrehozásának vége. Alapértelmezetten az iktatókönyvben szereplő ügyiratok keletkezési évének december 31-e. |

| 12 | Tartalmi összefoglalás | nem | nem | Az iktatókönyv tartalmára vonatkozó rövid összefoglaló leírás. |

| 13 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 14 | Részletes tartalmi leírás | nem | nem | A nyilvántartás tartalmát, időbeni, térbeli vonatkozásait részletesen bemutató leírás. |

| 15 | Földrajzi tárgyszavak | nem | igen | Az iktatókönyvhöz kapcsolódó jellemző földrajzi helyek, települések, címek. |

| 16 | Nyelv | nem | igen | Az iratanyag tartalmában használt nyelvekre vonatkozó leírás. |

| 17 | Hozzáférési korlátozások | igen | nem | Az iratanyag tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 18 | Felhasználási korlátozások | igen | nem | Az iratanyag reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 19 | Eredeti példányok léte és őrzőhelye | nem | igen | Ha az eredeti iratanyag nem kerül átvételre, csak annak másolata, akkor itt rögzíthető az eredeti irat pontos helyét meghatározó leírás. |

| 20 | Másolatok léte és őrzőhelye | nem | igen | Az átvett iratanyag másolatainak pontos helye. |

| 21 | Kapcsolódó leírási egységek | nem | igen | Az átvett iratanyag tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 22 | Leírási szabályok | nem | nem | Az iktatókönyvben vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.5. A főszám/alszámos iktatási hierarchiában az ügyiratokhoz használt leíró metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos az ügyirat iktatószámával. |

| 3 | Metaadat-leírás megnevezés | nem | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos az ügyirat tárgyával, kiegészítve az iktatószámmal. |

| 4 | Iktatószám | igen | nem | Az ügyirat azonosítója: a főszámot tartalmazó iktatószám, az ügyindító irat iktatószáma. |

| 5 | Ügyirat tárgya | igen | nem | Az ügyirat szöveges megnevezése, tárgya. |

| 6 | Irathierarchia szintje | igen | nem | Az ügyiratnak az irathierarchiában betöltött helye, a leírási szintje. Konstans érték: „file”. |

| 7 | Kezelési feljegyzések | nem | nem | Kezelési feljegyzések, amelyek az ügyintézés során keletkeztek. |

| 8 | Főszám iktatásának időpontja | igen | nem | Az ügyirat főszámos iktatásának időpontja. |

| 9 | Ügyirat lezárási időpontja | igen | nem | Az ügyirat lezárásának pontos időpontja. |

| 10 | Irattári tételszám | igen | nem | Annak az irattári tételnek az azonosítója, ahova az ügyirat be van sorolva. Az átadó iratkezelési szabályzatának melléklete alapján képzett, meghatározott formátumú azonosító. |

| 11 | Besorolás dátuma | igen | nem | Az irattári tételbe sorolás pontos időpontja. |

| 12 | Megőrzési mód | nem | nem | A megőrzési idő lejárta utáni teendő leírása, amely felülírhatja az irattári tervben meghatározott megőrzési mód értékét: Lehetséges értékei: „Határidő nélkül megőrzendő”, „Lejárati idő végén felülvizsgálandó”, „Levéltárba adandó”, „Selejtezendő”. |

| 13 | Tényleges megőrzési idő egység | nem | nem | Az ügyirathoz tartozó tényleges megőrzési idő jellege, amely felülírhatja az irattári tervben meghatározott megőrzési idő egység értékét: „Napok”, „Hetek”, „Hónapok”, „Évek”. |

| 14 | Tényleges megőrzési idő | nem | nem | Az ügyirathoz tartozó tényleges megőrzési idő, amely felülírhatja az irattári tervben meghatározott megőrzési idő értékét. |

| 15 | Tárgyszavak | nem | igen | Tárgyszókészlet. |

| 16 | Előirat iktatószáma | nem | nem | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú strukturált adat, amely alapján megállapítható egy adott ügyirattal szerelési kapcsolatban lévő további ügyirat egyedi azonosítója. |

| 17 | Utóirat iktatószáma | nem | nem | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú strukturált adat, amely alapján megállapítható egy adott ügyirattal szerelési kapcsolatban lévő további ügyirat egyedi azonosítója. |

| 18 | Kapcsolatos ügyiratok | nem | igen | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú strukturált adat, a kapcsolódó ügyirat(ok) egyedi azonosítója, amely alapján megállapítható(k) egy adott ügyirattal szerelési kapcsolatban nem lévő, de tárgya szerint kapcsolódó további ügyirat(ok). |

| 19 | Felelős | igen | nem | Az ügy elintézéséért felelős, megfelelő jogosultsággal rendelkező természetes személy(ek) vagy szervezeti egység. |

| 20 | Ügyintéző | nem | nem | Az ügyirat intézésére és a döntés előkészítésére kijelölt, megfelelő jogosultsággal rendelkező természetes személy(ek). |

| 21 | Ügyirat ügyintézési határideje | nem | nem | Az ügyintézés befejezésének tervezett/előírt határideje. |

| 22 | Ügyirat elintézési időpontja | nem | nem | Az ügyintézés befejezésének időpontja. |

| 23 | Intézés módja | nem | nem | Az ügyintézésre vonatkozó leírás. |

| 24 | Irattári átvevő | nem | nem | Ha az irat irattárba kerül, az irattári átvevő megnevezése. |

| 25 | Irattárba helyezés dátuma | nem | nem | Az átmeneti vagy a központi irattárba helyezés dátuma. |

| 26 | Selejtezhetőség dátuma | nem | nem | A tervezett selejtezési dátum. |

| 27 | Levéltárba adhatóság dátuma | nem | nem | A levéltárba adás tervezett dátuma. |

| 28 | Kölcsönzés időpontja | igen | igen |  |

| 29 | Kölcsönző személy | igen | igen | Kölcsönző természetes személy neve. |

| 30 | Kölcsönzést engedélyező személy | igen | igen | Kölcsönzést engedélyező természetes személy neve. |

| 31 | Kölcsönzési határidő | igen | igen | A kikölcsönzött ügyirat visszaadásának határideje. |

| 32 | Visszavétel kölcsönzésből időpontja | nem | igen | A kikölcsönzött ügyirat visszavételének ideje. |

| 33 | Visszavevő személy | nem | igen | Az ügyiratot visszavevő természetes személy neve. |

| 34 | Selejtezés időpontja | nem | nem | Selejtezés időpontja, amikor az irat a jóváhagyott selejtezési eljárás eredményeként selejtezésre került. |

| 35 | Selejtező személy | nem | nem | A selejtezést végző személy neve, amennyiben az irat selejtezésre került. |

| 36 | Ellenőr | nem | nem | A selejtezést ellenőrző személy neve, amennyiben az irat selejtezésre került. |

| 37 | Levéltárba adás dátuma | nem | nem |  |

| 38 | Levéltárnak átadó személy | nem | nem | Az átvétel során az iratátadó részéről az átadásért felelős személy. |

| 39 | Levéltári átvevő | nem | nem | Az átvétel során a levéltár részéről az átvételért felelős személy. |

| 40 | Irat helye | nem | nem | Irat fizikai helye. |

| 41 | Az iratképző neve | nem | nem | Az elektronikus átvételi csomagban szereplő ügyiratot keletkeztető szervezet megnevezése. Szervezeti változás, más szervezettől való iratátvétel során a nyilvántartásba felvett irat esetén az eredeti iratképzőt kell feltüntetni. |

| 42 | Idő(kör) kezdete | igen | nem | Az ügyirat létrehozásának kezdete. Értéke megegyezik a 8. sor Főszám iktatásának időpontja metaadat értékével. |

| 43 | Idő(kör) vége | igen | nem | Az ügyirat létrehozásának vége. Értéke megegyezik a 9. sor Ügyirat lezárási időpontja metaadat értékével. |

| 44 | Tartalmi összefoglalás | nem | nem | Az ügyirat tartalmára vonatkozó rövid összefoglaló leírás. |

| 45 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 46 | Részletes tartalmi leírás | nem | nem | Az ügyirat tartalmát, időbeni, térbeli vonatkozásait részletesen bemutató leírás. |

| 47 | Földrajzi tárgyszavak | nem | igen | Az ügyirathoz kapcsolódó jellemző földrajzi helyek, települések, címek. |

| 48 | Nyelv | nem | igen | Az ügyirat tartalmában használt nyelvekre vonatkozó leírás. |

| 49 | A megőrzés története | nem | nem | Az irategyüttes történetére vonatkozó mindazon információk, amelyek az azonosítás, a hitelesség vagy az értelmezés szempontjából fontosak lehetnek. Ide értendők a leírási egységet érintő tulajdoni változások, a megőrzésért és kezelésért felelős személyi/szervezeti változások, valamint mindazok a beavatkozások, így a rendezés, a konverzió, stb., amelyek kihatottak az ügyirat végleges állapotára és rendezettségére. |

| 50 | A levéltárba kerülés közvetlen forrása | nem | nem | Ha az iratanyag nem az iratképzőtől kerül átvételre, itt kell rögzíteni az átadóra vonatkozó információt. |

| 51 | A leírási egység szerkezete | nem | nem | Az ügyirat belső elrendezésére, felépítésére vonatkozó speciális információk. |

| 52 | Hozzáférési korlátozások | igen | nem | Az iratanyag tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 53 | Felhasználási korlátozások | igen | nem | Az iratanyag reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 54 | Eredeti példányok léte és őrzőhelye | nem | igen | Ha az eredeti iratanyag nem kerül átvételre, csak másolat, akkor itt rögzíthető az eredeti irat pontos helyét meghatározó leírás. |

| 55 | Másolatok léte és őrzőhelye | nem | igen | Az átvett ügyirat létező másolatainak pontos helye. |

| 56 | Kapcsolódó leírási egységek | nem | igen | Az ügyirat tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 57 | Leírási szabályok | nem | nem | Az ügyiratban vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.5.1. A kölcsönzés leírására használt 28-33. sorok metaadatai kötelező, ismételhető adatcsoportot alkotnak.

2.6. A főszám/alszámos iktatási hierarchiában az ügyiratokon belül nyilvántartott iratokhoz használt leíró metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat.leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos a nyilvántartott irat iktatószámával. |

| 3 | Metaadat-leírás megnevezés | nem | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos a nyilvántartott irat tárgyával, kiegészítve az iktatószámmal. |

| 4 | Irathierarchia szintje | igen | nem | A nyilvántartott iratnak az irathierarchiában betöltött helye, a leírási szintje. Konstans érték: „nyilvántartott irat”, amelynek reprezentációja „RECORD”. |

| 5 | Iktatószám | igen | nem | A nyilvántartott irat azonosítója: a főszámot és alszámot tartalmazó iktatószám. |

| 6 | Irat tárgya | igen | nem | A nyilvántartott irat szöveges megnevezése, tárgya. |

| 7 | Kezelési feljegyzések | nem | nem | Kezelési feljegyzések, amelyek az ügyintézés során keletkeztek. |

| 8 | Iktatás időpontja | igen | nem | Iktatási időpont megjelenítés dátum szerint (év, hó, nap). |

| 9 | Tárgyszavak | nem | igen | Tárgyszókészletből kiválasztott releváns tárgyszavak. |

| 10 | Ügyazonosító | nem | nem | Ügyazonosító, amennyiben az információ ügykezelő rendszerből érkezik. |

| 11 | Ügykezelő rendszer azonosítója | nem | nem | Az ügykezelő rendszer azonosítója, amennyiben az információ ügykezelő rendszerből érkezik. |

| 12 | Irat iránya | igen | nem | Az irat lehet bejövő, kimenő, vagy belső keletkezésű. |

| 13 | Beérkezés időpontja | nem | nem | Az iratnak az iratképzőhöz való érkezésének időpontja, bejövő irat esetében. Elektronikus érkeztetés esetén a dátum és idő adat. |

| 14 | Beérkezés módja | nem | nem | Az iratnak az iratképzőhöz való érkezésének módja, bejövő irat esetében. |

| 15 | Kézbesítés prioritása | nem | nem | Kézbesítés prioritása. Azonnali, sürgős, normál. |

| 16 | Érkeztető | nem | nem | Az érkeztető személy neve. |

| 17 | Érkeztetési azonosító | nem | nem | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító. |

| 18 | Küldő/feladó neve | nem | nem | Küldő/feladó természetes személy neve. |

| 19 | Küldő/feladó szervezet | nem | nem | Küldő/feladó jogi személy megnevezése. |

| 20 | Küldő/feladó címe | nem | nem |  |

| 21 | Címzett neve | nem | igen | A címzésben megjelölt természetes személy neve. |

| 22 | Címzett szervezet | nem | igen | A címzésben megjelölt jogi személy megnevezése. |

| 23 | Címzett címe | igen | igen |  |

| 24 | Adathordozó típusa | nem | nem | Az adathordozó típusa: papír, elektronikus, vegyes. |

| 25 | Küldemény bontója | nem | nem | Küldemény bontója, amennyiben nem azonos az érkeztetővel. |

| 26 | Bontás időpontja | nem | nem | A bontás időpontja megegyezhet az érkeztetés időpontjával. |

| 27 | Bontási megjegyzés | nem | nem | Szöveg típusú mező. |

| 28 | Iktató | nem | nem | Az iktatást végző személy neve. |

| 29 | Ügyirat állapota | nem | nem | Az iratképző által karbantartott és bővíthető listából választható, az ügyirat állapotát leíró adat. Alapértékei: iktatva, szignálva, törölve, határidőben, elintézett, átmeneti irattárban, központi irattárban, selejtezve, levéltárban. |

| 30 | Hivatkozási szám | nem | nem | Küldő saját iktatószáma (bejövő iratoknál), címzett saját iktatószáma (kimenő iratoknál). |

| 31 | Mellékletek | nem | nem | Mellékletek leírása. Szöveg típusú mező. |

| 32 | Mellékletek száma | nem | nem | Egy adott küldemény elemhez tartozó mellékletek száma. |

| 33 | Ügyintézési határidő | nem | nem | Az ügyintézés befejezésének tervezett / előírt határideje. |

| 34 | Elintézés időpontja | nem | nem | Az ügyintézés befejezésének időpontja. |

| 35 | Kiadmányozó | nem | nem | Az irat kiadmányozását elvégző, megfelelő jogosultsággal rendelkező természetes személy. |

| 36 | Kiadmányozás dátuma | nem | nem |  |

| 37 | Egyéb aláíró neve | nem | igen |  |

| 38 | Egyéb aláírás dátuma | nem | igen |  |

| 39 | Expediálás időpontja | nem | nem | Expediálás időpontja, kimenő iratok esetében. |

| 40 | Expediálás módja | nem | nem | Expediálás módja, kimenő iratok esetében. |

| 41 | Expediáló | nem | nem | Expediáló neve, kimenő iratok esetében. |

| 42 | Az iratképző neve | nem | nem | Az elektronikus átvételi csomagban szereplő nyilvántartott iratot keletkeztető szervezet megnevezése. Szervezeti változás, más szervezettől való iratátvétel során a nyilvántartásba felvett irat esetén az eredeti iratképzőt kell feltüntetni. |

| 43 | Idő(kör) kezdete | igen | nem | A nyilvántartott irat létrehozásának kezdete. Értéke megegyezik a 8. sor Iktatás dátuma mező értékével |

| 44 | Idő(kör) vége | igen | nem | A nyilvántartott irat létrehozásának vége. Értéke megegyezik a 35. sor Elintézés időpontja mező értékével. |

| 45 | Tartalmi összefoglalás | nem | nem | A nyilvántartott irat tartalmára vonatkozó rövid összefoglaló leírás. |

| 46 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 47 | Földrajzi tárgyszavak | nem | igen | Az irathoz kapcsolódó jellemző földrajzi helyek, települések, címek. |

| 48 | Nyelv | nem | igen | Az irat tartalmában használt nyelvekre vonatkozó leírás. |

| 49 | A megőrzés története | nem | nem | Az irategyüttes történetére vonatkozó mindazon információk, amelyek az azonosítás, a hitelesség vagy az értelmezés szempontjából fontosak lehetnek. Ide értendők a leírási egységet érintő tulajdoni változások, a megőrzésért és kezelésért felelős személyi/szervezeti változások, valamint mindazok a beavatkozások, így a rendezés, a konverzió, stb., amelyek kihatottak az ügyirat végleges állapotára és rendezettségére. |

| 50 | A levéltárba kerülés közvetlen forrása | nem | nem | Ha az iratanyag nem az iratképzőtől kerül átvételre, itt kell rögzíteni az átadóra vonatkozó információt. |

| 51 | A leírási egység szerkezete | nem | nem | A nyilvántarott irat belső elrendezésére, felépítésére vonatkozó információk. |

| 52 | Hozzáférési korlátozások | igen | nem | Az iratanyag tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 53 | Felhasználási korlátozások | igen | nem | Az iratanyag reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 54 | Eredeti példányok léte és őrzőhelye | nem | igen | Ha az eredeti iratanyag nem kerül átvétere, csak másolat, akkor itt rögzíthető az eredeti irat pontos helyét meghatározó leírás. |

| 55 | Másolatok léte és őrzőhelye | nem | igen | Az átadott iratanyag létező másolatainak pontos helye. |

| 56 | Kapcsolódó leírási egységek | nem | igen | Az átvett iratanyag tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 57 | Leírási szabályok | nem | nem | Az iratban vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.6.1. A címzett leírására használt 21-23. sorok metaadatai opcionális, csoportosan ismételhető adatcsoportot alkotnak.

2.7. A sorszámos (nem főszám/alszámos) iktatási rendszerben a nyilvántartott iratokat leíró metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Metaadat-leírás azonosító | igen | nem | A metaadat-leírás egyedi azonosítója. Alapértelmezetten azonos a nyilvántartott irat iktatószámával. |

| 3 | Metaadat-leírás megnevezés | nem | nem | A metaadat-leírás szöveges megnevezése. Alapértelmezetten azonos a nyilvántartott irat tárgyával, kiegészítve az iktatószámmal. |

| 4 | Iktatószám | igen | nem | A nyilvántartott irat azonosítója: sorszámos iktatószám. |

| 5 | Tárgy | igen | nem | A nyilvántartott irat szöveges megnevezése, tárgya. |

| 6 | Irathierarchia szintje | igen | nem | A nyilvántartott iratnak az irathierarchiában betöltött helye, a leírási szintje. Konstans érték: „record”. |

| 7 | Kezelési feljegyzések | nem | nem | Kezelési feljegyzések, amelyek az ügyintézés során keletkeztek. |

| 8 | Iktatás dátuma | igen | nem | Az iktatás időpontja. |

| 9 | Ügyirat lezárási időpontja | igen | nem | A sorszámosan nyilvántartott irat lezárási időpontja. |

| 10 | Irattári tételszám | igen | nem | Annak az irattári tételnek az azonosítója, ahova az ügyirat be van sorolva. Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító. |

| 11 | Besorolás dátuma | igen | nem | Az irattári tételbe sorolás pontos időpontja. |

| 12 | Megőrzési mód | nem | nem | A megőrzési idő lejárta utáni tényleges teendő leírása, amely felülírhatja az irattári tervben meghatározott megőrzési mód értékét: Lehetséges értékei: „Határidő nélkül megőrzendő”, „Lejárati idő végén felülvizsgálandó”, „Levéltárba adandó”, „Selejtezendő”. |

| 13 | Tényleges megőrzési idő egység | nem | nem | A sorszámos iktatásban nyilvántartott irathoz tartozó tényleges megőrzési idő jellege, amely felülírhatja az irattári tervben meghatározott megőrzési idő egység értékét: „Napok”, „Hetek”, „Hónapok”, „Évek”. |

| 14 | Tényleges megőrzési idő | nem | nem | A sorszámos iktatásban nyilvántartott irathoz tartozó megőrzési idő, amely felülírhatja az irattári tervben rögzített alapértelmezett megőrzési idő értékét. |

| 15 | Tárgyszavak | nem | igen | Tárgyszókészlet. |

| 16 | Előirat iktatószáma | nem | nem | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú strukturált adat, az előzmény ügyirat egyedi azonosítója, amely alapján megállapítható egy adott ügyirattal szerelési kapcsolatban lévő további ügyirat. |

| 17 | Utóirat iktatószáma | nem | nem | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú strukturált adat, az utóirat ügyiratának egyedi azonosítója, amely alapján megállapítható egy adott ügyirattal szerelési kapcsolatban lévő további ügyirat. |

| 18 | Kapcsolatos ügyiratok | nem | igen | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú strukturált adat, a kapcsolódó ügyirat(ok) egyedi azonosítója, amely alapján megállapítható(k) egy adott ügyirattal szerelési kapcsolatban nem lévő, de tárgya szerint kapcsolódó további ügyirat(ok). |

| 19 | Felelős | igen | nem | Az ügy elintézéséért felelős, megfelelő jogosultsággal rendelkező természetes személy(ek) vagy szervezeti egység. |

| 20 | Ügyintéző | nem | igen | Ügyintéző neve. |

| 21 | Irat ügyintézési határideje | nem | nem | Az ügyintézés befejezésének tervezett határideje. |

| 22 | Elintézés időpontja | nem | nem | Az ügyintézés befejezésének tényleges időpontja. |

| 23 | Intézés módja | nem | nem | Az ügyintézésre vonatkozó leírás. |

| 24 | Irattári átvevő | nem | nem | Ha az irat irattárba kerül az irattári átvevő megnevezése. |

| 25 | Irattárba helyezés dátuma | nem | nem | Az átmeneti vagy a központi irattárba helyezés dátuma. |

| 26 | Selejtezhetőség időpontja | nem | nem | A tervezett selejtezési időpont. |

| 27 | Levéltárba adhatóság dátuma | nem | nem | A levéltárba adás tervezett időpontja. |

| 28 | Kölcsönzés időpontja | igen | igen |  |

| 29 | Kölcsönző személy | igen | igen | Kölcsönző természetes személy neve. |

| 30 | Kölcsönzést engedélyező személy | igen | igen | Kölcsönzést engedélyező természetes személy neve. |

| 31 | Kölcsönzési határidő | igen | igen | A kikölcsönzött irat visszaadásának határideje. |

| 32 | Visszavétel kölcsönzésből időpontja | nem | igen | A kikölcsönzött ügyirat visszavételének ideje. |

| 33 | Visszavevő személy | nem | igen | Az iratot visszavevő természetes személy neve. |

| 34 | Selejtezés időpontja | nem | nem | Selejtezés időpontja, amennyiben az irat selejtezésre került. |

| 35 | Selejtező | nem | nem | A selejtezést végző személy neve, amennyiben az irat selejtezésre került. |

| 36 | Ellenőr | nem | nem | A selejtezést ellenőrző személy neve, amennyiben az irat selejtezésre került. |

| 37 | Levéltárba adás dátuma | nem | nem |  |

| 38 | Levéltárnak átadó személy | nem | nem | Az átvétel során az átadó részéről az átadásért felelős személy neve. |

| 39 | Levéltári átvevő | nem | nem | Az átvétel során a levéltár részéről az átvételért felelős személy neve. |

| 40 | Irat helye | nem | nem | Az irat fizikai helye. |

| 41 | Ügyazonosító | nem | nem | Ügyazonosító, amennyiben az információ ügykezelő rendszerből érkezik. |

| 42 | Ügykezelő rendszer azonosítója | nem | nem | Az ügykezelő rendszer azonosítója, amennyiben az információ ügykezelő rendszerből érkezik. |

| 43 | Irat irány | igen | nem | Az irat lehet bejövő, kimenő, vagy belső keletkezésű. |

| 44 | Beérkezés időpontja | nem | nem | Az iratnak az iratképzőhöz való érkezésének időpontja, bejövő irat esetében. Elektronikus érkeztetés esetén a dátum és idő adat. Manuális érkeztetés esetén a beérkezés tényleges dátuma. |

| 45 | Beérkezés módja | nem | nem | Az iratnak az iratképzőhöz való érkezésének módja, bejövő irat esetében. |

| 46 | Kézbesítés prioritása | nem | nem | Kézbesítés prioritása. Azonnali, sürgős, normál. |

| 47 | Érkeztető | nem | nem | Az érkeztető személy neve. |

| 48 | Érkeztetési azonosító | nem | nem | Az átadó iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító. |

| 49 | Küldő / feladó neve | nem | nem | Küldő / feladó természetes személy neve. |

| 50 | Küldő / feladó szervezet | nem | nem | Küldő / feladó jogi személy megnevezése. |

| 51 | Küldő / feladó címe | nem | nem |  |

| 52 | Címzett neve | nem | igen | A címzésben megjelölt természetes személy neve. |

| 53 | Címzett szervezet | nem | igen | A címzésben megjelölt jogi személy megnevezése. |

| 54 | Címzett címe | igen | igen |  |

| 55 | Adathordozó típusa | nem | nem | Az adathordozó típusa: papír, elektronikus, vegyes. |

| 56 | Küldemény bontója | nem | nem | A küldemény bontója, amennyiben nem azonos az érkeztetővel. |

| 57 | Bontás időpontja | nem | nem | A bontás időpontja megegyezhet az érkeztetés időpontjával. |

| 58 | Bontási megjegyzés | nem | nem | Szöveg típusú mező. |

| 59 | Iktató | nem | nem | Az iktatást végző személy neve. |

| 60 | Ügyirat állapota | nem | nem | Az iratképző által karbantartott és bővíthető listából választható, az ügyirat állapotát leíró adat. Alapértékei: iktatva, szignálva, törölve, határidőben, elintézett, átmeneti irattárban, központi irattárban, selejtezve, levéltárban. |

| 61 | Hivatkozási szám | nem | nem | Küldő saját iktatószáma (bejövő iratoknál), címzett saját iktatószáma (kimenő iratoknál). |

| 62 | Mellékletek | nem | igen | Szöveg típusú mező. Mellékletek leírása. |

| 63 | Mellékletek száma | nem | nem | Egy adott küldemény elemhez tartozó mellékletek száma. |

| 64 | Ügyintézési határidő | nem | nem | Az ügyintézés befejezésének tervezett / előírt határideje. |

| 65 | Ügyintézés időpontja | nem | nem | Az ügyintézés befejezésének tényleges időpontja. |

| 66 | Kiadmányozó | nem | nem | Az irat kiadmányozását elvégző, megfelelő jogosultsággal rendelkező természetes személy neve. |

| 67 | Kiadmányozás dátuma | nem | nem |  |

| 68 | Egyéb aláíró neve | nem | igen |  |

| 69 | Egyéb aláírás dátuma | nem | igen |  |

| 70 | Expediálás időpontja | nem | nem | Az expediálás időpontja, kimenő iratok esetében. |

| 71 | Expediálás módja | nem | nem | Az expediálás módja, kimenő iratok esetében. |

| 72 | Expediáló | nem | nem | Az expediáló neve, kimenő iratok esetében. |

| 73 | Az iratképző neve | nem | nem | Az elektronikus átvételi csomagban szereplő nyilvántartott iratot keletkeztető szervezet megnevezése. Szervezeti változás, más szervezettől való iratátvétel során a nyilvántartásba felvett irat esetén az eredeti iratképzőt kell feltüntetni. |

| 74 | Idő(kör) kezdete | igen | nem | A nyilvántartott irat létrehozásának kezdete. Értéke megegyezik a 8. sor Iktatás dátuma metaadat értékével. |

| 75 | Idő(kör) vége | igen | nem | A nyilvántartott irat létrehozásának vége. Értéke megyezik a 22. sor Elintézés időpontja metaadat értékével. |

| 76 | Tartalmi összefoglalás | nem | nem | A nyilvántartott irat tartalmára vonatkozó rövid összefoglaló leírás. |

| 77 | Megjegyzés | nem | nem | Szöveg típusú mező. |

| 78 | Földrajzi tárgyszavak | nem | igen | Az irathoz kapcsolódó jellemző földrajzi helyek, települések, címek. |

| 79 | Nyelv | nem | igen | Az irat tartalmában használt nyelvekre vonatkozó leírás. |

| 80 | A megőrzés története | nem | nem | Az irategyüttes történetére vonatkozó mindazon információk, amelyek az azonosítás, a hitelesség vagy az értelmezés szempontjából fontosak lehetnek. Ide értendők a leírási egységet érintő tulajdoni változások, a megőrzésért és kezelésért felelős személyi/szervezeti változások, valamint mindazok a beavatkozások, így a rendezés, a konverzió, stb., amelyek kihatottak az ügyirat végleges állapotára és rendezettségére. |

| 81 | A levéltárba kerülés közvetlen forrása | nem | nem | Ha az iratanyag nem az iratképzőtől kerül átadásra itt kell rögzíteni az átadóra vonatkozó információt. |

| 82 | A leírási egység szerkezete | nem | nem | A nyilvántarott irat belső elrendezésére, felépítésére vonatkozó információk. |

| 83 | Hozzáférési korlátozások | igen | nem | Az iratanyag tartalmának hozzáférhetőségét, annak korlátozását, illetve a hozzáférést befolyásoló információ. Szükséges azt is rögzíteni, ha nincs a hozzáféréssel kapcsolatos korlátozás. |

| 84 | Felhasználási korlátozások | igen | nem | Az iratanyag reprodukcióját érintő korlátozásokhoz kapcsolódó leírás. Szükséges azt is rögzíteni, ha nincs a reprodukcióval kapcsolatos korlátozás. |

| 85 | Eredeti példányok léte és őrzőhelye | nem | igen | Ha az eredeti iratanyag nem kerül átadásra, csak másolat, akkor itt rögzíthető az eredeti irat pontos helyét meghatározó leírás. |

| 86 | Másolatok léte és őrzőhelye | nem | igen | Az átvett iratanyag létező másolatainak pontos helye. |

| 87 | Kapcsolódó leírási egységek | nem | igen | Az átvett iratanyag tartalmához kapcsolódó olyan külső iratanyagokra vonatkozó leírás, amelyek az iratképző belső iratnyilvántartásának nem részei. |

| 88 | Leírási szabályok | nem | nem | Az iratban vagy annak leírásában alkalmazott szabályokat - rövidítéseket, kódokat, külső szabványokat - ismertető leírás. |

2.7.1. A kölcsönzés leírására használt 28-33. sorok metaadatai opcionális, csoportosan ismételhető adatcsoportot alkotnak.

2.7.2. A címzett leírására használt 52-54. sorok metaadatai opcionális, ismételhető adatcsoportot alkotnak.

3. Az 1. melléklet 2.8.2. pontja szerinti strukturális divízió elemet kell készíteni valamennyi irattári tétel, iktatókönyv, ügyirat és nyilvántartott irat számára.
