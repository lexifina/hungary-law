## 16. § A rendelet tervezetének a műszaki szabályokkal és az információs társadalom szolgáltatásaira vonatkozó szabályokkal kapcsolatos információszolgáltatási eljárás megállapításáról szóló, 2015. szeptember 19-i (EU) 2015/1535 európai parlamenti és tanácsi irányelv 5–7. cikke szerinti előzetes bejelentése megtörtént.

1. melléklet a 34/2016. (XI. 30.) EMMI rendelethez

## Az elektronikus levéltári átvételi csomag műszaki követelményei

1. Az elektronikus átvételi csomag felépítése

1.1. Az elektronikus átvételi csomag szerkezete

A. [ellenőrző összeg].txt

B. [konténer állomány].zip

a) header

aa) metadata.xml

b) content

ba) data

bb) documentation

1.2. Az ellenőrző összeg szöveges állománya négy sort tartalmaz az alábbiak szerint:

a) metadata.xml: [a fájl terjedelme (byte)]

b) [algoritmus elnevezése]: [a metadata.xml fájl ellenőrző összege a 6. § (3) bekezdés szerinti adatséma-leírásban megadott algoritmus szerint]

c) [konténer fájl neve]: [a fájl terjedelme (byte)]

d) [algoritmus elnevezése]: [a konténer fájl ellenőrző összege az MNL ajánlásban megadott algoritmus szerint]

2. A metadata.xml állomány tartalma

2.1. A metadata. xml állomány metaadataira vonatkozó követelményrendszer értelmezése:

a) A oszlop: A metaadatok szövegszerű megnevezése.

b) B oszlop: A metaadat szerepeltetésére vonatkozó megkötés.

c) C oszlop: Az A oszlop szerinti metaadat ismételhetőségére vonatkozó előírás.

d) D oszlop: Az A oszlopban rögzített metaadat használatát segítő, magyarázó leírás.

2.2. A metadata.xml gyökér elemének leírására használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | Az elektronikus átvételi csomag egyedi azonosítója, amely azonos lehet a csomag egyedi elnevezésével. |

| 3 | Leírás | nem | nem | Az elektronikus átvételi csomag tartalmának rövid leírása. |

| 4 | Csomag típus | igen | nem | Meghatározza az elektronikus átvételi csomag szerepét az archiválási folyamatban. Konstans érték: „SIP”. |

2.3. A metadata.xml fejléc elemének leírására használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Létrehozási idő | igen | nem | Az elektronikus átvételi csomag létrehozásának dátuma és időpontja. |

| 3 | Státusz | igen | nem | Az elektronikus átvételi csomag státusza. Lehetséges értékei: „Új csomag”, amelynek reprezentációja „NEW”; „Helyettesítő csomag”, amelynek reprezentációja „REPLACEMENT”; „Teszt csomag”, amelynek reprezentációja „TEST”. |

| 4 | Átadás típusa | igen | nem | Az elektronikus átvételi csomag átadási típusa: „tanúsított iratkezelési szoftver”, amelynek reprezentációja „TANÚSÍTOTT IKTATÁS”; „iktatási iratnyilvántartás”, amelynek reprezentációja „STRUKTURÁLT IKTATÁS”; „nem iktatási típusú iratnyilvántartás, iratszintű metaadatokkal”, amelynek reprezentációja „STRUKTURÁLT IRATNYILVÁNTARTÁS”; „nem iratszintű metaadatok”, amelynek reprezentációja „STRUKTURÁLATLAN”. |

| 5 | Átvétel típusát leíró dokumentum | igen | nem | Az elektronikus átvételi csomag átvételi típusát részletesen meghatározó dokumentum címe és elérhetősége. |

| 6 | Levéltári átadás-átvételi megállapodás | igen | nem | Az iratátadó és a levéltár között létrejött levéltári átadás-átvételi megállapodás iktatószáma és dátuma. A két adatot pontosvesszővel kell elválasztani. |

| 7 | Korábbi levéltári átadás-átvételi megállapodás | nem | igen | Az elektronikus átvételi csomag tartalmára vonatkozó korábbi levéltári átadás-átvételi megállapodás iktatószáma és dátuma, amely pl. két levéltár közötti átadás esetén nyújt információt az iratképzőtől való átvétel körülményeire vonatkozóan. |

| 8 | Beküldés | nem | nem | A megállapodás alapján az átvétel több szakaszra tagolva is megvalósítható. A metaadat tartalmazza a beküldési szakasz megnevezését, azonosítóját. |

| 9 | Beküldési sorszám | nem | nem | Az átvételi szakasz során több csomag is átadható. A metaadat tartalmazza az elektronikus átvételi csomag sorszámát a beküldési szakaszon belül. |

| 10 | Levéltári anyag törzsszáma | nem | nem | Az elektronikus átvételi csomagban lévő levéltári anyaghoz kapcsolódó, már a levéltár őrzésében lévő anyag törzsszáma. |

| 11 | Levéltári anyag megelőző törzsszáma | nem | igen | Az elektronikus átvételi csomagban lévő levéltári anyag korábbi törzsszáma két levéltár közötti átadás esetén nyújt információt az iratképzőtől való átvétel körülményeire vonatkozóan. |

| 12 | Rendelkezésre állás | nem | nem | Az elektronikus átvételi csomag tartalmához történő hozzáférés korlátozásnak jelölése. |

| 13 | Selejtezhetőség | nem | nem | Ez az adat lehetővé teszi, hogy az elektronikus átvételi csomag szintjén meghatározható legyen az átadott állomány selejtezhetősége, amire „Teszt” típusú átvétel során lehet szükség. Lehetséges értékei: „Selejtezhető”, „Nem selejtezhető”. |

| 14 | Iratképző neve | igen | nem | Az elektronikus átvételi csomagban szereplő iratokat keletkeztető szervezet pontos neve. |

| 15 | Iratképző azonosítója | igen | nem | Az elektronikus átvételi csomagban szereplő iratokat keletkeztető szervezet egyedi azonosítója. |

| 16 | Iratkezelési szoftver neve | igen | nem | Annak az iratkezelési szoftvernek vagy más informatikai rendszernek a neve, amelyből az elektronikus átvételi csomagban szereplő adatok, iratok származnak. |

| 17 | Iratkezelési szoftver verziója | nem | nem | Annak az iratkezelési szoftvernek vagy más infromatikai rendszernek a verziószáma, amelyből az elektronikus átvételi csomagban szereplő adatok, iratok származnak. |

| 18 | Iratátadó szerv neve | igen | nem | Az elektronikus átvételi csomagot készítő szervezet neve, amely alapértelmezetten azonos az iratképzővel. |

| 19 | Iratátadó szerv azonosítója | nem | nem | Az elektronikus átvételi csomagot készítő szervezet egyedi azonosítója, amely alapértelmezetten azonos az iratképzővel. |

| 20 | Közreműködő neve | nem | igen | Az elektronikus átvételi csomag készítésében közreműködő természetes személy vagy szervezet neve. |

| 21 | Közreműködő azonosítója | nem | igen | Az elektronikus átvételi csomag készítésében közreműködő természetes személy vagy szervezet egyedi azonosítója. |

| 22 | Átadó rendszer neve | nem | nem | Annak az informatikai rendszernek a neve, amely az elektronikus átvételi csomagot generálta. |

| 23 | Átadó rendszer verziója | nem | nem | Annak az informatikai rendszernek a verziószáma, amelyből az elektronikus átvételi csomagban szereplő adatok, iratok származnak. |

| 24 | Kapcsolattartó neve | nem | igen | A beadó szervezet részéről az átadásért felelős személy neve. |

| 25 | Kapcsolattartási adatok | nem | igen | A beadó szervezet részéről az átadásért felelős személy telefonszáma vagy e-mail címe. |

| 26 | Illetékes levéltár neve | igen | nem | Annak a levéltári szervezetnek a neve, amely az elektronikus átvételi csomag befogadását végzi. |

| 27 | Illetékes levéltár azonosítója | igen | nem | Annak a levéltári szervezetnek az azonosítója, amely az elektronikus átvételi csomag befogadását végzi. |

2.4. A beágyazott metaadat-reprezentációk leírására használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | nem | nem | A metaadat-leírás egyedi azonosítója. |

| 3 | Megnevezés | nem | nem | Címke az adott metaadat-tartalom dokumentumon belüli azonosításához. |

| 4 | Metaadat- reprezentáció | igen | nem | Az elektronikus átvételi csomagba beágyazott metaadatséma típusa, amely a technikai specifikáció által lehetővé tett értékeket veheti fel. |

| 5 | Egyéb metaadat- reprezentáció | nem | nem | Azon metaadatséma típusok megadása, amelyek a technikai specifikációtól eltérnek. |

| 6 | Metaadat- reprezentáció verzió | nem | nem | Alkalmazott metaadatséma-típus verziója. |

2.5. A metadata.xml-ben a leíró metaadatok tartalmazzák az elektronikus átvételi csomagban átadásra kerülő iratok leíró metaadatait, illetve a dokumentációhoz tartozó fájlok leírását.

2.5.1. A leíró metaadatok reprezentációjának leírására használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | A leíró metaadatok sémájának egyedi azonosítója. |

| 3 | Csoport azonosító | nem | nem | Egy csoporthoz tartozó több metaadat-szekció fogható össze vele. Felhasználható, ha a megváltozott adattartalmakat ugyanazoknál az objektumoknál tároljuk (változáskövetés). |

| 4 | Létrehozási idő | nem | nem | A metaadat létrehozásának dátuma és időpontja. |

| 5 | Metaadat státusza | nem | nem | A metaadat státusza. Lehetséges értékei: „Elavult”, amelynek reprezentációja „SUPERCEDED”; „Aktuális”, amelynek reprezentációja „CURRENT”. |

2.6. A metadata.xml-ben az adminisztratív metaadatok tartalmazzák az elektronikus átvételi csomagban átadásra kerülő adatok struktúrájának, adatfájljainak, a leíró metaadainak és maguknak az adminisztratív metaadatoknak a metaadatait.

2.6.1. A metadata.xml-ben a technikai metaadatok használata opcionális. A leírásra használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | A technikai metaadatok metaadatcsoportjának egyedi azonosítója. |

| 3 | Csoport azonosító | nem | nem | Egy csoporthoz tartozó több metaadat-szekció fogható össze vele. Felhasználható, ha a megváltozott adattartalmakat ugyanazoknál az objektumoknál tároljuk (változáskövetés). |

| 4 | Adminisztratív metaadatok azonosítója | nem | nem | Hivatkozás az adminisztratív metaadatok csoportjának azonosítójára. |

| 5 | Létrehozási idő | nem | nem | A metaadatcsoport létrehozásának dátuma és időpontja. |

| 6 | Státusz | nem | nem | A metaadat státusza. Lehetséges értékei: „Elavult”, amelynek reprezentációja „SUPERCEDED”; „Aktuális”, amelynek reprezentációja „CURRENT”. |

2.6.2. A metadata.xml-ben a szerzői jogoknak a leíró metaadatoktól független, önálló metaadat-reprezentációban való megadása opcionális. A leírásra használt metaadatok:

|  | A | B | C |  |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | A felhasználási jogokra vonatkozó metaadatcsoport egyedi azonosítója. |

| 3 | Csoport azonosító | nem | nem | Egy csoporthoz tartozó több metaadat-szekció fogható össze vele. Felhasználható, ha megváltozott adattartalmakat ugyanazoknál az objektumoknál tároljuk (változáskövetés.) |

| 4 | Adminisztratív metaadatok azonosítója | nem | nem | Hivatkozás az adminisztratív metaadatok csoportjának azonosítójára. |

| 5 | Létrehozási idő | nem | nem | A metaadatcsoport létrehozásának dátuma és időpontja. |

| 6 | Státusz | nem | nem | A metaadat státusza. Lehetséges értékei: „Elavult”, amelynek reprezentációja „SUPERCEDED”; „Aktuális”, amelynek reprezentációja „CURRENT”. |

2.7. A metadata.xml-ben rögzíteni kell az egyes adatfájlokhoz tartozó, csoportosításukra, azonosításukra és elérésükre vonatkozó metaadatokat. Az egyes adatfájlokra és azok csoportjaira vonatkozó metaadatok megadása kötelező.

2.7.1. A metadata.xml-ben az egyes fájlcsoportokhoz tartozó metaadatokkal kell leírni az egyedi fájlok logikai csoportjaihoz rendelt metaadatokat. A leírásra használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | A content mappában elhelyezett fájlok csoportjának egyedi azonosítója. |

| 3 | Adminisztratív metaadatok azonosítója | nem | nem | Hivatkozás az adminisztratív metaadatok csoportjának azonosítójára. |

| 4 | Használat | nem | nem | A csoportban található fájlok felhasználási területe (archív, referencia, nézőkép, egyéb). |

2.7.2. A metadata.xml-ben az egyes fájlokhoz tartozó metaadatokkal kell leírni az egyedi fájlok alapadatait és hivatkozásait. A leírásra használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | A content mappában elhelyezett fájl egyedi azonosítója. |

| 3 | MIME típus | nem | nem | A fájlhoz társított IANA MIME típus. |

| 4 | Sorszám | nem | nem | Ha a fájl egy csoport tagja, akkor a csoport részeként kapott sorszámot tartalmazza. |

| 5 | Méret | nem | nem | Fájl mérete bájtban megadva. |

| 6 | Létrehozás dátuma | nem | nem | A fájl létrehozásának dátuma és időpontja. |

| 7 | Ellenőrző összeg | igen | nem | A fájl sértetlenségét igazoló ellenőrző összeg értéke. |

| 8 | Ellenőrző összeg típusa | nem | nem | Az ellenőrző összeg létrehozásához használt algoritmus. |

| 9 | Adminisztratív metaadatok azonosítója | nem | nem | Hivatkozás az adminisztratív metaadatok csoportjának azonosítójára. |

| 10 | Leíró metaadatok azonosítója | nem | nem | Hivatkozás a leíró metaadatok csoportjának azonosítójára. |

| 11 | Fájlcsoport azonosító | nem | nem | Annak a csoportnak az azonosítója, amelyikhez a fájl tartozik. |

| 12 | Használat | nem | nem | A csoportban található fájlok felhasználási területe (archív, referencia, nézőkép, egyéb). |

2.7.2.1. A fájlok elérési útjának megadásakor a fájlhierarchia kiinduló gyökéreleme a content mappa. A content mappa data és documentation mappájában elhelyezett állományok elhelyezkedésének leírására használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | Nem | A fájl helyét meghatározó hivatkozás azonosítója. |

| 3 | Hely típus | igen | Nem | A fájl helyét meghatározó hivatkozás típusa. |

2.8. A metadata.xml-ben a logikai struktúrához tartozó metaadatokkal kell leírni az irategyüttes logikai struktúráit, azok hierarchikus elrendezését.

2.8.1. A hierarchikus elrendezés három típusa használható:

a) aggregáció: a nyilvántartott iratok fizikai elrendezése: iktatókönyvek, ügyiratok, irategyüttesek, iratok hierarchiája;

b) besorolás, a nyilvántartott iratok logikai elrendezése: az irattári terv vagy besorolási séma hierarchiája;

c) dokumentáció: a csomag adattartalmától független, a tartalom értelmezését támogató dokumentumok összessége.

2.8.2. A logikai struktúra egyes komponenseinek metaadatait egymásba ágyazott metaadatcsoportokban (a továbbiakban: divízió) kell megadni. Minden divízió elem egy vagy több fájlhoz kapcsolódhat, amelyek együttesen az adott strukturális elem teljes tartalmát magukba foglalják. A divízió leírására használt metaadatok:

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Azonosító | igen | nem | A fájlok logikai hierarchiában való elrendezését rögzítő metaadatcsoport egyedi azonosítója. |

| 3 | Sorrend | nem | nem | A többféle logikai hierarchia sorrendjét leíró numerikus metaadat. |

| 4 | Névsorrend | nem | nem | A többféle logikai hierarchia sorrendjét leíró alfabetikus metaadat. |

| 5 | Címke | nem | nem | A logikai hierarchia tartalmának azonosítására szolgáló metaadat. |

| 6 | Leíró metaadatok azonosító | igen | nem | Hivatkozás a leíró metaadatok csoportjának azonosítójára. |

| 7 | Adminisztratív metaadatok azonosítója | nem | nem | Hivatkozás az adminisztratív metaadatok csoportjának azonosítójára. |

| 8 | Típus | igen | nem | A logikai hierarchia típusának meghatározása. |

2.8.2.1. A logikai struktúrához tartozó metaadatok és a fizikai elhelyezkedés közötti kapcsolatot a fájlmutató hivatkozás metaadattal kell megadni. A metaadat megadása kötelező.

|  | A | B | C | D |

| 1 | Megnevezés | Kötelező | Ismételhető | Leírás |

| 2 | Fájl azonosító | igen | nem | A logikai hierarchia elemének az egyes fájlokkal való összekapcsolását biztosító metaadat. |
