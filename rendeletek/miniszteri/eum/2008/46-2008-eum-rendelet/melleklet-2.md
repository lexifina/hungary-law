## „1. számú melléklet az 53/2007. (XII. 7.) EüM rendelethez

## Az extra vonalkód adattartalma és műszaki leírása

## 1. Az „extra vonalkód” adattartalma:

## a) a vény felírás dátuma,

## b) a TAJ szám,

## c) a BNO kód,

## d) a vény felírás jogcíme,

## e) a helyettesíthetőség,

## f) a felírt gyógyszer TTT kódja,

## g) a felírt gyógyszer mennyisége,

## h) a külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslatot adó orvos pecsétszáma,

## i) a külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslat keletkezésének ideje a vény felírás időpontjához viszonyítva,

## j) a szoftver minősítésének azonosító kódja,

## k) a program által a vénynyomtatás során használt gyógyszertörzs érvényességi idejének kezdő dátuma.

## 2. Az „extra vonalkód” adattartalmának kódolása:

## a) A vény felírás dátuma: 1-től 366-ig terjedő, három számjegyből álló szám, amely azt jelzi, hogy a vényfelírás az év hányadik napján történt.

## b) A TAJ szám 9 számjegye.

## c) A BNO-kód: a nyomtatott vényen szereplő BNO-kód numerikus formában, mely úgy áll elő, hogy a BNO-kód első karaktere helyett minden esetben az adott karakter ASCII kódja szerepel, 2 számjegy hosszúságban. Ha az eredeti BNO-kód negyedik karaktere „H”, akkor helyette a vonalkódban „0” érték szerepel, továbbá az ma) pont szerinti bináris szám értéke „1”. Ha az eredeti BNO-kód negyedik karaktere nem „H”, akkor az ma) pont szerinti bináris szám értéke „0”.

## d) A vény felírás jogcíme:

| Általános jogcím | 1 |

| HM jogcímen | 2 |

| Közgyógyellátási jogcím | 3 |

| Üzemi baleset | 4 |

| Eü. rend. jogcím | 5 |

| Eü. tér. köt. jogcím | 6 |

| Teljes ár | 7 |

| Eü. rend. és közgyógyellátási jogcím együtt | 8 |

| Eü. tér. köt. és közgyógyellátási jogcím együtt | 9 |

## e) A helyettesíthetőség: értéke a „0” (nulla) vagy az „1” (egy) lehet. Az „1” jelentése, hogy a gyógyszer helyettesíthető, a „0” jelentése, hogy a gyógyszer nem helyettesíthető. A helyettesíthetőség értékét az mb) pont szerinti bináris számban kell feltüntetni.

## f) A felírt gyógyszer TTT kódja, 9 számjegy hosszúságban.

## g) A felírt gyógyszer mennyisége: jobbra igazított, vezető nullákkal feltöltött, 3 karakter hosszúságú numerikus adat.

## h) A külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslatot adó orvos pecsétszáma, 5-nél kevesebb számjegyből álló pecsétszám esetén vezető nullával feltöltve. Ha az orvosi pecsétszám 6 számjegyből áll és az első számjegye „1”, azaz a pecsétszám értéke 100 000–199 999 közötti, akkor az mc) pont szerinti bináris szám értéke „1”, különben „0”. Amennyiben a gyógyszer rendelése szakorvosi javaslathoz nem kötött, akkor 5 karakter hosszúságban nullával feltöltve.

## i) A külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslat időpontja és a vényfelírás időpontja között eltelt idő hónapban kifejezve, egész hónapra lefelé kerekítve, 2 számjegy hosszúságban. Amennyiben olyan gyógyszerről van szó, amely esetében a szakorvosi javaslat alapján határozatlan ideig lehet gyógyszert felírni és a javaslat 96 hónapnál régebbi, minden esetben a „99” számjegyeket kell használni. Amennyiben a gyógyszer rendelése szakorvosi javaslathoz nem kötött, akkor 2 karakter hosszúságban nullával feltöltve.

## j) A Felügyelet által a szoftver minősítésekor adott 3 számjegyből álló szám.

## k) A program által a vénynyomtatás során használt gyógyszertörzs érvényességi ideje kezdő dátumának hónapja és a vényfelírás dátumának hónapja között eltelt hónapok száma, egész hónapban számítva, lefelé kerekítve, 1 számjegy hosszúságban. Ha a két dátumban a hónapok megegyeznek, akkor a karakter értéke „0”; ha a gyógyszertörzs érvényességi ideje kezdő dátumából a hónap egy hónappal korábbi, mint a vényfelírás dátuma, akkor a karakter értéke „1” és így tovább.

## l) Az ma), mb) és mc) alpontok értéke alapján képzett bináris szám decimális megfelelője, 1 számjegy hosszúságban. A képzett decimális szám bináris összetevői sorrendben az alábbiak:

## ma) Ha a vényen szereplő BNO-kód negyedik karaktere „H”, akkor értéke „1”, különben „0”.

## mb) Ha a gyógyszer az e) pont szerint helyettesíthető, értéke „1”, különben „0”.

## mc) Amennyiben a h) pont szerinti orvos pecsétszáma hat számjegyű és első számjegye „1”, akkor értéke „1”, különben „0”.

## 3. Példa „extra vonalkód” adattartalmára és annak kódolására:

| Pozíció | Karakter tartalma | Hossz | Példa | Kódolt érték |

| 1–3 | a vény felírás dátuma | 3 | 2007. 02. 02 | 033 |

| 4–12 | a TAJ szám | 9 | 238338038 | 238338038 |

| 13–18 | a BNO kód | 6 | I10H0 | 731000 |

| – |  | – | +,,H” | → binA = 1 |

| 19–19 | a vény felírás jogcíme | 1 | Általános | 1 |

| – | a helyettesíthetőség | – | Helyettesíthető | → binB = 1 |

| 20–28 | a felírt gyógyszer TTT kódja | 9 | 210002737 | 210002737 |

| 29–31 | a felírt gyógyszer mennyisége | 3 | 99 | 099 |

| 32–36 | orvos pecsétszáma | 5 | 112345 | 12345 |

| – |  | – | + „1” | → binC = 1 |

| 37–38 | szakorvosi javaslat dátuma (relatív módon) | 2 | 2006.01.30 | 12 |

| 39–41 | a Felügyelet által minősítéskor adott szám | 3 | 020 | 020 |

| 42–42 | törzs érvényességének kezdő hónapja (relatív módon) | 1 | 2006.12.01 | 2 |

| – | binA: BNO-kód 4. karaktere „H” | – | 1xx |  |

| – | binB: helyettesíthető | – | x1x |  |

| – | binC: pecsétszám 6 számjegyű, első karaktere „1” | – | xx1 |  |

| 43–43 | → binA, binB, binC decimális megfelelője | 1 | 111 | 7 |

## 4. Az „extra vonalkód” műszaki leírása: Code–128 jelkép MSZ EN 799:2001 számú szabvány 4.6 pontja alapján a jelkép méreteit és tűréseit az adott alkalmazási környezet határozza meg. A megfelelő leolvashatóság érdekében – figyelembe véve az olvashatóságot és a dekódolhatóságot – az X=0,33–0,495 mm közötti modulméret javasolt. Ugyancsak az alkalmazási környezet alapján a javasolt minimális vonalmagasság 12 mm (MSZ EN 799:2001 számú szabvány 4.6 pontja alapján). A jelkép előtt és mögött megjelenő világos nyugalmi mező X=0,33 mm esetén minimum 3,4 mm (MSZ EN 799:2001 számú szabvány 4.6.3.1 pontja alapján). A vonalkódba bekódolt adatok szemmel olvasható módon történő feltüntetése az adott alkalmazási környezetben tiltott.

## ”

2. számú melléklet a 46/2008. (XII. 3.) EüM rendelethez

„2. számú melléklet az 53/2007. (XII. 7.) EüM rendelethez

A gyógyszertörzs adatállományának leírása

1.1 VERZIOK Tábla

| Név | Leírás | Hivatkozás |

| KIHIRD | Életbelépés dátuma |  |

| VERZIO | Hányadik módosítás |

| TIPUS | 1: gyógyszer, alapanyag, 2: gyse, gyógyfürdő |

| STATUS | 1: javítás alatt, 2: lezárva |

| JAVAUTH | Utoljára javította |

| JAVDAT | Javítás dátuma |

| ID | egyedi azonosító |

1.2 GYOGYSZ Tábla

| Név | Leírás | Hivatkozás |

| ID | Elsődleges azonosító. |  |

| KOZHID | OGYI által kezelt, időben változatlan, egyedi termékazonosító. |  |

| OEP_DAT | Az érvényesség kezdetének (a hatálybalépésének) dátuma ééééhhnn formában. |  |

| SWITCH | A változás kódja: U: új termék, M: módosított, K: kikerül a támogatásból, T: törlendő, forgalomból kivonva. | 4. § (4) c); 4. § (4) d) |

| TIPUS | A készítmény típusának kategóriája: G: gyógyszer, T: tápszer, R: radiofarmakon, H: homeopátiás szer, A: alapanyag,, F: FoNo készítmény, C: csomagolóanyag, K: készítési díj, S: gyógyászati segédeszköz, F: gyógyfürdő. |  |

| OEP_TTT | A készítmény azonosítására az OEP által használt kód (TTT). | 2. § c); 4. § (5) aa) |

| OEP_EAN | A termék EAN kódja. |  |

| OEP_TK | A készítmény OGYI által kiadott nyilvántartási száma. | 2. § i); 4. § (5) ab) |

| TKTORLES | A nyilvántartásból törölt készítmények megjelölésére használt oszlop: TT vagy null. |  |

| TKTORLESDAT | A készítmény nyilvántartásból való törlésének dátuma. |  |

| OEP_NEV | A készítmény neve. | 4. § (5) ac) |

| OEP_KSZ | A készítmény kiszerelése. | 4. § (5) ad) |

| OEP_ATC | OEP által meghatározott ATC kód. | 4. § (5) ae) |

| HATOANYAG | A készítmény fő hatóanyagának neve. | 4. § (5) ae) |

| ADAGMOD | A készítmény adagolásmódjának azonosítója. |  |

| ID_GYFORMA | A gyógyszerforma azonosítója. |  |

| GYFORMA | A teljes gyógyszerforma szöveges leírása. |  |

| RENDELHET | A készítmény rendelhetőségének azonosítója: V: vényköteles gyógyszerek VN: vény nélküli gyógyszerek I: rendelőintézeti járóbeteg-szakellátást vagy fekvőbeteg-szakellátást nyújtó szolgáltatók által biztosított körülmények között alkalmazható gyógyszerek J: a szakorvosi/kórházi diagnózist követő járóbeteg-ellátásban alkalmazható gyógyszerek SZ: szakorvos által rendelhető gyógyszerek | 4. § (5) ah) |

| EGYENID | Az OGYI által megállapított egyenértékűség esetén az OEP által adott csoport azonosító száma, ha nincs ilyen, akkor –1. | 4. § (5) ai) |

| OHATO_MENNY | Összes hatóanyag tartalom. |  |

| HATO_MENNY | Egy kiszerelési egységben levő hatóanyag tartalom. |  |

| HATO_EGYS | OHATO_MENNY, HATO_MENNY mezők mennyiségi egysége (pl. mg). |  |

| KISZ_MENNY | A termékben levő kiszerelési egységek száma. |  |

| KISZ_EGYS | A termékben levő kiszerelési egység egységneve (pl. db). |  |

| DDD_MENNY | DDD értéke. | 2. § f) |

| DDD_EGYS | DDD_MENNY mennyiségi egysége (pl. mg). |  |

| DDD_FAKTOR | HATO_EGYS és DDD_EGYS közti átváltó szám (pl. g, mg esetén 1000). |  |

| DOT | Terápiás napok száma | 2. § g) |

| OEP_TAR | Termelői ár |  |

| OEP_NKAR | Nagykereskedelmi ár |  |

| OEP_FAN | Fogyasztói ár nettó |  |

| OEP_FAB | Fogyasztói ár bruttó | 4. § (5) af) |

| OEP_AFA | Áfa kulcsa |  |

| NTK | Napi terápiás költség | 2. § d); 4. § (5) af) |

| OEP_ITM | A termék régi támogatásjelzése |  |

| OEP_JC1 | Az oszlop „I” karaktert tartalmaz, ha a készítmény honvédelmi jogosultsággal írható. |  |

| OEP_JC2 | Az oszlop „I” karaktert tartalmaz, ha a készítmény közgyógyellátott betegeknek írható. |  |

| OEP_JC3 | Az oszlop „I” karaktert tartalmaz, ha a készítmény üzemi baleset esetén felírható. |  |

| OEP_JC4 | Az oszlop „I” karaktert tartalmaz, ha a készítmény EÜ kiemelt jogosultsággal írható. |  |

| OEP_JC5 | Az oszlop „I” karaktert tartalmaz, ha a készítmény EÜ emelt jogosultsággal írható. |  |

| KGYKERET | Az oszlop 1-et tartalmaz, ha a készítmény közgyógy keretre elszámolható, 2-t ha nem. | 4. § (5) ca); 4. § (5) cb) |

| EGYSEGAR | HATO_EGYS-nyi hatóanyag ára. |  |

| NORM_TIP | Értékei: NT, nem támogatott és NOMIN, HFIX, TFX a normatív támogatás technikája. |  |

| NORM_SZAZ | Támogatás mértéke%-ban (pl. 0, 25, 55, 85) | 4. § (5) ag) |

| NORM_FIXID | Normatív fixcsoport azonosítója | 4. § (5) d) |

| NORM_REFNTK | Normatív fixcsoport referencia NTK-ja |  |

| OEP_INN | Normatív támogatás nettó |  |

| OEP_INB | Normatív támogatás bruttó | 4. § (5) ag) |

| NORM_TERDIJ | A beteg által térítendő összeg (normatív) | 2. § e) |

| NTK_TD | A beteg által térítendő összeg szerint kiszámított napi terápiás költség (normatív) | 2. § f) |

| NORM_MIHAID | Minőségi és Hatékony Gyógyszerrendelési Ösztönzés csoportazonosítója: 0: nem értelmezett; 1: Gyomorbántalmak, GERD; 2: Magas vérnyomás; 3: Vérzsíreltérések (magas koleszterin, triglicerid); 4: Cukorbetegség |  |

| NORM_MIHACEL | Minőségi és Hatékony Gyógyszerrendelési Ösztönzés a gyógyszer csoportjához tartozó célérték. |  |

| NORM_MIHASTAT | Minőségi és Hatékony Gyógyszerrendelési Ösztönzés status –1: célérték alatti vagy azonos; 0: nem értelmezett; 1: célérték fölött van | 4. § (5) e) |

| EUEM_TIP | Értékei: (null), NOMIN, HFIX, TFX, az EÜ emelt támogatás technikája |  |

| EUEM_SZAZ | Támogatás mértéke%-ban (pl. 50, 70, 90) | 4. § (5) ag) |

| EUEM_FIXID | EÜ emelt fixcsoport azonosítója | 4. § (5) d) |

| EUEM_REFNTK | EÜ emelt fixcsoport referencia NTK-ja |  |

| OEP_EUN | EÜ emelt támogatás nettó |  |

| OEP_EUB | EÜ emelt támogatás bruttó | 4. § (5) ag) |

| EUEM_TERDIJ | A beteg által térítendő összeg (EÜ emelt) | 2. § e) |

| NTK_EETD | A beteg által térítendő összeg szerint kiszámított napi terápiás költség (EÜ emelt) | 2. § f) |

| EUEM_PONTOK | EÜ pontok, amire a termék EÜ emelt támogatással írható |  |

| EUKIEM_TIP | Értékei: (null), NOMIN, HFIX, TFX, az EÜ kiemelt támogatás technikája |  |

| EUKIEM_SZAZ | Támogatás mértéke%-ban (pl. 100) | 4. § (5) ag) |

| EUKIEM_FIXID | EÜ kiemelt fixcsoport azonosítója | 4. § (5) d) |

| EUKIEM_REFNTK | EÜ kiemelt fixcsoport referencia NTK-ja |  |

| OEP_EU100N | EÜ kiemelt támogatás nettó |  |

| OEP_EU100B | EÜ kiemelt támogatás bruttó | 4. § (5) ag) |

| EUKIEM_TERDIJ | A beteg által térítendő összeg (EÜ kiemelt) | 2. § e) |

| NTK_EKTD | A beteg által térítendő összeg szerint kiszámított napi terápiás költség (EÜ kiemelt) | 2. § f) |

| EUKIEM_PONTOK | EÜ pontok, amire a termék EÜ kiemelt támogatással írható. |  |

| FORGALOMBAN | Ha forgalmazott termék, akkor 1, egyébként (null). |  |

| BESOROLAS | A költséghatékonysági kategória kódja jogcímenként (lásd megjegyzések). | 4. § (5) aj) |

| PATIKA | GYSE Patikában kapható-e (I) |  |

| KIHI | Kihordási idő |  |

| FELME | Felírható mennyiség |  |

| EGYEDI | Egyedi méretvétel alapján (I) |  |

| OEP_ISO | ISO kód |  |

| FORGENGT | Forgalomba hozatali engedély jogosultja |  |

| FORGENGT_ID | Forgalomba hozatali engedély jogosultjának azonosítója |  |

| FORGALMAZ | Forgalmazó |  |

| FORGALMAZ_ID | Forgalmazó azonosítója |  |

| BRANDNEV | A gyógyszercsalád (brand) neve |  |

| BRAND_ID | A gyógyszercsalád (brand) azonosítója |  |

| KERESZTJELZES | OGYI hatáserősség (méregosztály) jelzése pl. +, ++, ... stb. |  |

| VEGE | Az érvényesség vége, ha még nincs lezárva az érvényessége, akkor 2099.12.31 (Access, DBF fájlokban nem jelenik meg, mert felesleges). |  |

| REGI_NEV | Az átnevezett készítmény korábbi neve. |  |

1.2.1 GYOGYSZ táblához tartozó megjegyzések

A gyógyszer-hatékonysági színezés alapjául szolgáló

BESOROLAS mező kitöltésének kódjai:

1: referencia termék,

2: NTK <= REFNTK

3: NTK < 1,1 * REFNTK

4: NTK >= 1,1 * REFNTK

5: nem képezhető

6: TT

A normatív jogcímhez képzett kód: njk.

Az EÜ emelt jogcímhez képzett kód: eejk.

Az EÜ kiemelt jogcímhez képzett kód: ekjk.

BESOROLAS = 10000 * njk + 100 * eejk + ekjk

1.3 SZAKVKODOK Tábla

| Név | Leírás | Hivatkozás |

| ID KOD LEIRAS | Elsődleges azonosító A szakvizsga kódja A szakvizsga leírása | 4. § (5) ga) |

1.4 SZAKVHOZZAR Tábla

| Név | Leírás | Hivatkozás |

| EUPONT_ID SZAKV_ID | Az EÜ pont azonosítója Szakvizsgák, amikkel írható a ponton levő gyógyszer. |  |

1.5 EUPONTOK Tábla

| Név | Leírás | Hivatkozás |

| ID EUTIP KODSZAM PERJEL LEIRAS JAVASLATRA JIDOKORLAT | Elsődleges azonosító Értékei: EÜ50, EÜ70, EÜ90, EÜ100. Az indikáció kódja, ha pl.: 3/c, 9/a, akkor ebből a szám. Az indikáció perjel utáni része pl. c, b2. Az indikáció leírása 0: ha javaslatra nem írható, 1: ha igen. A javaslattól kezdve hány hónapig írható. |  |

| 4. § (5) f) |

1.6 EUHOZZAR Tábla

| Név | Leírás | Hivatkozás |

| EUPONT_ID GYOGYSZ_ID | Hivatkozás Hivatkozás |  |

1.7 BNOKODOK Tábla

| Név | Leírás | Hivatkozás |

| ID KOD LEIRAS | Elsődleges azonosító A BNO kódja, 5 vagy kevesebb hosszúságú, pl. C90, C90000. BNO leírása | 4. § (5) f) |

1.8 BNOHOZZAR Tábla

| Név | Leírás | Hivatkozás |

| EUPONT_ID BNO_ID | Hivatkozás Hivatkozás |  |

1.9 KIINTOR Tábla

| Név | Leírás | Hivatkozás |

| ID JAROFEKVO MEGYE INTKOD INTEZET GYFKOD EGYSEG ORVOSNEV PECSETKOD | Elsődleges azonosító J: járó-, F: fekvőbeteg intézmény Megye Az intézet kódja Intézet neve GYF kód Intézeten belüli egység (osztály, szakambulancia,...) neve A jogosult orvos neve A jogosult orvos pecsétkódja | 4. § (5) gb) |

1.10 KIINTHOZZAR Tábla

| Név | Leírás | Hivatkozás |

| EUPONT_ID KIINT_ID | Az EÜ pont azonosítója A kijelölt intézetre (és orvosra) mutat. |  |

2. Táblahivatkozások

2.1 Szülő-gyerek kulcsok

| Szülő | Oszlop | Gyerek | Hivatkozó oszlop |

| EUPONTOK EUPONTOK BNOKODOK GYOGYSZ EUPONTOK SZAKVKODOK EUPONTOK KIINTOR | ID ID ID ID ID ID ID ID | EUHOZZAR BNOHOZZAR BNOHOZZAR EUHOZZAR SZAKVHOZZAR SZAKVHOZZAR KIINTHOZZAR KIINTHOZZAR | EUPONT_ID EUPONT_ID BNO_ID GYOGYSZ_ID EUPONT_ID SZAKV_ID EUPONT_ID KIINT_ID |

”
