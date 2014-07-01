2. számú melléklet az 53/2007. (XII. 7.) EüM rendelethez[^47]

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

| KOZHID | A GYEMSZI által kezelt, időben változatlan, egyedi termékazonosító. |  |

| OEP_DAT | Az érvényesség kezdetének (a hatálybalépésének) dátuma ééééhhnn formában. |  |

| SWITCH | A változás kódja: U: új termék, M: módosított, K: kikerül a támogatásból, T: törlendő, forgalomból kivonva. | 4. § (4) c); 4. § (4) d) |

| TIPUS | A készítmény típusának kategóriája: G: gyógyszer, T: tápszer, R: radiofarmakon, H: homeopátiás szer, A: alapanyag,, F: FoNo készítmény, C: csomagolóanyag, K: készítési díj, S: gyógyászati segédeszköz, F: gyógyfürdő. |  |

| OEP_TTT | A készítmény azonosítására az OEP által használt kód (TTT). | 2. § c); 4. § (5) aa) |

| OEP_EAN | A termék EAN kódja. |  |

| OEP_TK | A készítmény GYEMSZI által kiadott nyilvántartási száma. | 2. § i); 4. § (5) ab) |

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

| EGYENID | A GYEMSZI által megállapított egyenértékűség esetén az OEP által adott csoport azonosító száma, ha nincs ilyen, akkor –1. | 4. § (5) ai) |

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

| KERESZTJELZES | A GYEMSZI hatáserősség (méregosztály) jelzése pl. +, ++, ... stb. |  |

| VEGE | Az érvényesség vége, ha még nincs lezárva az érvényessége, akkor 2099.12.31 (Access, DBF fájlokban nem jelenik meg, mert felesleges). |  |

| REGI_NEV | Az átnevezett készítmény korábbi neve. |  |

1.2.1 GYOGYSZ táblához tartozó megjegyzések

A gyógyszer-hatékonysági színezés alapjául szolgáló BESOROLAS mező kitöltésének kódjai:

1: referencia termék

2: PRAS csoport (fix csoport, ahol preferált referenciaársáv képződött) esetében: PRAS termék, egyébként NTK <= REFNTK

3: PRAS csoport esetében NTK > 1,15 *REFNTK ÉS NTK < 1,2 *REFNTK, egyébként NTK < 1,2 *REFNTK

4: NTK >= 1,2 *REFNTK

5: nem képezhető

6: TT (törzskönyvből törölt)

7: PRAS körbe tartozó, PRAS-on kívüli termékek, amelyek utólag a preferált referencia ársáv szintjére csökkentették árukat

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

[^47]: A 2. számú mellékletet a 46/2008. (XII. 3.) EüM rendelet 5. § (2) bekezdése iktatta be, szövege a 41/2014. (VI. 30.) EMMI rendelet 18. §-a szerint módosított szöveg.
