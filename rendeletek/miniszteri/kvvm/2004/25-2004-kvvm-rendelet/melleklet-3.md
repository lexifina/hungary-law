## Közúti közlekedés zajkibocsátásának számítása

## 1. Fogalommeghatározások

## 1.1 Vonatkoztatási egyenértékű A-hangnyomásszint LAeq(7,5), dB

## Akadálytalan hangterjedés estén a vonatkoztatási távolságban, a terepszint felett 1,2 m magasságban, e melléklet szerint számított egyenértékű A-hangnyomásszint.

## 1.2 Számított egyenértékű A-hangnyomásszint LAeq(d,h), dB

## A számítási (észlelési, megítélési, terhelési) pontban e melléklet szerint számított eredő A-hangnyomásszint

## 1.3 Egyidejűség (szinkronitás)

## Feltétel, amely szerint az 1.4 és az 1.5 pontok szerinti egyenértékű A-hangnyomásszintek vonatkoztatási időtartama(i) egymás között egyenlő(ek), és a számításhoz felhasznált, az egyes akusztikai járműkategóriákhoz, valamint a kötöttpályás közlekedéshez tartozó forgalomnagyság ehhez (ezekhez) a vonatkoztatási időtartam(ok)hoz tartozik (tartoznak).

## 1.4 Évi átlagos napi forgalom ÁNF, j/nap

## A hivatalos keresztmetszeti forgalomszámlálás szerint a vizsgált útvonalszakaszra vonatkozó, j/nap-ban megadott forgalomnagyság (amely az út keresztmetszetén áthaladó napi forgalom éves átlaga), járműkategóriánkénti bontásban.

## A keresztmetszeti forgalomszámlálási adatokat az Országos Közúti Adatbank (OKA-ÁKMI) adja közre. Az ÁNF-adathoz hozzátartozik, és a számítás eredményeinek felhasználásával készített dokumentációban fel kell tüntetni a számlálóállomás kódját.

## 1.5 Akusztikai járműkategória

## A keresztmetszeti forgalomszámlálás adataiból a 4. pont szerinti összevonással meghatározott három járműkategória.

## A továbbiakban a három akusztikai járműkategória jele: I., II., III. Az ”i”-edik akusztikai járműkategóriához tartozó adatot az ”i” alsó index jelöli.

## 1.6 Az egyes akusztikai járműkategóriákhoz tartozó évi átlagos forgalomnagyság

## A keresztmetszeti forgalomszámlálás során alkalmazott járműkategóriákhoz tartozó évi átlagos napi forgalomnagyságból a 4. pont szerinti összegzéssel, akusztikai járműkategóriákra meghatározott mennyiség.

## 1.7 Az egyes akusztikai járműkategóriákhoz tartozó évi átlagos forgalomnagyság adott vonatkoztatási időre

## Az egyes akusztikai járműkategóriákhoz tartozó járművek évi átlagos napi forgalmi adatából képzett, az adott vonatkoztatási időhöz tartozó összforgalom.

## 1.8 Adott vonatkoztatási időhöz tartozó évi átlagos óraforgalom Qix j/óra

## Az egyes akusztikai járműkategóriákhoz és Tx óra vonatkoztatási időtartamhoz tartozó évi átlagos napi forgalomnagyság (ÁNF) 1/Tx-ed része.

## x az adott vonatkoztatási időre utaló jelölés, amit a felhasználó alkalmilag határoz meg.

## Általában

## „nappal” x = nappal és Tnappal = 16 óra

## „napközben” x = napköz és Tnapköz = 12 óra

## „este” x = este és Teste = 4 óra

## „éjszaka” x = éjjel és Téjjel = 8 óra.

## 1.9 Vonatkoztatási távolság dref, m

## A közút, ill. a vágány akusztikai tengelyétől mért 7,5 m távolság, azaz dref = 7,5 m.

## 1.10 Látószög β, fok

## Egy útszakasznak a raszterhálópontban vett látószöge. Az útszakasz látószögétől függő korrekciót a 7. számú melléklet 9. pontja szerint kell számolni.

## 1.11 Útszakasz (szakasz):

## a) Általában

## aa) közút esetén az út akusztikai középvonalának azon szakasza, amelyen belül mindegyik akusztikai járműkategóriára nézve a forgalomnagyság, a mértékadó sebesség, továbbá az útburkolat fajtája és a hosszesés mértéke állandó, valamint az ”útszakasz”-hoz tartozó látószög által meghatározott tartományon belül a terjedés feltételei azonosak (azonos kialakítású, úthoz képesti helyzetű zajárnyékoló fal, azonos hangelnyelő-tulajdonságú terep).

## ab) városi kötöttpályás jármű (villamos) esetén a vágány akusztikai középvonalának azon szakasza, amelyen belül mindegyik kötöttpályás járműkategóriára nézve a forgalomnagyság, továbbá a vágányrendszer állandó. valamint az ”útszakasz”-hoz tartozó látószög által meghatározott tartományon belül a terjedés feltételei azonosak (azonos kialakítású, úthoz képesti helyzetű zajárnyékoló fal, azonos hangelnyelő-tulajdonságú terep).

## b) Ha a számítás kiindulási adata az éves átlagos napi forgalomnagyság

## (azaz ÁNF adott járműkategóriánként, napszakonként a 4. pont szerint), akkor

## ba) közút esetén a közútnak az a szakasza, amelyre a számításba vett ÁNF-adat vonatkozik, az útburkolat fajtája, a hatóságilag engedélyezett haladási sebesség és a lejtés állandó, valamint az ”útszakasz”-hoz tartozó látószög által meghatározott tartományon belül a terjedés feltételei azonosak (azonos kialakítású, úthoz képesti helyzetű zajárnyékoló fal, azonos hangelnyelő-tulajdonságú terep)

## bb) városi kötöttpályás jármű (villamos) esetén az ab)-vel azonos.

## - Az a) esetben

## szintbeni kereszteződést egy adott számítási útszakaszra vonatkozóan két olyan egymást követő útszakasszal kell figyelembe venni , amelynek az egyik határa az adott forgalmi irányra vonatkozó stopvonal, illetve stopvonal hiányában a kereszteződés belátását már lehetővé tevő keresztmetszet;

## a körforgalmat egy adott számítási útszakaszra vonatkozóan két olyan egymást követő útszakasszal kell figyelembe venni, amelynek az egyik határa az adott forgalmi irányra vonatkozó stopvonal, illetve a kereszteződés belátását már lehetővé tevő keresztmetszet. A körforgalomban mindig több számítási vagy teljes útszakasz találkozik. Ezek mindegyikéhez található olyan útszakasz, amelyik a megfelelő belépő keresztmetszettől indulva és a körgyűrű egy részén áthaladva valamelyik ágon kilép a csomópontból. A körgyűrű forgalmát tehát külön nem kell figyelembe venni, az a fentiek szerint adódik.

## - A b) esetben a kereszteződés és a körforgalom hatása nem vehető figyelembe.

## - A j-edik útszakaszhoz rendelt adatok jelölése ”j” alsó index és összesen ”n” darab útszakaszból áll a számítási vagy a teljes útszakaszámú

## 1.12 Számítási- vagy teljes útszakasz

## A számítás során figyelembe vett közútnak, illetve vágánynak az adott akusztikai középvonalát felépítő ”n” darab egymáshoz fűzött szakasza.

## - Az adott megítélési pont zajterhelését egynél több ilyen számítási útszakasz is meghatározhatja (így például: széles út, párhuzamosan futó utak, vágányok, egymást keresztező utak, vágányok).

## - Az s-edik számítási útszakaszhoz rendelt adat jelölése ”s” alsó index és összesen ”r” darab számítási útszakasz – azaz figyelembe veendő akusztikai középvonal – van.

## 1.13 Végtelen hosszú, egyenes vonalforrás

## Ha a számítási útszakasz akusztikai középvonala az 1. ábrán feltüntetett távolságarányokkal meghatározott tartományon belül helyezkedik el, akkor a számítási útszakasz végtelen hosszú egyenes vonalforrásnak tekinthető.

## 1.14 Akusztikai középvonal

## Az útburkolat, illetve a sínkorona szintje fölött 0.5 m magasan

## a) közút esetén

## aa) irányonként egy forgalmi sávnál az út geometriai tengelyében,

## ab) irányonként kettő, vagy kettőnél több forgalmi sávnál az egyes forgalmi irányokhoz tartozó forgalmi sávok összefüggő burkolt felületének a geometriai középvonalában;

## b) városi villamos- és HÉV-vágány esetén a vágány geometriai középvonalában

## húzódó végtelen hosszú egyenes vonalforrás.

## 1.15 Szétosztott forgalom

## a) közút esetén

## aa) irányonként egy forgalmi sávnál a számításba vett teljes forgalom,

## ab) irányonként kettő, vagy kettőnél több forgalmi sávnál a számításba vett teljes forgalomnagyság irányonként és akusztikai járműkategóriánként 50-50 %-ban megosztott mennyisége, illetve az irányonkénti és akusztikai járműkategóriánkénti forgalomnagyság (ha ismert);

## ab) városi kötöttpályás közlekedés esetén kötöttpályás járműkategóriánként és vágányonként ismert forgalom.

## 1.16 Mértékadó sebesség v, km/óra

## Az egyes akusztikai járműkategóriáknak a számításhoz alapul vett forgalomnagyságához tartozó sebesség.

## - Gyorsuló, illetve lassuló forgalom esetén az útszakasz határait úgy kell megállapítani, hogy az így kijelölt útszakaszon a járművek gyorsulása, illetve lassulása állandó legyen. Ekkor a mértékadó sebesség az útszakaszon várható (kialakuló) legkisebb és legnagyobb járműsebesség számtani átlaga.

## - Ha a számítás kiindulási adata az éves átlagos napi forgalomnagyság (ÁNF járműkategóriánként, napszakonként, a 4. pont szerint), akkor mértékadó sebességnek minden járműkategóriában az adott út- és időszakaszra érvényes, hatóságilag engedélyezett, illetve előírt vmegengedett legnagyobb (esetenként legkisebb) haladási sebesség korrigált értéke alkalmazandó, és a forgalmat egyenletesen áramlónak kell tekinteni.

## A korrigált sebesség:

## Adott „x” vonatkoztatási időre:

## ahol

## A = 0,07 vmegengedett + 20

## Qsáv,x = (Q1x + Q2x + Q3x) / FS

## és

## Q1x, Q2x, Q3x a 4.1.2 pont szerint

## FS a forgalmi sávok összes száma, ahol a forgalom lebonyolódik

## - Kötöttpályás közlekedés esetén

## villamosnál v = 40 km/óra

## HÉV-nél v = 60 km/óra

## 1.17 Időszakasz, 1 órás időszakasz:

## Időtartam, amelyben a közút, illetve a vágány akusztikai középvonalának adott szakaszán mindegyik akusztikai- és kötöttpályás járműkategóriára nézve a forgalomnagyság és a mértékadó sebesség állandó.

## - A leghosszabb figyelembe vehető időszakasz 1 óra tartamú (ekkor f = 1, a jelöléseknél). A megítélési időben tehát, például a nappali időszakban legalább 16 db, az éjszakai időszakban pedig legalább 8 db időszakasz van.

## - A t-edik időszakaszhoz rendelt adatok jelölése ”t” alsó index és összesen ”f” darab ”Tt” másodpercben megadott időszakaszból szakaszból tevődik össze 1 óra. A megítélési időtartam összesen ”u” darab ”Tg” = 1 órás időszakaszból tevődik össze.

## 1.18 A kopóréteg akusztikai érdességi kategóriája

## A kopórétegnek a forgalom zajhatását jelentősen befolyásoló érdessége és hangelnyelő tulajdonsága.

## A számítási eljárásban a kopóréteget az ”A”-”E” kategóriák valamelyikébe soroljuk. A számítási modell az ”A”-tipusú kopórétegen lebonyolódó forgalomra vonatkozik, így a burkolatra vonatkozó korrekció az ”A”-akusztikai érdességi kategóriába tartozó kopórétegen lebonyolódó forgalom esetén nulla.

## 2. A számítás alkalmazhatósága

## 2.1 A számítás akkor alkalmazható, ha

## a) a számítási útszakasz (akár közúti, akár kötöttpályás) végtelen hosszúságú egyenes vonalforrásnak tekinthető, és

## b) a számítási útszakaszon belül meghatározott útszakaszokra, mindhárom akusztikai járműkategóriára érvényes a következő:

## Q/v < 43

## ahol

## Q jármű/óra az adott akusztikai járműkategóriához tartozó forgalomnagyság;

## v km/óra az adott akusztikai járműkategóriához rendelt mértékadó sebesség.

## 2.2 A számítás a közúti forgalomból (beleértve a városi kötöttpályás közlekedést is) adódó, az észlelési pontra vonatkozó egyenértékű A-hangnyomásszintet adja eredményül. A számítás a mértékadó sebesség 20-130 km/óra közötti tartományában, a forgalomnagyságnak a gyakorlatban megvalósuló minden értékére elvégezhető.

## 2.3 A számítás során a rendelkezésre álló forgalmi adatok (Q és v) térbeli és időbeli felbontásához illeszkedő módon alkalmazni kell a szakaszokra bontás módszerét.

## 2.4 Ha a számítás kiindulási adata az éves átlagos napi forgalomnagyság (ÁNF járműkategóriánként, napszakonként, a 4. pont szerint), akkor nem lehetséges figyelembe venni a kereszteződés hatását, vagy a forgalom napi menete hatását, mivel nem lehet a kiindulási adatnál finomabb út- és időszakasz-felbontást alkalmazni. Az útszakasz ilyenkor jellemzően az ÁNF-adat érvényességi szakasza által van adva, az időszakasz pedig 1 óra. A számítás közbülső eredményeként adódó, (napszakonként) 1 órás időtartamra vonatkozó egyenértékű A-hangnyomásszint egyben a kérdéses napszakra vonatkozó megítélési időre is érvényes lesz, mivel az ÁNF-adat jelen előírás szerinti alkalmazásában az adott napszak (napközben, este, éjjel) minden egyes órájához azonos forgalomnagyság tartozik.

## 3. A számítás menete

## 3.1 Általános előírások

## 3.1.1 A számítás során figyelembe kell venni az összes olyan közutat és villamos vágányt, amelynek a forgalma befolyásolhatja a végeredményt.

## 3.1.2 Az egyes közút(ak), vágány(ok)) számítási szakaszát(szakaszait) meghatározva el kell végezni a közút(ak) (vágány(ok)) összes akusztikai középvonalának a szakaszokra bontását.

## 3.1.3 Ha a felhasznált forgalmi adatok időfüggése indokolja, akkor el kell végezni az egyes érintett útszakaszokra nézve az időszakaszokra bontást is (például, ha kereszteződés hatását kívánjuk figyelembe venni). A szakaszokra bontást a szakaszok fogalmának meghatározásánál ismertetett feltételek megtartásával kell elvégezni.

## 3.1.4 Az út- és időszakaszokra egyenként kell meghatározni a megítélési pontban számított egyenértékű A-hangnyomásszinteket. A számítási eljárás mindegyik út- és időszakaszra nézve azonos. A meghatározott adatokból az eredő zajszintet több lépcsőben kell képezni, a következők szerint.

## 3.2 A g-edik 1 órás időtartamra vonatkozó számított egyenértékű A-hangnyomásszint meghatározása

## A g-edik 1 órás időtartamra vonatkozó számított egyenértékű A-hangnyomásszint meghatározása az alábbi pontok alapján történik.

## 3.2.1 A t-edik időszakaszra és j-edik útszakaszra vonatkozó egyenértékű A-hangnyomásszint meghatározása

## 3.2.1.1 Az egyes útszakaszokhoz tartozó vonatkoztatási egyenértékű A-hangnyomásszintet a vonatkoztatási távolságban [a g-edik órán belül, az s-edik számítási útszakaszhoz tartozó, j-edik út- és t-edik időszakasz esetén az LAeq(7,5)g,s,t,j mennyiséget] az útszakaszra megállapított (Q és v) forgalmi adatokból kell meghatározni a 4. pont szerint.

## Ha a zajszámító programban kiinduló adatként a 25 m-es egyenértékű A-hangnyomásszintet alkalmazzák, akkor azt az LAeq(7,5)g,s,t,j mennyiségből a következő összefüggéssel kell számítani:

## 3.2.1.2 Adott számítási pontban az egyes útszakaszokhoz tartozó számított egyenértékű A-hangnyomásszintet [a g-edik órán belül, az s-edik számítási útszakaszhoz tartozó, j-edik út- és t-edik időszakasz esetén az LAeq(d,h)g,s,t,j mennyiséget] az útszakaszra már kiszámított LAeq(7,5)g,s,t,j vonatkoztatási egyenértékű A-hangnyomásszintből a 7. számú melléklet szerinti zajterjedés-számítással kell meghatározni.

## 3.2.2 Az s-edik számítási útszakaszhoz tartozó, t-edik időszakaszra vonatkozó eredő számított egyenértékű A-hangnyomásszint

## A g-edik órán belül, az s-edik számítási útszakaszhoz és a t-edik időszakaszhoz tartozó eredő számított egyenértékű A-hangnyomásszintet a számítási pontban a következő összefüggéssel kell meghatározni (összesen n darab szakasz van):

## 3.2.3 Az s-edik számítási útszakaszhoz tartozó, 1 órás időtartamra vonatkozó eredő számított egyenértékű A-hangnyomásszint

## A g-edik órán belül, az s-edik számítási útszakaszhoz és az összes időszakaszhoz tartozó eredő számított egyenértékű A-hangnyomásszintet a számítási pontban a következő összefüggéssel kell meghatározni (összesen f darab Tt másodperc időtartamú időszakasz van):

## 3.2.4 Az összes számítási útszakaszhoz tartozó, 1 órás időtartamra vonatkozó eredő számított egyenértékű A-hangnyomásszint

## A g-edik órán belül, az összes számítási útszakaszhoz és az összes időszakaszhoz tartozó eredő számított egyenértékű A-hangnyomásszintet a számítási pontban a következő összefüggéssel kell meghatározni (összesen r darab számítási útszakasz van):

## 3.3 A megítélési időtartamra vonatkozó számított egyenértékű A-hangnyomásszint meghatározása

## A megítélési időtartamra vonatkozóan az összes számítási útszakaszhoz és az összes 1órás időszakaszhoz tartozó eredő számított egyenértékű A-hangnyomásszintet a számítási pontban a következő összefüggéssel kell meghatározni (összesen u darab 1 órás időszakasz van):

| LAeq(d,h)nappal esetén | u = 16 |

| LAeq(d,h)éjjel esetén | u = 8 |

| LAeq(d,h)napköz esetén | u = 12 |

| LAeq(d,h)este esetén | u = 4 |

## 3.4 Az indexek elhagyhatósága

| Ha |  | akkor |  |

|  | – a nappali/éjszakai/napközbeni/esti megítélési idők minden órájában azonos forgalomnagysággal számolunk |  | u=1 |

|  | – egyetlen számítási útszakasszal kell számolni |  | r=1 |

|  | – az aktuális, s-edik számítási útszakaszon az aktuális, g-edik órán belül a forgalom időfüggésével nem számolunk |  | f=1 |

|  | – az aktuális, s-edik számítási útszakaszon az aktuális, g-edik órán belül a forgalmi jellemzők, az útburkolat, az emelkedési viszonyok, a vágány tipusa, a kötöttpályás forgalom, a terjedést befolyásoló tényezők (például végig van/nincs zajárnyékoló fal stb.) a teljes számítási útszakaszon egyaránt állandóak |  | n=1 |

## 3.5 A hosszútáv, nagytáv forgalmának figyelembevétele

## Az 5. pont szerint (ha szükséges).

## 4. Az egyes útszakaszokhoz tartozó zajszint számítása

## 4.1 A forgalmi adatokra vonatkozó feltételek

## 4.1.1 Az alkalmazott forgalmi adatok feleljenek meg az egyidejűség (szinkronitás) követelményének (1.8 pont).

## 4.1.2 A számítás alapját képező forgalmi adatok

## a) közúti forgalom esetén a 4.3 pont szerint képzett forgalmi adat és az 1.16 pont szerinti mértékadó sebességadat;

## b) városi kötöttpályás közlekedés esetén a figyelembe vehető járműtípusok (jelölés: ”v” alsó index) és forgalmi irányok (vágányok) szerinti forgalmi adat, a vágánytípussal együtt. Sebesség az 1.16 pont szerint.

## 4.1.3 A számításnál az 1. táblázat szerinti kötöttpályás járműtípusok vehetők figyelembe.

## 1. táblázat

## Kötöttpályás járműtípus

| Jelölés v = | Rövidítés | Leírás |

| 1 | ICS1 | Ganz Ipari csuklós x 1 (kocsi) |

| 2 | ICS2 | Ganz Ipari csuklós x 2 (szerelvény) |

| 3 | UVMM | UV(MM) (2 motorkocsiból álló szerelvény) |

| 4 | UVMPM | UV(MpM) (2 motorkocsiból és közöttük 1 pótkocsiból álló szerelvény) |

| 5 | T5C5 | TATRA T5C5 szerelvény |

| 6 | TW 6000 | Hannoverből beszerzett szerelvény (2001-től) |

| 7 | MXA+P+MXA | HÉV |

| 8 | 2x(MXA+P+MXA) | HÉV (dupla szerelvény) |

## Az 1. táblázatban nem szereplő kötöttpályás járműtípusok esetén a térképet készítő szakértő megítélése szerint a táblázat megfelelő „v” jelű sora használható, más esetekben a számításokhoz szükséges 7. táblázat szerinti Cvk állandókat méréssel kell meghatározni.

## 4.2 A forgalmi járműkategóriák összevonása akusztikai járműkategóriákká

## Az I-II. és III. jelű akusztikai járműkategóriákba a 2. táblázat szerinti, az ÚT 2-1.109 Útügyi előírásban meghatározott járművek tartoznak (Jelölésük: ”k” alsó index).

## 2. táblázat

## Akusztikai járműkategóriák meghatározása

| Jelölés: k= | Járműkategória megnevezése (ÚT 2-1.109) | Akusztikai járműkategória | Járművek főbb jellemzői | Jel |

| 1. | személy- és kistehergépkocsi | I. | személygépkocsi vontatmánnyal, vagy anélkül, kis autóbusz 16 férőhely alatt, tehergépkocsi, amelynek megengedett legnagyobb össztömege kisebb 3500 kg-nál (kb. 1500 kg-nál kisebb hasznos teherbírású) | szgk |

| 2. | szóló autóbusz | II. | KRESZ szerint meghatározott (kivéve a 16 férőhely alattiakat) | busz |

| 3. | csuklós autóbusz | III. | KRESZ szerint meghatározott | cs-busz |

| 4. | könnyű tehergépkocsi | II. | tehergépkocsi, 3500-7000 kg össztömegű (kb. 1500-3000 kg hasznos teherbírású) | ktgk |

| 5. | szóló nehéz tehergépkocsi | III. | tehergépkocsi pótkocsi, vagy vontatmány nélkül, 7000 kg-nál nagyobb össztömegű (kb. 30000 kg-nál nagyobb hasznos teherbírású) | ntgk |

| 6. | tehergépkocsi szerelvény | III. | tehergépkocsi pótkocsival, nyergesvontató | tgk-szer |

| 7. | motorkerékpár és segéd-motoros kerékpár | II. | KRESZ szerint meghatározott | mkp |

## 4.3 Forgalmi adatok képzése a mértékadó zajterhelés számításához

## A mértékadó zajterhelés számításának alapját képező, adott vonatkoztatási időhöz tartozó óraforgalmat közúti közlekedés esetén a következők szerint kell megállapítani:

## 4.3.1 Az egyes akusztikai járműkategóriákhoz tartozó, a napközben napszakra vonatkozó évi átlagos óraforgalom Qi,napköz

## Q1,napköz = A1,napköz * ÁNF1/12

## Q2,napköz = A2,napköz * (ÁNF2+ ÁNF4+ ÁNF7)/12

## Q3,napköz = A3,napköz * (ÁNF3+ ÁNF5+ ÁNF6)/12

## 4.3.1.2 Az egyes akusztikai járműkategóriákhoz tartozó, az este napszakra vonatkozó évi átlagos óraforgalom Qi,este

## Q1,este = A1,este * ÁNF1/4

## Q2,este = A2,este * ( ÁNF2+ ÁNF4+ ÁNF7)/4

## Q3,este = A3,este * (ÁNF3+ ÁNF5+ ÁNF6)/4

## 4.3.1.3 Az egyes akusztikai járműkategóriákhoz tartozó, az éjszaka napszakra vonatkozó évi átlagos óraforgalom Qi,éjjel

## Q1,éjjel = A1,éjjel * ÁNF1/8

## Q2,éjjel = A2,éjjel * (ÁNF2+ ÁNF4+ ÁNF7)/8

## Q3,éjjel = A3,éjjel * (ÁNF3+ ÁNF5+ ÁNF6)/8

## 4.3.1.4 A 4.3.1.1 – 4.3.1.3 pontok szerinti összefüggésekben:

## ÁNFk = a k-adik járműkategória (4.2 pont) ÁNF-adata, jármű/nap

## Az ”Ai,napköz”, ”Ai,este” és „Ai,éjjel” tényezők a 3.táblázat szerint.

## 3. táblázat

## Napszak forgalom aránya (Ai,x) az ÁNF-hez képest

| Út-/ forgalomjelleg kategória* | Napszak forgalom aránya (Ai,x) az ÁNF-hez képest |

| Napközben 06-18 óra | Este 18-22 óra | Éjszaka 22-06 óra |

| Akusztikai járműkategória jele |

| I. | II. | III. | I. | II. | III. | I. | II. | III. |

| i=1 | i=2 | i=3 | i=1 | i=2 | i=3 | i=1 | i=2 | i=3 |

| M1, M5 autópályák M0-n kívüli szakaszai | 0,699 | 0,618 | 0,590 | 0,164 | 0,162 | 0,160 | 0,137 | 0,220 | 0,250 |

| M0 és az M3, M7 autópályák M0-n kívüli szakaszai | 0,745 | 0,660 | 0,612 | 0,162 | 0,160 | 0,158 | 0,093 | 0,180 | 0,230 |

| M0-n belüli autópálya szakaszok | 0,765 | 0,747 | 0,743 | 0,150 | 0,148 | 0,145 | 0,085 | 0,105 | 0,112 |

| Jelleg2=1 (Nagyarányú nemzetközi forgalmat lebonyolító főutak) | 0,750 | 0,743 | 0,736 | 0,162 | 0,160 | 0,158 | 0,088 | 0,097 | 0,106 |

| Jelleg2=2 (átlagos éjszakai forgalmú utak) | 0,780 | 0,777 | 0,773 | 0,150 | 0,148 | 0,145 | 0,070 | 0,075 | 0,082 |

| Jelleg2=3 (kis éjszakai forgalmú utak) | 0,802 | 0,799 | 0,795 | 0,139 | 0,138 | 0,136 | 0,059 | 0,063 | 0,069 |

| * ÚT 2-1.109:2004 szerinti forgalomjelleg kategóriák |

## 4.4 Az egyes út- és időszakaszokhoz tartozó vonatkoztatási egyenértékű A-hangnyomásszint (LAeq(7,5)g,s,t,j ) számítása

## 4.4.1 Az egyes út- és időszakaszokhoz tartozó vonatkoztatási egyenértékű A-hangnyomásszintet a vonatkoztatási távolságban, ”A”-típusú akusztikai érdességi kategóriába tartozó kopórétegen (a g-edik órán belül, az s-edik számítási útszakaszhoz tartozó

## j-edik út- és t-edik időszakasz esetén az LAeq(7,5)g,s,t,j mennyiséget) a szakaszra megállapított forgalmi (Q és v) adatokból a következő összefüggéssel kell meghatározni:

## ahol a g-edik órán belül az s-edik számítási útszakaszhoz tartozó j-edik út- és t-edik időszakaszban

## LAeq(7,5)g,s,t,j,i az i-edik akusztikai járműkategória forgalmától származó kiindulási egyenértékű A-hangnyomásszint

## LAeq(7,5)g,s,t,j,v az egyes villamos típusoknak (összesen ”n”-féle típus a j-edik vágánytípuson) forgalmától származó kiindulási egyenértékű A-hangnyomásszint

## 4.4.2 Az LAeq(7,5)g,s,t,j,i kiszámítása:

## LAeq(7,5)g,s,t,j,i = [ Kt + KD ] g,s,t,j,i

## A [ Kt ] g,s,t,j,i számítása:

## ahol:

## – az adott akusztikai járműkategóriához tartozó Ai Bi Ci Di Ei Fi állandókat a 4. táblázat szerint kell behelyettesíteni:

## 4. táblázat

| i = | Ai | Bi | Ci | Di | Ei | Fi |

| 1 | 2.00 | 2.92 | 3.03 | 2.00 | 2.62 | 3.92 |

| 2 | 2.40 | 2.92 | 3.17 | 2.10 | 3.15 | 3.79 |

| 3 | 2.70 | 2.92 | 3.90 | 1.86 | 5.07 | 2.53 |

## – vg,s,t,j,i az adott akusztikai járműkategóriához rendelt mértékadó sebesség, km/óra

## – pg,s,t,j.i az adott akusztikai járműkategóriához tartozó terhelési paraméter az 5. táblázat szerint.

## 5. táblázat

| Akusztikai járműkategória: | pg,s,t,j.i értéke |

| emelkedő esetén (c%>0) | lejtő esetén (c%<0) |

| egyenletesen áramló forgalom esetén |

| I. | c | c |

| II. és III. | c | -c |

|  | gyorsuló forgalom esetén |

| I. | c+2 | c+2 |

| II. és III. | c+4 | c+4 |

|  | lassuló forgalom esetén |

| I. | c-1 | c-1 |

| II. és III. | c-3 | -c-3 |

## − [ K ] g,s,t,j,i útburkolat miatti korrekció értékét az adott akusztikai járműkategóriához tartozóan az adott kopórétegre az OKA adatbázisából kell venni.

## Ha az OKA adatbázisának a [ K ] g,s,t,j,i útburkolat miatti korrekcióval való kiegészítése az adott járműkategóriához tartozóan az adott kopórétegre nem történt meg, akkor a zajtérkép készítőjének szakmai döntésétől függően a kopóréteg

## a) vagy besorolható a 6. táblázat szerinti kategóriákba, és ha a kopórétegen

## (a kopóréteg életkorától függetlenül) nincs felfagyástól, az alépítményen pedig nincs vetemedéstől vagy egyéb okból származó, kiterjedt folytonossági hiány vagy törés, akkor a 6. táblázat megfelelő [ K ] g,s,t,j,i értéket kell behelyettesíteni, és a 4. táblázat szerinti Ai Bi regressziós állandókat kell használni;

## b) vagy ha az a) pont szerinti besorolás nem hajtható végre, akkor [ K ] g,s,t,j,i = 0, és az Ai Bi regressziós állandók értékeit a 4. táblázat szerinti értékek helyett az adott járműkategóriához tartozóan az adott útburkolatra méréssel kell meghatározni. A mérésekért a zajtérkép előállítója a felelős.

## Az Ai Bi regressziós állandók mért értékei nem lehetnek 5 évnél régebbiek.

## Az Ai Bi regressziós állandók méréssel való meghatározásánál az MSZ EN ISO 11819-1 „Az útburkolatok közlekedési zajra gyakorolt hatásának mérése. 1. rész: Statisztikus elhaladási mérési módszer” előírásai szerint eljárni. Ez a szabványnak a regresszió alapjául szolgáló adatgyűjtésre (mérésre) vonatkozó előírásai, továbbá a műszerezésre és a regresszió-analízisre vonatkozó követelményei teljesítését jelenti. A vizsgálatok során az MSZ EN ISO 11819-1 szerinti 1. járműkategóriát az I. akusztikai járműkategóriának, a 2. járműkategóriát a II: akusztikai járműkategóriának és a 2.b. járműkategóriát a III. akusztikai járműkategóriának kell megfeleltetni. Az Ai Bi regressziós állandók értékeként a vizsgálattal meghatározott ai és bi állandók tizedrészét kell aalkalmazni, azaz Ai = ai /10 és Bi = bi /10.

## Megjegyzés: A szabvány szerinti „SPBI” (statisztikus elhaladási index) meghatározása nem feladat, mivel az alkalmatlan a sebesség hatásainak a becslésére.

## 6. táblázat

| Akusztikai érdességi kategória | [ K ] g,s,t,j,i = | Kopórétegek (ÚT 2-3.301 szerint) |

| A | 0 | AB-8; AB-12; ZMA-8; ÖA-8; ÖA-12; Modifikált vékonyaszfaltok |

| B | 0,29 | AB- és ÖA-kopórétegek pmB-B 35/65 kötőanyaggal 4 évesnél régebbi vékonyaszfaltok ZMA -12; mZMA-12; AB-12/F |

| C | 0,49 | 4 évesnél régebbi AB- és ÖA-kopórétegek pmB-B 35/65 kötőanyaggal Egy, ill. kétrétegű bevonattal (UKZ 5/8; UKZ 2/5) ellátott kopórétegek AB-16; AB-16/F; AB-20 |

| D | 0,67 | Beton Repedezett aszfalt kopórétegek 4 évesnél régebbi AB-16; AB-16/F; AB-20 |

| E | 0,78 | Kiverődött beton Kiskockakő Díszburkolat (pl.VIACOLOR) Keramit ÉHA-16; ÉHA-20 |

## A [ KD ] g,s,t,j,i számítása:

## [ KD ] g,s,t,j,i = 10 lg (Q g,s,t,j,i /v g,s,t,j,i) - 16,3

## ahol

## v g,s,t,j,i az adott akusztikai járműkategóriához rendelt mértékadó sebesség, km/óra

## Q g,s,t,j,i az adott akusztikai járműkategóriához tartozó forgalomnagyság, jármű/óra

## Megjegyzés: Ha Q/v nagyobb 43-nál, akkor a jelen előírás szerinti számítás nem végezhető el.

## 4.4.3 Az LAeq(7,5)g,s,t,j,v kiszámítása:

## A vizsgált, Tt(másodperc) hosszúságú időszakaszra vonatkozó és Qv [jármű/óra] mértékegységben kifejezett kötöttpályás forgalomtól származó kiindulási egyenértékű A-hangnyomásszintje, dref = 7,5 m távolságban:

## LAeq(7,5)g,s,t,j,v= 10 lg (Qv) + Cvk

## ahol:

## v a 4.1 pont szerinti 1. táblázatból a járműtípus azonosítója

## Cvk a járműtípustól (v) és vágánytípustól (k) függő állandó a 7. táblázat szerint.

## 7. táblázat

## A kötöttpályás járműtípustól és a vágánytípustól függő állandó Cvk

| Vágány típus k= | Megnevezés | v=1 ICS1 | v=2 ICS2 | v=3 UVMM | v=4 UVMPM | v=5 T5C5 | v=6 TW 6000 | v=7 HÉV | v=8 HÉV (dupla) |

| Burkolatban fekvő vágányok |

| 1 | Tömbsínes, nagypaneles vágány | 55.1 | 57.2 | 54.5 | 55.9 | 58.4 | 56.1 |  |  |

| 2 | Phoenix-sín zúzottkő ágyazaton nagykockakő burkolat | 53.0 | 57.2 | 49.2 | -- | -- |  |  |  |

| 3 | Phoenix-sín, R.A.F.S. ágyazat | -- | 58.0 | -- | 55.3 | 55.1 |  |  |  |

| 4 | Kispaneles | -- | -- | -- | 56.8 | 56.1 |  |  |  |

| Nyitott vágányok |

| 5 | Vignol-sín 34 kg/m, zúzottkő ágyazat | 46.1 | -- | 45.6 | 48.3 | 49.4 |  |  |  |

| 6 | Vignol-sín 48 kg/m, zúzottkő ágyazat | -- | -- | -- | -- | 47.3 | 51.6 | 52.0 | 55.0 |

| 7 | Vignol-sín 34 kg/m, fa alj | 49.4 | -- | -- | -- | -- |  |  |  |

| 8 | Vignol-sín 48 kg/m, fa alj | 50.8 | -- | -- | -- | -- | -- |  |  |

| 9 | Vignol-sín 48 kg/m, vasbeton lemez alj | 50.0 |  |  |  |  |  |  |  |

## A táblázatban nem szereplő kötöttpályás járműtípus vagy vágánytípus esetén a kötöttpályás járműtípustól és a vágánytípustól függő Cvk állandó értékét méréssel kell meghatározni.

## 5. A hosszútáv, nagytáv forgalmának figyelembevétele

## 5.1 A Zr. szerint a közlekedéstől származó zajterhelés zajtérképét az aktuális forgalmi adatokból, a fennálló zajhelyzetre kell elkészíteni.

## Bizonyos esetekben, például az intézkedési tervekben elhatározott forgalomszervezési intézkedések várható hatásának értékeléséhez, szükség lehet a hosszútávú, nagytávú forgalomtól származó zajterhelés becslésére. A közúthálózat új külterületi szakaszain, a hálózat módosulása, illetve új forgalomvonzó létesítmény építése miatt lényeges forgalom-változással érintett útszakaszokon a forgalom megváltozását eredményező fejlesztések terveinek (tanulmányterv, hatásvizsgálat) forgalombecslési adatait kell figyelembe venni. Amennyiben ilyen, a forgalom-fejlődést lényegesen érintő hatással nem kell számolni, a vonatkozó (ÚT 2-1.118:2000 „Közutak távlati forgalmának meghatározása előrevetítő módszerrel” című) útügyi műszaki előírást kell alkalmazni.

## Ezt meglévő útvonalak és megítélési pontok esetén a legpontosabban a zajmérésre alapozott számítással lehet elvégezni.

## Tervezett, létesítendő útvonalak, illetve megítélési pont esetén mérések elvégzésére nincs mód, ekkor a mértékadó zajterhelést természetesen csak a távlati forgalmi adatok felhasználásával és csak számítással lehet becsülni.

## 5.1.1 A hosszútáv, nagytáv forgalmától származó zajterhelés mérésre alapozott becslése, meglévő útvonal és megítélési pont esetén

## 5.1.2 A megítélési ponton és e rendelet szerint kijelölt vonatkoztatási ponton,

## – napközben 08.00-12.00 óra vagy 15.00-18.00 óra között,

## – este 18.00-20.00 óra között,

## – éjszaka 22.00-23.00 vagy 05.00-06.00 óra között

## legalább 1-1 óra időtartamban mérni kell az egyenértékű A-hangnyomásszintet, valamint forgalomszámlálást és átlagsebesség-mérést kell végezni a 2. számú melléklet szerint.

## A forgalomszámlálás terjedjen ki az összes olyan közútra, amelynek forgalma befolyásolhatja a megítélési ponton keletkező zajszintet.

## 5.1.3 A 2.1 pont szerinti mérésekkel meghatározott mérési eredmények felhasználásával előjeles (+ vagy – előjeles) korrekciót kell megállapítani mind a vonatkoztatási távolságra, mind a megítélési pontra, a megfelelő napszakokra, és a következő mennyiségeket kell számolni:

## A vonatkoztatási távolságban:

## ΔLAeq(7,5) = LAeq(7,5 számított) - LAeq (7,5 mért )

## A megítélési ponton:

## ΔLAeq(d,h) = LAeq(d,h számított) - LAeq(d,h mért )

## 5.1.4 A távlati forgalmi adatokra vonatkozóan a következők számíthatók:

## LAeq(7,5 korrigált, távlati) = LAeq(7,5 számított, távlati ) - ΔLAeq(7,5)

## LAeq(d, h korrigált, távlati) = LAeq(d, h számított, távlati) - ΔLAeq(d, h)

3. számú melléklet a 25/2004. (XII. 20.) KvVM rendelethez
