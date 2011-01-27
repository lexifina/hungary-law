## Az elektronikus kormányzati gerinchálózat informatikai biztonsági szabályzata

| 1. | Informatikai biztonsági szabályzat |

|  | 1.1. | A biztonsági szabályzat hatálya |

|  | 1.2. | Biztonsági szabályzat helye a szabályzatok között |

| 2. | Biztonsági intézkedések |

|  | 2.1. | Szervezet |  |

|  |  | 2.1.1. | Felelősségi körök |

|  |  | 2.1.2. | Személyzet |

|  |  | 2.1.3. | Eljárás rend |

|  |  | 2.1.4. | Csatlakozás biztonsági feltételei |

|  |  | 2.1.5. | Beszerzés |

|  |  | 2.1.6. | Üzemeltetés |

|  |  | 2.1.7. | Fenntartás |

|  |  | 2.1.8. | Katasztrófa terv |

|  |  | 2.1.9. | Biztonsági osztályok |

|  | 2.2. | Infrastruktúra |

|  |  | 2.2.1. | Általános intézkedések |

|  |  | 2.2.2. | Számítógéptermek |

|  |  | 2.2.3. | A számítógéptermeken kívül található eszközök védelme |

|  |  | 2.2.4. | Üzemelés biztosítása |

|  |  | 2.2.5. | Villámcsapás- és túlfeszültség-védelem |

|  |  | 2.2.6. | Tűzvédelem |

|  |  | 2.2.7. | Vízvédelem |

|  | 2.3. | Hardver eszközök |

|  |  | 2.3.1. | Szerverek |

|  |  | 2.3.2. | Munkaállomások |

|  |  | 2.3.3. | Hálózati hardver eszközök |

|  |  | 2.3.4. | A csatlakozott intézmények által üzemeltetett eszközök |

|  |  | 2.3.5. | Hardver eszközök nyilvántartása |

|  |  | 2.3.6. | Tartalék eszközök |

|  | 2.4. | Szoftverek |

|  |  | 2.4.1. | Szoftverkarbantartás |

|  |  | 2.4.2. | Biztonsági mentések |

|  |  | 2.4.3. | Vírusvédelem |

|  | 2.5. | Hálózat védelme |

|  |  | 2.5.1. | Rendelkezésre állás biztosítása |

|  |  | 2.5.2. | Jogosultsági rendszer |

|  |  | 2.5.3. | MPLS VPN |

|  |  | 2.5.4. | IP VPN |

|  |  | 2.5.5. | Tűzfalakra, védelmi intézkedésekre vonatkozó követelmények |

|  |  | 2.5.6. | Csatlakozott szervezetekre vonatkozó szabályok |

|  |  | 2.5.7. | Hálózat felügyelete |

|  |  | 2.5.8. | Rendhagyó (rendkívüli) események jelentése, kezelése |

| 3. | Záró rendelkezések |

|  | 3.1. | A biztonsági szabályzat bevezetése, oktatása |

|  | 3.2. | A biztonsági szabályzat hatálybalépése |

|  | 3.3. | A biztonsági szabályzattól való eltérés rendje |

|  | 3.4. | A biztonsági szabályzat aktualizálásának, kiegészítésének rendje |

## 1. Az informatikai biztonsági szabályzat célja

## Az informatikai biztonsági szabályzat (a továbbiakban: IBSz) célja az elektronikus kormányzati gerinchálózat (a továbbiakban: EKG) üzembiztonságát megteremtő szabályok és intézkedések meghatározása.

## 1.1. A biztonsági szabályzat hatálya

## Az EKG címzett feladata, hogy a csatlakozott szervezetek közötti elektronikus kommunikáció átviteli közege legyen, így a rajta átfolyó adatok tartalmával nem foglalkozik, azokért nem felel, ez minden esetben az egyes intézmények feladata. Emiatt a biztonsági szabályzat az üzembiztonságról szól, és adatbiztonsággal kapcsolatos kérdésekkel kizárólag akkor foglalkozik, ha azok hatással lehetnek az üzembiztonságra.

## A dokumentum hatálya kiterjed:

## – az EKG hálózatgazdájának feladataira és kötelességeire;

## – a hálózat üzemeltetőjének feladataira és kötelességeire;

## – a hálózathoz csatlakozott intézmények feladataira és kötelességeire.

## 1.2. Biztonsági szabályzat helye a szabályzatok között

## Az IBSz a biztonsági kérdésekben alapszabályzat, ugyanakkor nem tér ki részletesen az üzembiztonság minden aspektusára, hanem az őt körülvevő szabályozási rendszer szerves része, lehetőség szerint kerülve az átfedéseket. Tartalmazza ugyanakkor a szabályozás további szükséges területeit, amelyek azonban olyan mértékben helyzetfüggőek, hogy jogszabályi szinten szabályozásuk nem kezelhető.

## Az IBSz szándékoltan nem áll meg önmagában, hanem szervesen beilleszkedik az őt körülfogó szabályzati rendszerbe, vagyis eredeztethető a megfelelő jogszabályokból (pl. minősített adatról szóló rendeletek stb.) és szabványokból (pl. Országos Építési Szabályzat, ITSEC stb.), kiegészíti az EKG működési szabályzatát és megteremti az alapot az üzembiztonság egyes aspektusaival (pl. biztonsági szervezet működési szabályzata, katasztrófa terv stb.) részletesen foglalkozó szabályzatok létrehozásához.

## A biztonsági szabályzatot a hálózatgazdának évente felül kell vizsgálni és szükség esetén aktualizálni, kiegészíteni. A hálózatban bekövetkező jelentős változások esetén a felülvizsgálatot soron kívül el kell végezni.

## 2. Biztonsági intézkedések

## A biztonsági intézkedések alkalmazása szempontjából öt fő kategóriát különböztettünk meg:

## szervezet – az EKG biztonságáért felelős szervezetre vonatkozó, illetve az ahhoz kötődő intézkedések;

## infrastruktúra – az EKG fizikai védelmét biztosító környezetre vonatkozó intézkedések;

## hardver eszközök – az EKG hardver eszközeire vonatkozó intézkedések;

## szoftverek – az EKG üzemeltetéséhez és szolgáltatásaihoz szükséges szoftverekre vonatkozó intézkedések;

## hálózat védelme – a fenti csoportokba nem besorolható, de a hálózat védelmét szolgáló intézkedések.

## Az intézkedések konkrét feladatokat jelentenek, a felelős és a végrehajtás ajánlott gyakoriságával együtt.

## A felelős megjelölésénél az IBSz szabályzat a kormányzati célú hírközlési szolgáltató, az üzemeltető és a csatlakozott/csatlakozandó intézmény szintjén marad (az IBSZ alapfogalmainak értelmezését a szabályzat 1. számú függeléke tartalmazza).

## 2.1. Szervezet

## 2.1.1. Felelősségi körök

| Biztonságért felelős szervezet kialakítása |

| Feladat: | – | A biztonságért felelős szervezet felállítása a következő munkakörök kialakításával (munkaköri leírás készítése): |

|  | biztonságért felelős vezető – a hálózat informatikai biztonságáért, és ennek megfelelően magáért a (csatlakozott intézményi, illetve üzemeltetői) biztonsági szabályzat (BSZ) meglétéért, tartalmáért felelős személy |

|  | biztonsági felügyelők – a BSZ betartásának ellenőrzéséért felelős személyek |

|  | biztonsági szakértők – a hálózat biztonságát célzó védelmi intézkedésekért, a káresemények elemzéséért, a BSZ naprakészen tartásáért felelős személyek |

|  | – | A megfelelő személyek körültekintő kiválasztása. |

| Eredmény: | Biztonságért felelős szervezet. |

| Felelős: | Kormányzati célú hírközlési szolgáltató (a szabályzat meglétéért, EKG-ra vonatkozó tartalmáért és a szervezet kialakításáért) |

| Gyakoriság: | A biztonsági szabályzat hatálybalépésekor, ezt követően szükség szerint (megfelelő munkatárs távozása stb.). |

| Feladatok és hatáskörök pontos meghatározása és dokumentálása |

| Feladat: | – | Az EKG-val kapcsolatban pontosan meg kell határozni, hogy mik a feladatok, kinek, milyen felelőssége van, és milyen hatáskörrel bír. Mindezt írásban dokumentálni kell, és gondoskodni kell arról, hogy az EKG-val kapcsolatba kerülő minden szereplő tisztában legyen a rá vonatkozó részekkel. |

| Eredmény: | Feladatok és hatáskörök pontos leírása. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | A biztonsági szabályzat hatálybalépésekor, majd ezt követően legalább évente kell felülvizsgálni, illetve káresemény esetén azonnal. |

## 2.1.2. Személyzet

| Személyzet kiválasztása |

| Feladat: | – | Mivel az EKG nemzetbiztonsági jelentőséggel bír, ezért az azzal kapcsolatba kerülő, annak tervezésében, üzemeltetésében, karbantartásában részt vevő személyeket nagyon körültekintően, az erre vonatkozó jogszabályoknak megfelelően kell kiválasztani. |

|  | – | Külön figyelmet kell fordítani mindazokra, akik az EKG üzemeltetésében adminisztrátori jogosultságokkal rendelkeznek, az ő megbízhatóságuk ellenőrzése kiemelten fontos feladat. |

| Eredmény: | Körültekintően kiválasztott, megbízható személyzet. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető, csatlakozott szervezetek |

| Gyakoriság: | A biztonsági szabályzat hatálybalépésekor, majd ezt követően szükség szerint (munkatárs távozása stb.). |

| Személyzet képzése |

| Feladat: | – Feladatuk szerint csoportosítva el kell készíteni a személyi állomány képzését segítő anyagokat és meg kell szervezni azok tervszerű és ellenőrzött végrehajtását. |

|  | – A képzések során fokozott figyelmet kell fordítani biztonsági kérdésekre. |

|  | – A képzések színvonalát és az elsajátított tudás szintjét ellenőrizni kell. |

| Eredmény: | Képzett, a feladatait megfelelően ellátni képes, a biztonsági előírásokkal és teendőkkel tisztában lévő személyi állomány. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | A biztonsági szabályzat hatálybalépésekor, majd ezt követően szükség szerint (új munkatárs belépése stb.), rendszeres ismeret karbantartás. |

| Biztonsági előírások betartásának ellenőrzése |

| Feladat: | – A biztonsági felügyelőnek folyamatosan ellenőriznie kell, hogy a személyzet tisztában van a megfelelő biztonsági előírásokkal és be is tartja azokat. – Az ellenőrzéseket dokumentálni kell, a jegyzőkönyveket legalább 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

| Eredmény: | Betartott biztonsági előírások. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Folyamatosan, de nem kiszámítható módon (fontos, hogy ne lehessen rá előre felkészülni). |

## 2.1.3. Eljárás rend

| Védelmi intézkedések ellenőrzése és felülvizsgálata |

| Feladat: | – Az üzembiztonság érdekében tett védelmi intézkedéseket a biztonsági felügyelőnek rendszeresen kell ellenőriznie és felülvizsgálnia. |

|  | – Az ellenőrzéseket és felülvizsgálatokat dokumentálni kell, az ezt tartalmazó jegyzőkönyveket legalább 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

|  | – A felülvizsgálat eredményeképp a felügyelő a védelmi intézkedések módosítását kezdeményezheti. |

| Eredmény: | Ellenőrzött, visszakövethető és naprakészen tartott védelmi intézkedések. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Félévente, illetve káresemény esetén azonnal. |

| Káresemény kezelése |

| Feladat: | – Az üzembiztonság sérülése esetén a felfedezést követően haladéktalanul meg kell kezdeni az elhárítást és a károk csökkentését (lásd alább a biztonsági események kezelésénél). |

|  | – A káreseményeket elhárításuk után azonnal elemeznie kell a biztonsági szervezetnek (a biztonsági vezető vezetésével a kijelölt biztonsági szakértők végzik). |

|  | – Az elemzést dokumentálni kell, a jegyzőkönyvet legalább 5 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

|  | – Az elemzés eredményeképp a biztonsági szakértők akciótervet dolgoznak ki a hasonló káresemények jövőbeni elkerülésének érdekében. Ebben javaslatot tehetnek a védelmi intézkedések és a felelősségi körök megváltoztatására, kiegészítésére. |

|  | – Az akciótervet a biztonságért felelős vezető hagyja jóvá, ezt követően haladéktalanul végre kell hajtani. |

| Eredmény: | Elhárított és elemzett káresemény, a jövőbeli előfordulás elkerülését célzó jóváhagyott és végrehajtott akcióterv. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Káresemény esetén. |

## 2.1.4. Csatlakozás biztonsági feltételei

| Csatlakozott/csatlakoztatandó szervezetek biztonsági szabályzata |

| Feladat: | – Minden csatlakozó szervezetnek az EKG biztonsági szabályzatával összhangban álló, azzal teljes mértékben harmonizáló biztonsági szabályzatot kell kidolgozni (újonnan csatlakozó szervezet esetén ez alapkövetelmény), melyet a kormányzati célú hírközlési szolgáltató nevében az EKG biztonsági felelősének véleményeznie kell. Ha a csatlakozott szervezet teljes biztonsági szabályzata nem adható ki véleményezésre, akkor az EKG-t érintő részeket kell véleményezni. |

| Eredmény: | Az EKG biztonsági felelőse által véleményezett biztonsági szabályzat. |

| Felelős: | Csatlakozott/csatlakozandó szervezet |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépését követően 6 hónapon belül, illetve a csatlakozás előtt, a csatlakozással hatályba léptetve. |

## 2.1.5. Beszerzés

| Beszerzési politika |

| Feladat: | – A Hálózatgazdának egységes beszerzési politikát kell kidolgoznia az EKG-ra vonatkozó minden (hardver, szoftver stb.) beszerzési feladatra, a közbeszerzésre vonatkozó jogszabályok maximális figyelembevételével. |

|  | – A beszerzési politikában lehetőség szerint maximálisan érvényesíteni kell az üzembiztonság fenntartását elősegítő szempontokat. |

|  | – Amennyire ezt a közbeszerzés szabályai megengedik, törekedni kell arra, hogy az EKG eszközei minél egységesebbek legyenek. |

| Eredmény: | Egységes beszerzési politika (egységes megbízhatóságú rendszer). |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor aktualizálni a külső tényezők (pl. jogszabályok stb.) megváltozásakor, illetve a piac lényeges változásakor szükséges. |

| Amortizációs szabályozás |

| Feladat: | – A Hálózatgazdának ki kell dolgoznia az EKG minden eszközére (beleértve a hardver és a szoftver eszközöket is) vonatkozó amortizációs szabályokat. |

|  | – Az amortizációs szabályok kidolgozásakor az eszközöket azonos amortizációs jellemzővel rendelkező kategóriákba kell sorolni, minden egyes kategóriára meghatározva az amortizációs időtartamot és az amortizációs eljárást. |

| Eredmény: | Amortizációs szabályok. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | A biztonsági szabályzat hatálybalépésekor, aktualizálni a külső vagy belső tényezők (pl. technológia stb.) megváltozásakor szükséges. |

## 2.1.6. Üzemeltetés

| Eszköznyilvántartás |

| Feladat: | – Az üzemeltetőnek naprakész nyilvántartást kell vezetni minden az EKG-hoz tartozó eszközről (hardverek, szoftverek stb.), annak állapotáról, helyéről stb. (a nyilvántartásnak minden olyan adatot tartalmaznia kell, ami alapján az adott eszköz megtalálható, felügyelhető, tervszerűen karbantartható, amortizálható stb.). |

|  | – A nyilvántartásban már a beszerzési szándéktól fogva meg szükséges jeleníteni az adott eszközt és állapotát (beszerzés alatt, leszállítva, raktárban, tesztelés alatt, installálás alatt, üzemben, meghibásodott, javítás alatt, kivezetés alatt, amortizálva stb.) a teljes életciklus során végigkövetni. |

| Eredmény: | Naprakész eszköznyilvántartás. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

| Tesztelés |

| Feladat: | – Az üzemeltetőnek minden eszköztípusra (lehetőség szerint a tömeges, rendszerszerű beszerzés előtt) teszttervet kell készítenie, melynek végrehajtása után az adott típusú eszköz már nagy biztonsággal üzembe helyezhető. |

|  | – Minden eszközt üzembe helyezése előtt tesztelni kell az előre kidolgozott teszttervek alapján. |

|  | – Káresemények esetén az elemzések eredménye magával vonhatja a teszttervek kiegészítését. |

| Eredmény: | Kész teszttervek, csökkentett kockázatú üzembe helyezési folyamat. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor, majd ezt követően folyamatosan. |

## 2.1.7. Fenntartás

| Változások |

| Feladat: | – Az EKG-ban bekövetkezett bármilyen változást (pl. új tűzfal üzembe helyezése, korszerűtlen eszközök újabbra cserélése, router konfiguráció változtatása stb.) dokumentálni kell, minden a változás visszakövethetőségét elősegítő információval (pl. az esemény leírása, oka, az azt megelőző helyzet, az általa okozott tényleges változások, ezek hatása stb.). |

|  | – A változások jegyzőkönyvét legalább 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

| Eredmény: | Nyomon követhető változások. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Bármilyen az EKG-ban bekövetkező változással egy időben. |

| Külső cégekkel végeztetett javítások, karbantartások |

| Feladat: | – Minden esetben, amikor külső céget kell valamilyen javítási vagy karbantartási feladattal megbízni, amely csak a hálózatba „beavatkozva” (helyszíni javítás, illetve távoli elérésen keresztül végzett tevékenységek stb.) végezhető el, az üzemeltető köteles ezt a tevékenységet folyamatosan ellenőrizni, felügyelni és gondoskodni arról, hogy az EKG-ra vonatkozó bizalmas információk (pl. tűzfal konfiguráció stb.) ne kerülhessenek illetéktelen kezekbe. |

| Eredmény: | A külső cégek bevonásával járó kockázat minimalizálása. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Minden esetben, amikor külső cég helyszíni javítást vagy karbantartást végez. |

## 2.1.8. Katasztrófa terv

| Katasztrófa terv kidolgozása |

| Feladat: | – A Hálózatgazdának és az üzemeltetőnek együttműködve ki kell dolgozni a megfelelő katasztrófa tervet, mely csökkenti a bekövetkezett esemény okozta károkat, segít fenntartani a működést, és hozzájárul az eredeti állapot (vagy a körülményekhez képest az ahhoz legközelebb álló állapot) visszaállításához. |

|  | – A katasztrófa terv részeként el kell készíteni a végrehajtás feltételeit megteremtő akciótervet, amit jóváhagyás után gyakoroltatni kell. |

|  | – A katasztrófa tervet évente aktualizálni kell, és tükröznie kell az időközben beállt változásokat. Amennyiben szükséges, úgy ismételten akciótervet kell megfogalmazni és azt gyakoroltatni. |

|  | – A katasztrófa tervet ismertetni kell az érintettekkel, és gondoskodni kell arról, hogy minden érintett tisztában legyen a rá háruló feladatokkal. |

| Eredmény: | Katasztrófa terv. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor, majd ezt követően évente, illetve a körülmények lényegi megváltozása esetén kell aktualizálni. |

## 2.1.9. Biztonsági osztályok

| EKG-eszközök biztonsági osztályokba történő sorolása |

| Feladat: | – Az EKG, illetve az EKG üzemeltetéshez szükséges eszközöket az ITB ajánlásnak megfelelően három biztonsági osztályba kell besorolnia az üzemeltetőnek. A biztonsági osztályokba történő sorolás az ITB 12. ajánlásának 4.1. fejezetében leírt káreseményeknek megfelelően definiált kárérték osztályzás szerint kell, hogy történjen, annak alapján, hogy az adott eszköz kiesése vagy hibás működése mekkora hatással bírna. |

|  | – A biztonsági osztályokba sorolás támogatja, hogy az adott rendszerelem mennyire fontos a tartalékképzés, a karbantartás és redundancia biztosításának szempontjából. |

|  | – Az alábbi osztályokba kell sorolni az eszközöket: |

|  | = A – alapbiztonsági követelmények, ha az elem kiesése vagy hibás működése maximum „2”, azaz legfeljebb közepes kárértékű eseményt okozhat; |

|  | = F – fokozott biztonsági követelmények, ha az elem kiesése vagy hibás működése maximum „3”, azaz legfeljebb nagy kárértékű eseményt okozhat; |

|  | = K – kiemelt biztonsági követelmények, ha az elem kiesése vagy hibás működése „4+”, azaz katasztrofális kárértékű eseményt okoz |

| Eredmény: | Biztonsági osztályok kialakítása. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor. |

## 2.2. Infrastruktúra

## Alábbiakban az EKG fizikai védelmét biztosító infrastruktúra kialakítására és üzemeltetésére vonatkozó intézkedések felsorolása található.

## 2.2.1. Általános intézkedések

| Biztonsági zónák kialakítása |

| Feladat: | – Az EKG eszközeit tároló, valamint az üzemeltetéssel más módon kapcsolódó helyiségeket biztonsági zónákra kell felosztani. |

|  | – Az épületbe való bejutáson túl biztosítani kell, hogy az EKG üzemelést biztosító helyiségekbe (pl. szerverszoba, hálózati felügyeleti szoba) csak azok juthassanak be, akik jogosultak a belépésre. |

|  | – Definiálni szükséges, hogy melyik helyiségek legyenek védettebbek, mint az épület egyéb helyiségei (pl. szerverszoba). |

| Eredmény: | Fizikailag elkülönített biztonsági zónák az EKG üzemelését biztosító épületekben. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor. |

| A biztonsági zónákon belüli közlekedés szabályozása |

| Feladat: | – Definiálni szükséges, hogy az egyes helyiségekbe (pl. szerverszoba) ki léphet be. Javasolt, hogy az üzemeltető különböző szakértő csoportjai csak saját helyiségeikbe kapjanak belépést (pl. a hálózati eszközöket tartalmazó terekbe csak a hálózati szakértők juthassanak be). |

| Eredmény: | A definiált biztonsági zónákba csak a jogosult embereknek, személyeknek van belépési lehetősége. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | A rendszer kiépítésekor, illetve új helyiségek igénybevételekor. |

## 2.2.2. Számítógéptermek

| Számítógéptermek |

| Feladat: | – Az EKG védett eszközeit (szerverek, menedzsment eszközök stb.) az üzemeltető köteles a kormányzati célú hírközlési szolgáltató által kijelölt helyiségekben elhelyezni. |

|  | – A hálózatgazdának gondoskodnia kell arról, hogy a kijelölt helyiségek rendelkezzenek mindazokkal a felszerelésekkel, amelyek a nagy üzembiztonságú rendszerek üzemeltetéséhez kellenek (részletesen lásd az Infrastruktúra fejezet további intézkedéseiben). |

| Eredmény: | Az EKG eszközeinek a nagy üzembiztonságú működést biztosítani képes környezetben való elhelyezése. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Amikor az EKG bővülése ezt szükségessé teszi. |

| Számítógéptermek beléptető rendszere |

| Feladat: | – Az EKG eszközeinek helyt adó számítógéptermeknek olyan beléptető rendszerrel kell rendelkezniük, melyek lehetővé teszik, hogy kizárólag az arra jogosult személyek juthassanak be. |

|  | – A számítógéptermekbe való belépéseket, illetve belépési kísérleteket minden esetben naplózni kell, a naplókat legalább 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

| Eredmény: | Az EKG számítógéptermeibe csak a hozzáféréshez jogosult emberek lépnek be, illetéktelenül nem juthatnak be a helyiségekbe. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | A számítógépterem üzembe helyezésekor, illetve a jogosulti kör változásakor haladéktalanul. |

| Számítógéptermekre vonatkozó belépési jogosultságok kezelése |

| Feladat: | – Definiálni kell a számítógéptermekbe való belépési jogosultságok menedzselésének módját. Meg kell határozni, hogy kinek adható ki belépési engedély, mikor módosulhat valakinek a hozzáférése, illetve belépési jogosultság megszűnése esetén azonnali hatállyal intézkedést kell tenni a jog megvonására. |

| Eredmény: | Az EKG számítógéptermeibe csak a hozzáféréshez jogosult emberek, személyek lépnek be. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Számítógépterem üzembe helyezésekor, illetve a jogosulti kör változásakor haladéktalanul. |

| Számítógéptermek fizikai védelme |

| Feladat: | – Az üzemeltetőnek gondoskodnia kell arról, hogy az EKG eszközeinek helyt adó számítógéptermek (ideértve a klímaberendezéseket és a szünetmentes tápellátást biztosító eszközöket is) fizikailag is védettek legyenek úgy, hogy mindennemű lopás, manipuláció, külső beavatkozás, támadás lehetőség szerint elkerülhető, illetve legrosszabb esetben legalább észlelhető legyen. |

|  | – A megyei központokban elsősorban a számítógépszekrények védelmét szükséges megoldani, mivel a számítógépes helyiségek ott nem az EKG tulajdonát képezik. |

| Eredmény: | Fizikailag védett számítógéptermek. |

| Felelős: | Az üzemeltető telephelyén az üzemeltető, a kormányzati célú hírközlési szolgáltató telephelyén lévő helyiségek védelméért a kormányzati célú hírközlési szolgáltató a felelős. Csak olyan helyiségben lehet EKG eszközt elhelyezni, amelyre annak üzemeltetője garanciát vállal az EKG normáinak megfelelő biztonságáért. |

| Gyakoriság: | Számítógéptermek kialakításakor 2 évente, illetve átalakításkor felülvizsgálva az intézkedéseket. |

| Számítógépszekrények védelme |

| Feladat: | – Az üzemeltető köteles az EKG megyei csatlakozási pontjainál elhelyezett eszközeit az illetéktelen hozzáféréstől számítógépszekrényekkel védeni. |

|  | – Gondoskodni kell arról, hogy a számítógépszekrények kinyitását kizárólag arra jogosult személy tehesse meg. |

|  | – A számítógépszekrényekhez való hozzáférést minden esetben naplózni kell, a naplókat legalább 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

| Eredmény: | A területi alközpontokban elhelyezett eszközök megfelelő szintű védelme. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Újabb csoportos csatlakozási pontok kialakításakor, 2 évente felülvizsgálva az intézkedéseket. |

| Belépési eszközök (pl. belépési kártya) használati szabályának előírása |

| Feladat: | – Rögzíteni (valamennyi használóval ismertetni) kell a belépésre szolgáló eszközök használati szabályait. Ezek a szabályok a következők: |

|  | eszköz elvesztésének bejelentési kötelezettsége, |

|  | eszköz másra való átruházásának tiltása, |

|  | eszköz biztos helyen való őrzése, |

|  | kilépéskor eszköz visszaadása. |

|  | – A szabályokat a belépési eszköz használóival ismertetni kell. |

| Eredmény: | Belépési eszközök rendeltetésének megfelelő használata. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Belépési eszköz kiadásakor. |

## 2.2.3. A számítógéptermeken kívül található eszközök védelme

| Számítógéptermeken kívül található eszközök védelme |

| Feladat: | – A számítógéptermeken kívül található, távközlési szolgáltatótól bérelt telekommunikációs csatornákat is védeni szükséges. Mivel ezek az eszközök nem az EKG tulajdonát képezik, ezért a távközlési szolgáltatóval kötött szerződésben kell felelősségszintű védelmet biztosítani (rendelkezésre állás, tartalék biztosítása, hibaelhárítási kötelezettség). |

|  | – Az EKG-hoz csatlakozó intézmények biztonságos üzemelése szempontjából javasolt, hogy az intézmény biztosítson hozzáférést saját az EKG-hoz csatlakozó routeréhez, valamint hiba esetén bejelentési kötelezettsége legyen az üzemeltető felé. |

| Eredmény: | Számítógéptermeken kívül található eszközök szerződésben meghatározott védelme. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Szerződések megkötésekor. |

| Üzemeltető raktárának védelme |

| Feladat: | – Mivel az üzemeltető a tartalék eszközöket nem a számítógéptermekben tárolja, ezért szükséges a raktárnak is a megfelelő belépési és fizikai védelme. A raktárba csak az üzemeltető léphet be, illetve akinek a kormányzati célú hírközlési szolgáltató erre külön engedélyt ad. |

| Eredmény: | Tartalék eszközöket tároló raktár megfelelő védelme. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Rendszer kialakításakor. |

## 2.2.4. Üzemelés biztosítása

| Eszközök szünetmentes áramellátásának biztosítása |

| Feladat: | – Az üzemeltetőnek – a kormányzati célú hírközlési szolgáltató által biztosított eszközök terhére – gondoskodnia kell arról, hogy az EKG eszközeinek szünetmentes áramellátása biztosítva legyen. Az üzemeltetést biztosító eszközöket redundáns UPS-sel szükséges ellátni. A hosszabb áramszünetek esetére tartalék generátort kell biztosítani az országos központban. A megyei központokban a tervezett áramszünetek esetére mobil generátoros megoldást kell biztosítani (az üzemeltető szakemberei szállítják a helyszínre a generátort). |

|  | – Az UPS-eket rendszeresen ellenőrizni kell, mert azok akkumulátorai gyakran meghibásodhatnak. Az UPS-ekből ennek megfelelően kellő számú tartalékot kell képezni (lásd 3.3.6. Tartalékgazdálkodás). |

| Eredmény: | Szünetmentes energiaforrással (UPS) és generátorral ellátott számítástechnikai eszközök. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Számítógéptermek kialakításakor, félévente ellenőrizve az UPS és a generátor állapotát. |

| Működtetéshez szükséges optimális külső hőmérséklet fenntartása |

| Feladat: | – A számítástechnikai eszközök zavarmentes működéséhez folyamatosan optimális hőmérsékletet kell fenntartani. Különösen veszélyeztetett időszak a nyár, amikor a környezeti hőmérséklet magasabb lehet, mint az eszközök tűrőképessége. Az optimális hőmérsékletet klimatizáló készülékekkel szükséges biztosítani. Ez vonatkozik a budapesti központra és a vidéki központokra egyaránt. |

| Eredmény: | Optimális hőmérséklet a számítástechnikai eszközök zavartalan működéséhez. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Infrastruktúra kiépítésekor, illetve új infrastruktúra igénybevételekor. |

| Klimatizáló, illetve megfelelő hőmérsékletet biztosító készülékek rendszeres ellenőrzése |

| Feladat: | – Az optimális hőmérsékletet biztosító eszközök működését folyamatosan ellenőrizni szükséges. Amennyiben a klíma nem üzemszerűen működik, úgy gondoskodni kell annak javításáról vagy szükség esetén cseréjéről. |

| Eredmény: | Optimális hőmérséklet a számítástechnikai eszközök zavartalan működéséhez. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Félévente. |

| Környezeti tűréshatárok túllépésének figyelése és kezelése |

| Feladat: | – A számítástechnikai eszközök környezeti tűréshatárát folyamatosan monitorozni kell. Amennyiben az eszköz túl magas hőmérsékletnek van kitéve, akkor intézkedni szükséges, amely a körülményektől függően többféle tevékenység is lehet (shutdown, állományok elmentése, tovább üzemelés, körülmények megváltoztatása). |

| Eredmény: | Az eszközök nem lépik túl fizikai tűréshatárukat, és folyamatosan üzemelnek. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

## 2.2.5. Villámcsapás- és túlfeszültség-védelem

| Túlfeszültség-védelem |

| Feladat: | – Fel kell készülni a vihar, illetve villám okozta károkozásokra. Az EKG eszközeit tároló épületeket megfelelő védelemmel kell ellátni, valamint védekezni kell a villám által okozott esetleges feszültségcsúcsokkal (feszültségtüskékkel) szemben is. |

| Eredmény: | Vihar- és villámvédett épületek, eszközök. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Kiépítéskor. |

| Túlfeszültség-védelem |

| Feladat: | – A villám keltette vagy a hálózati feszültség ingadozásából eredő túlfeszültség meghibásodást okozhat számítógépekben, illetve egyéb hardver eszközökben. Ezeket az eszközöket minden helyszínen védeni kell megfelelően érzékeny, akár többszintű feszültségszabályozó eszközökkel. |

| Eredmény: | Túlfeszültség elleni védelem. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Eszközök telepítésekor. |

## 2.2.6. Tűzvédelem

| Tűzvédelem |

| Feladat: | – A tűz ellen minden érintett helységben (budapesti központ, üzemeltető telephelyei, vidéki központok stb.) megfelelő mennyiségű és minőségű füstérzékelő és tűzjelző készüléket szükséges biztosítani. Az érzékelő és riasztó rendszereken túl biztosítani kell a helyszíni oltáshoz szükséges eszközöket. |

|  | – A szerverszobában tárolt biztonsági mentéseket tartalmazó adathordozók és dokumentáció tűz- és vagyonvédett tárolását is biztosítani kell. Arra is figyelmet kell fordítani, hogy esetleges oltás esetén se sérüljenek. |

|  | – Ki kell dolgozni a tűzvész esetére a szükséges intézkedéseket, melyeket tűz esetén felül kell vizsgálni. |

| Eredmény: | Megfelelő tűzvédelemmel ellátott eszközök, illetve helyiségek. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | 2 évente, de minden rendszer indításakor, minden új helyiség igénybevétele esetén, valamint tűzeset után. |

| Tűzjelző készülékek rendszeres ellenőrzése |

| Feladat: | – A tűzjelző, illetve füstértékelő készülékeket rendszeresen ellenőrizni szükséges. Ezek közé beleértendő nemcsak a helyiségek tűzvédelmét biztosító eszközök, de a számítógépes szekrények érzékelői is. |

| Eredmény: | Működőképes tűzjelző készülékek. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Félévente, illetve riasztás után. |

## 2.2.7. Vízvédelem

| Vízvédelem |

| Feladat: | – A szomszédos helyiségekben, illetve az eszközökhöz közel levő falakban történt csőtörés miatt érheti víz az EKG eszközeit. Mivel vízérzékelővel jelenleg nem minden az EKG működtetését szolgáló helyiség rendelkezik, ezért biztosítani kell, hogy ilyen helyiségben az eszközök ne legyenek vízvezeték közelében. |

|  | – Vízveszély olyan esetben is előfordulhat, amennyiben árvíz fenyegeti az épületet. Amennyiben az EKG eszközeit biztosító eszközök árvízveszélyes helyen vannak (egyes vidéki központokban előfordulhat), úgy gondoskodni kell arról, hogy az eszközök áthelyezhetőek legyenek olyan szintre, ahol az árvíz már nem okoz problémát. |

| Eredmény: | Vízveszélytől védett EKG-eszközök. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | A „vízbiztos” helyszínek kijelölését a rendszer telepítésekor, illetve konkrét intézkedéseket vízveszély esetén szükséges megtenni. |

| Vízvédelmet támogató készülékek rendszeres ellenőrzése és karbantartása |

| Feladat: | – Amennyiben rendelkezik egy helyiség vagy eszköz vízérzékelő készülékkel (javasolt), akkor ezeket a készülékeket rendszeresen kell ellenőrizni, és rajtuk szükség esetén a megfelelő karbantartási munkálatokat végezni. |

| Eredmény: | Működőképes vízvédelmet támogató készülékek. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Félévente, illetve riasztás után. |

## 2.3. Hardver eszközök

## Ebben a fejezetben találhatók mindazok a feladatok és intézkedések, melyek az EKG hardver eszközeire vonatkoznak, illetve azok védelmét szolgálják.

## 2.3.1. Szerverek

| Szerverek üzembe helyezése |

| Feladat: | – A szerverek üzembe helyezését meg kell előznie az installálás utáni tesztelésnek, melyek eredményéről jegyzőkönyvet kell írni. Amennyiben a szerver üzembe helyezése csere okán történik, úgy tesztelni kell, hogy a biztonsági mentésből visszaállított programok, fájlok elérhetők-e. |

|  | – A tesztelési jegyzőkönyveket a szerver üzemből való kivonása után legalább még 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

| Eredmény: | Működőképes új szerverek. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Új szerver beüzemelése esetén. |

| Szerverek karbantartása |

| Feladat: | – A szerverek karbantartását és javítását az üzemeltető felügyeli. |

|  | – Hiba esetén az üzemeltető a tartalékokból biztosít készüléket, majd a szerver szállítójával javíttatja a meghibásodott hardvert. |

|  | – A szállítókkal kötött szerződésekben mindenképp szerepelnie kell a hardverjavítások időintervallumára vonatkozó megállapodásnak, illetve a tartalékeszközök biztosításáról szóló garanciának (A szállító vállalja a 12 órán belüli hibajavítást, vagy tartalék eszközt kell biztosítani, amelyet 12 órán belül az üzemeltetőnek képes kell lenni konfigurálni és telepíteni). |

|  | – Folyamatosan vizsgálni kell, hogy az újabb kiadású szoftverek (operációs rendszer, biztonsági szoftverek stb.) futnak-e a szerveren. Amennyiben nem, úgy csere lehet szükséges (lásd Szerverek cseréje). |

| Eredmény: | Hiba esetén a szerverek gyors helyreállítása. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

| Szerverek cseréje |

| Feladat: | – Az amortizáció nyomán a régi szervereket ki kell cserélni, hogy a korszerűbb operációs rendszerek, védelmi programok, illetve egyéb szoftverek megfelelően futhassanak rajtuk. Ennek megfelelően a hardverekből kell tartalék. A szerverek cseréjét az üzemeltető kell javasolja írásban, amit a kormányzati célú hírközlési szolgáltató bírál el. |

|  | – A régi szervereken levő tartalomról biztonsági mentést kell készíteni. |

|  | – A kiselejtezett szerverek adattárolóin szereplő adatok megsemmisítéséről minden esetben gondoskodni kell, függetlenül az adatok esetleges minősítésétől. |

| Eredmény: | Korszerű hardverek, melyeken az újabb fejlesztésű szoftverek is megfelelően futnak. |

| Felelős: | Szervercsere időben történő igénylése és indokolása: üzemeltető; Szervercseréről döntés: kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Üzemeltető javaslata alapján. |

## 2.3.2. Munkaállomások

| Munkaállomásokra vonatkozó korlátozások |

| Feladat: | – A munkaállomások jogosultságait az üzemeltetéshez szükséges mértékre kell korlátozni, hogy az azokat ért támadások minél kevesebb eséllyel következzenek be. |

|  | – Tiltani szükséges mindenféle program öncélú telepítését. Szoftvert csak a rendszergazda telepíthessen a gépekre, az üzemeltető ezért felelős munkatársának jóváhagyása után. |

|  | – A munkaállomások vírusvédelmét üzemeltetői szinten központilag kell megoldani. |

|  | – Azokra a munkaállomásokra, amit egy felhasználó használ csak, kizárólag az adminisztrátornak és a felhasználónak legyen belépési jogosultsága. |

| Eredmény: | Jól ellenőrizhető munkaállomások. |

| Felelős: | Üzemeltető, csatlakozott szervezetek |

| Gyakoriság: | Új munkaállomás implementálásakor. |

## 2.3.3. Hálózati hardver eszközök

| Hálózati hardver eszközök üzembe helyezése |

| Feladat: | – Hálózati eszköz üzembe helyezése esetén az eszközt tesztelni kell, és az eredményről jegyzőkönyvet szükséges felvenni. Biztosítani kell, hogy az új eszköz esetleges működésképtelensége esetén legyen olyan meleg tartalék, amelyik ellátja az eszköz funkcióit. |

|  | – A tesztelési jegyzőkönyveket az eszköz üzemből való kivonása után legalább még 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

| Eredmény: | Működőképes hálózati hardver eszközök. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Új hálózati eszköz beüzemelésekor. |

| Hálózati hardver eszközök karbantartása |

| Feladat: | – A hálózati hardver eszközök karbantartását és javítását az üzemeltető felügyeli. |

|  | – Hiba esetén az üzemeltető a tartalékokból biztosít készüléket, majd a hálózati eszköz szállítójával javíttatja a meghibásodott eszközt. |

|  | – A szállítókkal kötött szerződéseknek mindenképp tartalmazniuk kell a hálózati eszközjavítások időintervallumára vonatkozó megállapodást, illetve a tartalékeszközök biztosítására vonatkozó kötöttségeket (pl. a szállító vállalja a 12 órán belüli hibajavítást, vagy tartalékeszközt kell biztosítani, amelyet 12 órán belül az üzemeltetőnek képes kell lenni konfigurálni és telepíteni). |

| Eredmény: | Hiba esetén a hálózati eszközök gyors helyreállítása, illetve rendszeres karbantartása. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

| Hálózati hardver eszközök cseréje |

| Feladat: | – A hálózati eszköz cseréjét az üzemeltető kell javasolja írásban, amit a kormányzati célú hírközlési szolgáltató bírál el. Ezen túlmenően a kormányzati célú hírközlési szolgáltató is utasíthatja írásban az üzemeltetőt az eszköz cseréjére. |

|  | – A javításra külső szervezetnek átadott, illetve leselejtezett hálózati eszközök nem tartalmazhatnak konfigurációs információt. |

|  | – A csere céljára használt új eszközt előzetesen tesztelni szükséges. |

|  | – A lecserélt eszköz a körülményektől függően kerülhet selejtezésre, de képezhet tartalékot is. |

| Eredmény: | Működőképes hálózati hardver eszközök. |

| Felelős: | Hálózati hardver eszköz cseréjének időben történő jelzése és indoklása: üzemeltető; Eszközcseréről döntés: kormányzati célú hírközlési szolgáltató. |

| Gyakoriság: | Üzemeltető javaslata alapján. |

## 2.3.4. A csatlakozott intézmények által üzemeltetett eszközök

| Csatlakozott intézmények által üzemeltetett eszközök |

| Feladat: | – A csatlakozott szervezetek által üzemeltetett hálózati eszközök rendelkezésre állása az adott intézmény felelőssége, ilyen esetben az üzemeltetőt semmilyen kötelezettség sem terheli. |

|  | – A csatlakozott intézménytől elvárható, hogy gondoskodjon az adott eszköz folyamatos és zavartalan üzemeléséhez szükséges körülményekről (pl. folyamatos áramellátás, klimatizálás stb.). |

|  | – Az elektronikus közszolgáltatást nyújtó szervezet köteles gondoskodni az általa üzemeltetett eszköz védelméről (pl. illetéktelen hozzáféréstől, lopástól és manipulációtól való védelem). |

| Eredmény: | Az elektronikus közszolgáltatást nyújtó szervezetek által üzemeltetett eszközökből eredő biztonsági kockázat csökkenése. |

| Felelős: | Csatlakozott szervezet |

| Gyakoriság: | Folyamatosan. |

| Csatlakozott intézmények által üzemeltetett eszközökkel kapcsolatos hibák |

| Feladat: | – Az elektronikus közszolgáltatást nyújtó szervezetek kötelesek az általuk üzemeltetett EKG-hoz kapcsolt eszközökkel kapcsolatos bárminemű hibáról az üzemeltetőt haladéktalanul értesíteni. |

|  | – A hibák javítása az elektronikus közszolgáltatást nyújtó szervezet feladata, de a hiba igazolt kijavításáig a hiba természetétől függően a hálózatgazdának joga van az üzemeltetővel az adott szervezet hálózati kapcsolatát lezáratni. |

| Eredmény: | Az elektronikus közszolgáltatást nyújtó szervezetek által üzemeltetett eszközökből eredő biztonsági kockázat csökkenése. |

| Felelős: | Csatlakozott szervezet |

| Gyakoriság: | Csatlakozott szervezetek által üzemeltetett eszközök hibája esetén. |

| Csatlakozott intézmények által üzemeltetett eszközökkel kapcsolatos változások |

| Feladat: | – Az elektronikus közszolgáltatást nyújtó szervezetek az általuk üzemeltetett EKG-hoz kapcsolt eszközökről, az azokkal kapcsolatos bármilyen változásról kötelesek az üzemeltetőt haladéktalanul tájékoztatni. |

|  | – Aktív hálózati hardver elemek esetén az elektronikus közszolgáltatást nyújtó szervezet még a változtatás előtt köteles a tervezett változtatást bejelenteni, és arról az üzemeltető véleményét kérni. |

| Eredmény: | A csatlakozott szervezetek által üzemeltetett eszközökből eredő biztonsági kockázat csökkenése. |

| Felelős: | Csatlakozott szervezet |

| Gyakoriság: | Csatlakozáskor teljes eszközlistáról tájékoztatás, ezt követően változás esetén. |

## 2.3.5. Hardver eszközök nyilvántartása

| Hardvernyilvántartás |

| Feladat: | – Az üzemeltetőnek az összes EKG hardver eszközről (szerverek, munkaállomások, hálózati eszközök, valamint egyéb elektronikus eszközök) részletes nyilvántartást kell készítenie. |

|  | – A nyilvántartást biztonságos helyen kell tárolni, melyhez csak megfelelő jogosultsággal férhet hozzá bárki. Gondoskodni kell arról, hogy az aktuális nyilvántartásról mindig legyen biztonsági másolat, melyet az eredetitől elszeparáltan, szintén biztonságos helyen, lopástól és manipulációtól védetten tárolnak. |

|  | – A hardvernyilvántartás alapján kell történjen a szükséges tartalék eszközök számszerűsítése. |

|  | – A nyilvántartásban dokumentálni kell a tervezett eszközbeszerzéseket is. |

| Eredmény: | Pontos hardvernyilvántartás, mely alapján a tartalékképzés tervezhető. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

## 2.3.6. Tartalék eszközök

| Tartalékolási osztályokba sorolás |

| Feladat: | – Az EKG eszközöket az alábbi tartalékolási osztályokba kell sorolni: |

|  | Általános eszközök (normális mennyiségű – lásd köv. pont – tartalék szükséges); üzemeltetés szempontjából kiemelt eszközök (dupla mennyiségű tartalék szükséges) |

| Eredmény: | Eszközök tartalékolási osztályokba sorolása, amely alapján tervezhető a tartalékképzés. |

| Felelős: | Üzemeltető |

| Gyakoriság: | IBSZ érvénybe lépésekor, utána tapasztalatok alapján átsorolni. |

| Tartalékképzés |

| Feladat: | – A tartalékképzés a folyamatos üzemeltetés egyik legfontosabb feladata, ennek megfelelően fokozott figyelmet igényel. |

|  | – Alapvető szabály, hogy minden EKG-üzemelést biztosító eszközből legyen megfelelő mennyiségű tartalék; és azok üzemképességét folyamatosan kell ellenőrizni. Eszközök, amelyekből tartalékot kell biztosítani: Szerverek, Munkaállomások, hálózati hardver eszközök (switchek, routerek, tűzfalak, hub-ok stb.), Egyéb elektronikus eszközök (UPS, klíma, UPS-akkumulátorok stb.), Egyéb alkatrészek (pl. porszűrő szivacs stb.) |

|  | – Az általános eszközökből megközelítőleg 5–20%-nyi tartalék szükséges (pl. 10 munkaállomás esetén 1 vagy 2 tartalék munkaállomás). |

|  | – Az üzemeltetés szempontjából lényeges elemekre megközelítőleg dupla ennyi tartalék (kb. 20–40%) szükséges (pl. 5 router esetén 1 vagy 2 tartalék router). |

|  | – A tartalékképzésre történő szabály bizonyos esetekben változtatható, a 20% durva becslés. Jelenleg a hálózati eszközökre az alábbi tartalékolási szabály létezik: |

|  | =   1– 10 darab létezik az eszközből: 1 tartalék eszköz; |

|  |  | =  11– 30: | 2 tartalék eszköz; |

|  |  | =  31– 60: | 3 tartalék eszköz; |

|  |  | =  61–100: | 4 tartalék eszköz; |

|  |  | = 100–: | 5 tartalék eszköz. |

|  | – Javasolt megoldás a tartalékok előre történő beszerzésére az éves gazdálkodási terv kialakítása. |

| Eredmény: | Megfelelő mennyiségű tartalék, mely meghibásodás esetén is biztosítja az EKG üzemelését. |

| Felelős: | Tartalékképzésért és tartalékok időben történő igényléséért: üzemeltető; Tartalékok beszerzéséért: kormányzati célú hírközlési szolgáltató. |

| Gyakoriság: | Folyamatosan. |

## 2.4. Szoftverek

## Ez a fejezet tartalmazza az EKG-ban használt szoftverekre vonatkozó, illetve azok védelmét szolgáló feladatokat.

## 2.4.1. Szoftverkarbantartás

| Szoftverek biztonsági frissítéseinek nyomon követése és alkalmazása |

| Feladat: | – Az üzemeltető köteles az EKG eszközein használt szoftverek frissítéseit figyelemmel kísérni, és a csatlakoztatott intézmények figyelmét felhívni, illetve azok további működését a szoftverfrissítés után is biztosítani. |

|  | – A szoftverfrissítéseket (update-ek, service pack-ok) a várható biztonsági hatásuk (pl. kritikus biztonsági probléma javítása stb.) alapján értékelni kell, majd ennek alapján ütemtervet kell meghatározni a bevezetésükre, amennyiben erre tényleg sor kerül. Az ütemtervben meghatározott határidőknek tükrözniük kell a frissítés fontosságát. |

|  | – Minden használt szoftverre (és azok minden egyes üzemben lévő verzióira) az üzemeltetőnek rendelkeznie kell kidolgozott teszttervekkel. |

|  | – Minden frissítést az éles rendszeren való telepítés előtt a kidolgozott tesztterveknek megfelelően tesztelni kell. A tesztelés eredménye alapján kell a telepítésre vonatkozó döntést meghozni. |

|  | – Amennyiben a tesztelés után a telepítés végrehajtását jóváhagyó döntés születik, úgy a megfelelő frissítést a korábban kidolgozott ütemterv szerint telepíteni kell (kritikus frissítés esetén ennek haladéktalanul meg kell történnie). |

|  | – A szállítókkal kötött szerződésekben mindenképp szerepelnie kell a szoftverfrissítések rendelkezésre állásának, ezzel is biztosítva a szoftverek naprakészségét. |

| Eredmény: | Biztonsági szempontból naprakész szoftverek. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Minden szoftverfrissítés megjelenésekor. |

| Szoftverek újabb verzióinak nyomon követése és alkalmazása |

| Feladat: | – Az üzemeltető köteles figyelemmel kísérni az EKG üzemeltetésében használt szoftverek újabb verzióinak megjelenését. |

|  | – Új verzió esetén elemezni kell a verzióváltás hatásait (pl. direkt és indirekt költségek, biztonsági szint változása, használhatóság javulása stb.). Az elemzés eredményét dokumentálni kell. Az elemzést lehetőség szerint az új verzió tesztelésével is meg kell támogatni (csak akkor hagyható ki, ha az új verzió nem elérhető, de ebben az esetben az átállási döntésnél figyelembe kell venni a tesztelés hiányából fakadó kockázatokat). |

|  | – Az elemzés eredménye alapján döntést kell hozni a verzióváltás szükségességéről, és pozitív döntés esetén meg kell határozni az átállás ütemezését. |

|  | – A kidolgozott ütemezésnek megfelelően el kell végezni a verzióváltást. |

|  | – Az üzemeltetőnek törekednie kell arra, hogy a használt szoftverek a lehető legnagyobb mértékben egységesek legyenek. |

|  | – A szállítókkal kötött szerződésekben lehetőség szerint szerepelnie kell a szoftverek verziókövetésének, ezzel is segítve a verzióváltások végrehajtását. |

| Eredmény: | A lehetőségekhez igazodó, korszerű szoftverpark. |

| Felelős: | Üzemeltető |

| Gyakoriság: | A használt szoftverek újabb verzióinak megjelenésekor. |

| Szoftverek üzemeltetői környezetének folyamatos ellenőrzése és karbantartása |

| Feladat: | – Az üzemeltetőnek folyamatosan ellenőriznie kell, hogy minden az EKG üzemeltetésében használt szoftver üzemeltetési feltételei megvannak-e (pl. szükséges memóriamennyiség, szükséges tárterület, naplóállományok számára elegendő tárhely stb.), és mennyire térnek el az optimálistól. |

|  | – Amennyiben valamely feltétel nem teljesül, úgy haladéktalanul meg kell kezdeni ennek javítását. |

|  | – Időszakosan (hetente, de legalább kéthetente) gondoskodni kell arról (tárhelyek felszabadítása, megfelelő adatok archiválása stb.), hogy a szükséges környezeti feltételek normális üzemmenet esetén a következő időszakra teljesüljenek. |

| Eredmény: | A szoftverek üzembiztonságának fenntartása. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Ellenőrzés folyamatosan, karbantartás szükség esetén, de legalább kéthetente. |

## 2.4.2. Biztonsági mentések

| Biztonsági mentések |

| Feladat: | – Az üzemeltetőnek definiálnia kell minden – az EKG-hoz tartozó – adattartalomra (pl. hálózati komponensek konfigurációs állományai, eszköz- és szoftvernyilvántartások, jogosultság adatbázisok, dokumentációk, felhasználói adatok stb.), hogy kell-e róluk biztonsági másolatokat készíteni és milyen sűrűséggel. Ez alapján el kell készíteni a mentési ütemezéseket, forgatókönyveket és ellenőrző listákat. |

|  | – Az ütemezéseknek megfelelően az üzemeltető köteles a biztonsági mentések elvégzésére. |

|  | – Amennyiben valamilyen biztonsági esemény ezt szükségessé teszi, úgy az üzemeltető köteles a biztonsági mentésekből az utolsó stabil állapotot visszaállítani. |

| Eredmény: | Visszaállítható kritikus adattartalom. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor kidolgozott ütemezésnek megfelelően. |

| Biztonsági mentések tárolása |

| Feladat: | – A biztonsági mentéseknek legalább három példányban kell elkészülniük, melyeket egymástól szeparáltan kell tárolni, lehetőség szerint a két budapesti központból és a vidéki tartalékközpontból elérhető helyeken. |

|  | – Az utolsó 5 biztonsági mentést úgy kell tárolni, hogy azokból a visszaállítás azonnal megkezdhető legyen. |

|  | – A biztonsági mentéseket legalább 2 évig biztonságosan, lopástól, manipulációtól és illetéktelen hozzáféréstől védve kell megőrizni. |

| Eredmény: | Többszörösen védett biztonsági másolatok. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor kidolgozott ütemezésnek megfelelően. |

## 2.4.3. Vírusvédelem

| Az EKG-n forgalmazott adatok vírusszűrése és mentesítése |

| Feladat: | – Mivel az EKG dedikáltan átviteli közeg, ezért sem a hálózatgazdának, sem az üzemeltetőnek nincs jogalapja az adatok tartalmába való betekintésre. Emiatt azok vírusszűrését és mentesítését nem végezheti el. |

|  | – A fentiek miatt minden csatlakozott szervezet köteles gondoskodni a hozzá tartozó adatok vírusvédelméről, és az ilyen jellegű károkért minden esetben az azt okozó (a nem megfelelő védelemről gondoskodó) intézmény felel. |

| Eredmény: | Vírusmentesített adatok. |

| Felelős: | Csatlakozott szervezetek |

| Gyakoriság: | Folyamatosan. |

| EKG-ra csatlakozott számítógépek vírusvédelme |

| Feladat: | – Az EKG minden szerverén (ahol ilyen megoldás elérhető) gondoskodni kell a folyamatos vírusvédelemről. Ez kiemelten érvényes a Microsoft által forgalmazott operációs rendszereket futtató gépekre. |

|  | – Minden az EKG-hoz csatlakozott munkaállomáson és szerveren (ahol ilyen megoldás elérhető) gondoskodni kell a vírusvédelemről, ez kiemelten érvényes egyrészt a Microsoft operációs rendszerekre, másrészt azokra a gépekre, amelyekről a hálózat menedzsmentje, üzemeltetése folyik. |

| Eredmény: | Vírusvédett eszközök. |

| Felelős: | Üzemeltető, csatlakozott/csatlakozandó szervezetek |

| Gyakoriság: | Szerverek, munkaállomások üzembe helyezésekor és utána folyamatosan. |

| A vírusvédelmi eszközök karbantartása |

| Feladat: | – Minden az EKG-hoz csatlakozott szerver vagy munkaállomás üzemeltetője (ez vagy a hálózat üzemeltetője, vagy a csatlakozott szervezet) köteles gondoskodni a telepített vírusvédelmi eszközök folyamatos karbantartásáról. |

|  | – Folyamatosan figyelemmel kell kísérni a vírusvédelmi eszközhöz megjelenő frissítéseket (pl. vírus adatbázis aktualizálás) és azokat haladéktalanul telepíteni kell. |

|  | – Folyamatosan figyelemmel kell kísérni a vírusvédelmi eszköz újabb verzióinak megjelenését. Új verzió esetén elemezni kell, hogy a verzióváltás milyen hatással járna, el kell dönteni, hogy kell-e verziót váltani, és amennyiben igen, úgy előre kidolgozott ütemterv szerint végre kell hajtani. |

|  | – A vírusvédelmi eszközök szállítóival kötött szerződésben ki kell kötni, hogy frissítések megjelenése esetén a szállító azt nyomban rendelkezésre bocsátja. |

| Eredmény: | Naprakész vírusvédelmi eszközök. |

| Felelős: | Üzemeltető, csatlakozott szervezetek |

| Gyakoriság: | Folyamatosan. |

## 2.5. Hálózat védelme

## Alábbiakban azok az intézkedések szerepelnek, melyek nem köthetők egyértelműen a szoftverekhez vagy a hardver eszközökhöz, hanem inkább a hálózat egészének védelmét szolgálják.

## 2.5.1. Rendelkezésre állás biztosítása

| Szolgáltatási szint megállapodások (SLA) |

| Feladat: | – A hálózatgazdának megfelelő szolgáltatási szint megállapodásokat (SLA) kell kötnie az üzemeltetővel és a hálózati kapcsolatokat biztosító távközlési szolgáltatókkal. |

| Eredmény: | Szolgáltatási szint megállapodások (SLA). |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Az üzemeltetési szerződés, illetve a szolgáltatási szerződések megkötésekor, megújításakor. |

| Hálózati központok |

| Feladat: | – Az EKG üzembiztonságának szempontjából a hálózati központok kiesése jelentheti a legnagyobb problémát, ezért a hálózatgazdának gondoskodnia kell arról, hogy két, gyakorlatilag azonos üzemeltetési képességgel rendelkező hálózati központ legyen. |

|  | – A hálózatgazdának gondoskodnia kell arról is, hogy létezzen olyan vidéki központ, mely ha csökkentett funkcionalitással is, de képes átvenni a hálózat üzemeltetési központjának a szerepét olyan esetben, amikor Budapest nagy területét érintő katasztrófahelyzet következik be. |

|  | – Amennyiben a kormányzati célú hírközlési szolgáltató biztosítja az ehhez szükséges eszközöket és helyiségeket, úgy az üzemeltető feladata a központok megtervezése, kialakítása és üzembe helyezése. |

| Eredmény: | Nagyon megbízható hálózati struktúra. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Az anyagi források rendelkezésre állásától függően. |

| Redundáns hálózati elemek |

| Feladat: | – Az EKG rendelkezésre állási követelményei miatt a hálózat minden elemének redundánsnak kell lennie, nem lehet olyan eszköz vagy hálózati összeköttetés, ami egyedi hibapontnak (single point of failure) minősül. |

|  | – A redundancia mértékét a szerint kell megválasztani, hogy az adott hálózati elem kiesése a hálózat szolgáltatásának milyen mértékű kiesését veszélyezteti. |

|  | – Lehetőség szerint a redundanciát úgy kell kialakítani, hogy az egymás kiváltására használt eszközök együtt csak nagyon kivételes esetekben sérülhessenek. |

| Eredmény: | Nagyon megbízható hálózati struktúra. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | A hálózati elem üzembe állításakor, illetve a hálózat bővítésekor. |

## 2.5.2. Jogosultsági rendszer

| Jogosultságokra vonatkozó szabályok |

| Feladat: | – A jogosult személyek azonosításának egyértelműnek kell lennie. |

|  | – A jogosultságokat feladatra vonatkozóan kell meghatározni, és amint szükségtelenné válik haladéktalanul vissza kell vonni. |

|  | – Az azonosítást és hitelesítést jelszóval vagy egyéb eszközökkel (smart card, token stb.) kell támogatni. |

|  | – Jelszóhasználat esetén ki kell kötni a jelszavakra vonatkozó szabályokat (minimális hossz, minimális bonyolultság, ciklikusan változó jelszavak kiküszöbölése), és ezeket a jogosultsági rendszernek ki kell kényszerítenie. |

|  | – Szabályozni kell tudni, hogy az egyes eszközökre (pl. router) milyen IP-címekről lehet bejelentkezni. |

|  | – Egyéb azonosítást és hitelesítést támogató eszközök esetén meg kell határozni az azok használatára vonatkozó szabályokat (pl. nem átruházható, elvesztés esetén azonnal jelenteni kell, jelentés hiányában az okozott kárért az adott személyt terheli a felelősség stb.). |

|  | – A szabályokat rendszeresen felül kell vizsgálni és szükség esetén átalakítani. |

| Eredmény: | A jogosultsági rendszer kijátszásából eredő kockázatok csökkenése. |

| Felelős: | Üzemeltető, csatlakozott szervezetek |

| Gyakoriság: | Az informatikai biztonsági szabályzat, illetve a BSZ hatálybalépésével, majd félévente. |

| Jogosult személyek és alkalmazások nyilvántartása |

| Feladat: | – Az üzemeltető köteles a jogosult személyek és alkalmazások nyilvántartására a kapott jogosultságokkal együtt. |

|  | – A nyilvántartásnak naprakésznek kell lennie, minden változást azonnal át kell vezetni. A változásokat naplózni kell, a naplókat legalább 2 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

|  | – Lehetőség szerint minden jogosultságokkal kapcsolatos menedzsment feladatot központilag az üzemeltetőnek kell elvégeznie. |

| Eredmény: | Egyértelmű, naprakész jogosultság-nyilvántartás. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

| Jogosultságok kiadásának és visszavonásának folyamata és szabályai |

| Feladat: | – Jogosultságok kiadására és visszavonására a kormányzati célú hírközlési szolgáltató jogosult, melyet utasítására az üzemeltető végez el, csatlakozott intézményeknek bármilyen ezzel kapcsolatos igényüket írásban kell jelezniük. |

|  | – Jogosultságkérés esetén minden esetben meg kell vizsgálni annak indokoltságát, és ennek eredménye alapján kell meghozni az engedélyezési döntést. |

|  | – Minden a hálózatban valamilyen szereppel bíró intézmény (csatlakozott intézmények, üzemeltető) haladéktalanul köteles tájékoztatni a hálózatgazdát, ha valamely személy vagy alkalmazás bármilyen jogosultságát vissza kell vonni (pl. dolgozó kilép, új munkakörbe kerül, alkalmazást lecserélik stb.). Ilyen esetben a kormányzati célú hírközlési szolgáltató köteles azonnal intézkedni. |

| Eredmény: | Ellenőrzött jogosultság kiadás és visszavonás. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető, csatlakozott intézmény |

| Gyakoriság: | Jogosultsági igény felléptekor vagy megszűnésekor. |

| Jogosultságok felülvizsgálata |

| Feladat: | – Az üzemeltető köteles a jogosultságokat negyedévente felülvizsgálni, és mindazokat a jogosultságokat megszüntetni, melyek már nem indokoltak. |

|  | – Jogosultság felülvizsgálat alapján történő megvonásáról az adott intézményt előzetesen írásban kell tájékoztatni. |

| Eredmény: | Naprakész, indokolt jogosultságok. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Negyedévente. |

| Azonosítási és hitelesítési kísérletek naplózása |

| Feladat: | – Mind a sikeres, mind a sikertelen azonosítási és hitelesítési kísérleteket naplózni kell. |

|  | – A naplófájlok 3 hónap elteltével archiválhatók, de az archivált állományokat legalább 2 évig biztonságosan, lopás és manipulációtól védve meg kell őrizni. |

|  | – A rendszerben lévő naplóállományokhoz csak adminisztrátori jogosultsággal rendelkező személyek, illetve a biztonsági felügyelők férhetnek hozzá. |

|  | – A naplófájlokat rendszeresen, legalább naponta fel kell dolgozni (ezt a tevékenységet mindenképpen érdemes megfelelő automatikus eszközökkel segíteni), és amennyiben szükséges, úgy haladéktalanul intézkedni kell a jogosultságok korlátozásáról, visszavonásáról vagy a rendszer biztonságának fokozásáról. |

| Eredmény: | Ismert és minden jogosult által elfogadott eljárásrend. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor, majd ezt követően évente felülvizsgálva. |

| Eredménytelen azonosítás, illetve hitelesítés esetén elvégzendő intézkedések rögzítése |

| Feladat: | – Meg kell határozni, hogy eredménytelen azonosítás, illetve hitelesítés esetén milyen eljárásrendet kell követni (pl. érvénytelen jelszó vagy felhasználói név beírása után maximum háromszor újra próbálkozhat, ha harmadikra sem sikerül, akkor fél órára zárolódnak a jogosultságai és a rendszer üzenetet küld az adminisztrátornak). |

|  | – Az eljárásrendet írásban kell rögzíteni és minden jogosultsággal rendelkező személynek vagy alkalmazás felelősének alkalmaznia kell, ellenkező esetben elveszíti a jogosultságait. |

|  | – Az eljárásrendet évente felül kell vizsgálni és szükség esetén módosítani. |

| Eredmény: | Ismert és minden jogosult által elfogadott eljárásrend. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Az informatikai biztonsági szabályzat hatálybalépésekor, majd ezt követően évente felülvizsgálva. |

## 2.5.3. MPLS VPN

| VPN-csoportok kialakítása |

| Feladat: | – Az EKG tagjai közötti biztonságos és garantált sávszélességű kommunikáció miatt a hálózatban VPN-kapcsolatokat szükséges kiépíteni. Az intézményeket kapcsolatok jellegétől függően csoportokba javasolt bontani. A VPN-csoportokat meg kell határozni, és a már csatlakozott intézményeket be kell sorolni ezekbe a kategóriákba. |

|  | – Meg kell oldani, hogy egy intézmény több VPN-csoportba is tartozhasson. |

|  | – Ki kell dolgozni a VPN-használat szabályzatát, amely garantálja, hogy több csoportba is tartozó felhasználó révén az érintett VPN-csoportok nem válnak eggyé. A szabályzatot minden érintetthez el kell juttatni. |

| Eredmény: | Biztonságos, VPN-en keresztül történő kommunikáció. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | VPN-ek kialakítása előtt. |

| Csatlakozó intézmények VPN-csoportba való besorolása, átsorolása |

| Feladat: | – Az újonnan csatlakozó intézmények valamelyik VPN-csoportba történő besorolása. |

|  | – A már csatlakozott intézmény kérésére más VPN-csoportba történő átsorolása, illetve hozzáadása. |

| Eredmény: | Biztonságos, VPN-en keresztül történő kommunikáció. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Csatlakozáskor, illetve intézmény igénye esetén. |

| Egy VPN-csoport kiesése nem érintheti más VPN-csoport működését |

| Feladat: | – Amennyiben valamelyik VPN-csoport tevékenységét korlátozni kell (pl. az adott VPN-csoportba tartozó intézmények valamelyikét célzott spam támadás éri), úgy gondoskodni kell arról, hogy ez a többi csoport működését csak a lehető legkevésbé zavarja. |

| Eredmény: | Biztonságosan szeparált és egymástól független VPN-ek. |

| Felelős: | Üzemeltető |

| Gyakoriság: | VPN-csoport működésképtelensége vagy korlátozásának szükségessége esetén. |

| Külső VPN-kapcsolatok engedélyezésének vizsgálata |

| Feladat: | – Az üzemeltetés alatt nagy valószínűséggel előfordulnak olyan esetek a jövőben, hogy az EKG-hoz csatlakozott intézmény külső, nem EKG-s IP-címmel kíván VPN-kapcsolatot nyitni. Ilyen esetben erre az adott intézménynek írásban kell engedélyt kérnie a hálózatgazdától, akinek az üzemeltető segítségével meg kell vizsgálnia az adott kapcsolat veszélyeit. A kockázati szint figyelembevételével kell az engedélyezési döntést meghozni. |

|  | – Engedélyezése esetén az érintett intézménytől igényelni kell a kapcsolat logolását, a logok archiválását és az üzemeltetőnek való átadását. |

|  | – Az üzemeltető köteles a kapott log fájlokat rendszeresen auditálni és az üzembiztonságot veszélyeztető esemény esetén a kapcsolatot azonnal lezárni. |

|  | – Ilyen kapcsolatból származó kár esetén a felelősség a kapcsolatot igénylő intézményt terheli. |

| Eredmény: | Az intézmény oldaláról logolt kapcsolat, melyet az igénylési adminisztráció és a felelősség miatt valószínűleg megfontoltabban kér az intézmény. |

| Felelős: | Kormányzati célú hírközlési szolgáltató az engedélyezésért, üzemeltető a felügyeletért |

| Gyakoriság: | Külső VPN-kapcsolat igénylése esetén. |

## 2.5.4. IP VPN

| IP VPN-ek használata |

| Feladat: | – A csatlakozott szervezeteknek ajánlott IP VPN-ek kialakítása, mellyel saját tevékenységüket is még biztonságosabbá tehetik. |

|  | – IP VPN-ek kódolt adatcsomagjainak kicsomagolására az EKG határvédelmi tűzfalán nincs lehetőség, így azok szűréséről a csatlakozott szervezeteknek kell gondoskodniuk. Ezért minden ebből eredő kár az adott intézményt terheli. |

| Eredmény: | Intézményi IP VPN-ek. |

| Felelős: | Csatlakozott szervezetek |

| Gyakoriság: | Csatlakozáskor vagy erre vonatkozó igény esetén. |

## 2.5.5. Tűzfalakra, védelmi intézkedésekre vonatkozó követelmények

| Határvédelmi tűzfalak felállítása |

| Feladat: | – Az EKG üzembiztonsága megköveteli, hogy hálózati forgalmának zavartalanságát többszintű határvédelmi (a gerinchálózat az internet felé való védelme, amely az üzembiztonságot védi, de a rajta átfolyó adatmennyiség adatbiztonságáért már nem felel) tűzfalrendszer védje. |

|  | – A felállítandó tűzfalrendszer megtervezéséről, méretezéséről, felállításáról és karbantartásáról az üzemeltetőnek kell gondoskodnia. |

| Eredmény: | Az EKG tűzfalakkal védett működése. |

| Felelős: | Üzemeltető |

| Gyakoriság: | A hálózat kiépítésekor. |

| Tűzfalak felügyelete és karbantartása |

| Feladat: | – Az üzemeltetőnek gondoskodnia kell a tűzfalak zavartalan üzemeléséről. |

|  | – A tűzfalak konfigurációját időszakosan felül kell vizsgálni, és szükség esetén el kell végezni a megfelelő változtatásokat. A változtatást minden esetben dokumentálni kell, megadva az okot és tényleges változásokat. A jegyzőkönyvet legalább 2 évig biztonságosan, lopástól és manipulációtól védetten meg kell őrizni. |

|  | – A tűzfalak szállítóival kötött szerződésben ki kell kötni, hogy bármely, a tűzfalakat érintő, nem az üzemeltetésből fakadó hiba esetén köteles annak haladéktalan elhárítására. |

|  | – A tűzfalaknak minden kapcsolatot naplózniuk kell, a naplófájlokat archiválni kell és legalább 2 évig biztonságosan, lopástól és manipulációtól védetten meg kell őrizni. |

|  | – A tűzfalak naplófájljait az üzemeltetőnek folyamatosan auditálnia kell. |

| Eredmény: | Naprakész, felügyelt tűzfalrendszer. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Felülvizsgálat negyedévente, illetve betörés esetén; naplófájlok auditja legalább hetente. |

| Intézmény adott portjának megnyitása |

| Feladat: | – Amennyiben valamilyen csatlakozott intézmény tevékenységéhez a tűzfalon egy új portot akar megnyittatni, úgy azt írásban a hálózatgazdával kell engedélyeztetni. |

|  | – A kormányzati célú hírközlési szolgáltató az üzemeltető segítségével megvizsgálja, hogy a kérvényezett port megnyitása milyen kockázatokat rejt magában. A vizsgálatról írásos jegyzőkönyvet kell készíteni, melyet legalább 2 évig biztonságos helyen, lopástól és manipulációtól védett módon meg kell őrizni. A kockázati szinttől függően engedélyezhető a port megnyitása. |

|  | – Az üzemeltető negyedévente köteles felülvizsgálni a megnyitott portokat. Nem használt vagy veszélyforrást jelentő nyitott portok esetén kezdeményezni kell azok lezárását, amit a kormányzati célú hírközlési szolgáltató hagy jóvá és az üzemeltető végez el. Ilyen esetben előzetesen írásban kell az adott intézményt értesíteni. |

| Eredmény: | Felügyelt és ellenőrzött port megnyitások. |

| Felelős: | Csatlakozott intézmény, kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Port megnyitás kérésekor, illetve a felülvizsgálat negyedévente. |

## 2.5.6. Csatlakozott szervezetekre vonatkozó szabályok

| Csatlakozó intézmény egyéb internetkapcsolatainak megszüntetése |

| Feladat: | – Az EKG egyik legjelentősebb veszélyforrása az, hogy a csatlakozó intézmények oldaláról érkezik támadás – azok internetes hálózatának nem megfelelő védelme miatt. Ezért az EKG-ra történő csatlakozás alapfeltétele (szerződésben rögzítve), hogy a kapcsolódó intézmény az EKG-ra csatlakozó számítógépeivel, illetve az e számítógépekből álló hálózatával nem kapcsolódhat más külső hálózatra. |

|  | – Szerződésben szükséges szabályozni, hogy a csatlakozó intézmény felelős az ő oldaláról okozott támadásokért és károkért, legyen az belső (az intézmény alkalmazottjától érkező) vagy külső (az intézmény egyéb hálózati kapcsolatából eredő) támadás. |

| Eredmény: | Biztonságosan üzemeltethető hálózat. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Csatlakozás esetén. |

| Csatlakozó intézmény routerének felügyelete |

| Feladat: | – A csatlakozó vidéki intézmények nagy száma miatt törekedni kell arra, hogy a csatlakozás minden igényelt kapcsolódási ponton megfelelő router meglétéhez legyen kötve, amelyre az üzemeltetőnek betekintési és menedzselési jogokat kell adni. |

|  | – Ha a csatlakozó szervezet számára a szükséges routereket az EKG bocsátja rendelkezésre, úgy ezek karbantartása és felügyelete teljes mértékben az üzemeltető feladata, az adott intézmény a routerhez semmilyen jogosultsággal nem rendelkezhet. |

| Eredmény: | Üzemeltető felügyelete alatt álló routerek. |

| Felelős: | Felügyeletért az üzemeltető, a betekintési jogok adásáért a kormányzati célú hírközlési szolgáltató. |

| Gyakoriság: | Csatlakozás esetén. |

| Csatlakozó intézmény kapcsolattartóinak megnevezése |

| Feladat: | – A csatlakozó intézményektől a szerződés megkötésekor be kell kérni azokat az adatokat, amelyek meghibásodás esetén lehetnek fontosak az EKG üzemeltetésének szempontjából: |

|  | kapcsolattartók megnevezése (informatikai vezető, illetve technikai szakember), |

|  | amennyiben a kapcsolat EKG kezelésű eszközzel történik (nem valamely szolgáltató biztosítja a kapcsolatot a megyei alközpontig) |

|  | pontosan hol helyezkednek el az EKG-hoz kapcsolódó eszközök, klimatizációs lehetőségek, |

|  | tűzjelző és oltókészülék helye, |

|  | bejutási lehetőségek adminisztrációja. |

|  | – Amennyiben ezek az adatok megváltoznak, úgy az intézménynek tájékoztatási kötelezettsége legyen az üzemeltető felé. |

| Eredmény: | A csatlakozott intézmény főbb – üzemeltetés szempontjából lényeges – adatai. |

| Felelős: | Kormányzati célú hírközlési szolgáltató, üzemeltető |

| Gyakoriság: | Csatlakozás, illetve valamely adat megváltozása esetén. |

## 2.5.7. Hálózat felügyelete

| Hálózati események felügyelete |

| Feladat: | – Az üzemeltető köteles folyamatos (7×24 órás) hálózati felügyeletet biztosítani. |

|  | – A hálózat felügyelete magába foglalja a hálózathoz tartozó minden eszköz (amennyiben erre lehetőség van) folyamatos monitorozását, a különböző hálózati események figyelemmel kísérését (pl. terhelések nyomon követése, esetleges kiesések felismerése stb.), azok naplózását, illetve szükség szerint beavatkozást. |

|  | – A felügyeletet lehetőség szerint a hálózat minél nagyobb részére kiterjedő menedzsment eszközzel kell megtámogatni. |

| Eredmény: | Felügyelt hálózat. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Folyamatosan. |

## 2.5.8. Rendhagyó (rendkívüli) események jelentése, kezelése

| Biztonsági események kezelése |

| Feladat: | – Üzembiztonságot befolyásoló esemény észlelése történhet a hálózat felügyelet által, illetve felhasználói bejelentésre. |

|  | – Mindkét esetben haladéktalanul meg kell kezdeni az esemény hatásainak csökkentését és magának az eseménynek az elemzését. |

|  | – Az elemzés eredményét dokumentálni kell, a jegyzőkönyvet legalább 5 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

|  | – Az elemzés eredményét felhasználva el kell dönteni, hogy milyen módon kell a hálózatba beavatkozni, az esemény kivédéséhez és az okozott kár minimalizálásához. Ennek megfelelően ki kell alakítani egy akciótervet. |

|  | – A kialakított akciótervet végre kell hajtani folyamatosan ellenőrizve, hogy közben a hálózatban nem keletkeznek-e újabb biztonságot befolyásoló események. |

| Eredmény: | Kezelt biztonsági események. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Biztonsági esemény bekövetkeztekor. |

| Incidens menedzsment |

| Feladat: | – Incidensnek minősül bármi, ami arra utal, hogy a hálózat nem üzemszerűen, az elvárt módon működik. |

|  | – Incidens észlelése történhet a hálózat felügyelet által, illetve felhasználói bejelentésre. |

|  | – Mindkét esetben az incidenst az üzemeltető erre a célra használt rendszerében rögzíteni kell az összes felderítést és elhárítást elősegíthető adattal együtt, majd haladéktalanul meg kell kezdeni az esemény hatásainak csökkentését és magának az eseménynek az elemzését. |

|  | – Az elemzés eredményét dokumentálni kell, a jegyzőkönyvet legalább 5 évig biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni. |

|  | – Az elemzés eredményét felhasználva el kell dönteni, hogy milyen módon kell a hálózatba beavatkozni, az esemény kivédéséhez és az okozott kár minimalizálásához. Ennek megfelelően ki kell alakítani egy akciótervet. |

|  | – A kialakított akciótervet végre kell hajtani folyamatosan ellenőrizve, hogy közben a hálózatban nem keletkeznek-e újabb biztonságot befolyásoló események. |

|  | – Az üzemeltető incidens követő rendszerének képesnek kell lennie az incidensek életciklusának nyomon követésére, a korábbi incidensek közötti keresés támogatására, a problémák eszkalálására stb. |

| Eredmény: | Kialakult incidenskezelési folyamat, hálózati problémák gyors, szakszerű megoldása. |

| Felelős: | Üzemeltető |

| Gyakoriság: | Incidens bekövetkeztekor. |

| Nagy felhasználószámú intézmény csatlakozása |

| Feladat: | – Amennyiben nagy felhasználószámú intézmény csatlakozik az EKG-hoz, úgy a kormányzati célú hírközlési szolgáltató értesítse az üzemeltetőt, hogy az fel tudjon készülni a várható terhelésnövekedésre. Ilyen esetben eszközbővítések válhatnak szükségessé. |

| Eredmény: | Nagyobb intézmény csatlakozása sem okoz negatív változást az üzemeltetés biztonságában. |

| Felelős: | Kormányzati célú hírközlési szolgáltató |

| Gyakoriság: | Nagy felhasználószámú intézmény csatlakozásakor. |

## 3. Záró rendelkezések

## 3.1. A biztonsági szabályzat bevezetése, oktatása

## Az üzemeltetői biztonsági szabályzatot hatálybalépése előtt mind a hálózatgazdának, mind az üzemeltetőnek el kell fogadnia. A csatlakozott szervezet biztonsági szabályzatát az EKG biztonsági felelőse véleményezi, és nem megfelelő szabályozás esetén a kormányzati célú hírközlési szolgáltató jogosult a csatlakozást felfüggeszteni a szabályozás (illetve a probléma) korrekciójáig.

## A hatálybalépés előtt minden érintett személyt tájékoztatásban kell részesíteni. Ehhez szerepekre (pl. rendszeradminisztrátorok, hálózati mérnökök stb.) szabott tájékoztató anyagokat célszerű készíteni, ezáltal lehetővé téve, hogy mindenki tisztában legyen a saját feladatának biztonsági vonzataival.

## Mindazok esetében, akik a hálózat üzembiztonságának szempontjából jelentős feladattal (pl. biztonsági vezető, biztonsági felügyelő, rendszeradminisztrátorok, üzemeltetési vezető stb.) bírnak, a tájékoztatást (oktatást) számon kérhető módon kell végrehajtani, és az elsajátított ismeret szintjét ellenőrizni kell.

## A hatálybalépés előtt ki kell dolgozni a biztonsági szabályzat betartásához szükséges feltételek megteremtését célzó akciótervet, pontos feladatokkal, határidőkkel és felelősökkel. Ezt az akciótervet a hatálybalépés előtt (illetve a hatálybalépést követően a kormányzati célú hírközlési szolgáltató által meghatározott türelmi időn belül) végre kell hajtani, amit a hálózatgazdának felügyelnie kell.

## 3.2. A biztonsági szabályzat hatálybalépése

## A biztonsági szabályzat hatálybalépése a csatlakozás időpontja, illetve a korábban csatlakozott szervezetek esetében a jogszabályban meghatározott időpont.

## A csatlakozó szervezet biztonsági szabályzata kizárólag akkor léphet hatályba, ha a végrehajtásához szükséges minden alapfeltétel vagy fennáll, vagy meghatározásra került a teljesítés határideje.

## 3.3. A biztonsági szabályzattól való eltérés rendje

## A biztonsági szabályzattól csak rendkívül indokolt esetben, a kormányzati célú hírközlési szolgáltató jóváhagyásával és előre meghatározott ideig lehet eltérni.

## Amennyiben a szabályzat betartása valami okból nem lehetséges, úgy ezt írásban jelezni kell a kormányzati célú hírközlési szolgáltató felé. A hálózatgazdának ilyen esetben az üzemeltető segítségével meg kell vizsgálnia, hogy a kérés indokolt-e, létezik-e egyéb megoldás, amivel a probléma áthidalható, illetve a kérés jóváhagyása milyen kockázatokat rejt magában. A vizsgálat eredményét írásban dokumentálni kell (a jegyzőkönyvet legalább 5 évig, biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni).

## Amennyiben a vizsgálat alapján a kérést a kormányzati célú hírközlési szolgáltató jóváhagyja, úgy azt is meg kell határoznia, hogy a felmentés meddig állhat fent. Mindezeket jegyzőkönyvezni kell (a jegyzőkönyvet legalább 5 évig, biztonságosan, lopástól és manipulációtól védett módon meg kell őrizni).

## Jóváhagyott szabályzattól való eltérés esetén az érintettek kötelesek ezt az állapotot a meghatározott határidő leteltével megszüntetni.

## A biztonsági szabály véletlen megsértése esetén, annak észlelését követően az érintettek kötelesek tájékoztatni erről a helyzetről a hálózatgazdát, illetve kötelesek haladéktalanul megkezdeni ennek az állapotnak a felszámolását. Amennyiben az EKG üzembiztonsága ezt megköveteli, úgy a szabálysértés megszüntetéséig a hálózatgazdának joga van a hálózat működőképességének fenntartása érdekében az érintettek hálózati kapcsolatát felfüggeszteni.

## 3.4. A biztonsági szabályzat aktualizálásának, kiegészítésének rendje

## A biztonsági szabályzatot (ideértve az IBSz-t is) legalább évente felül kell vizsgálni, és gondoskodni kell szükség szerinti módosításáról, kiegészítéséről.

## A hálózati rendszer jelentős változása esetén a felülvizsgálatot soron kívül el kell végezni.

## A biztonsági szabályzat módosításainak bevezetésére és hatályba léptetésére a 3.1. és a 3.2. alfejezetekben leírtak érvényesek.

## A szabályzat kiegészítésére, módosítására az üzemeltető és a felhasználók közvetlenül tehetnek javaslatot a hálózatgazdának. A kormányzati célú hírközlési szolgáltató a módosítás előtt kikéri az üzemeltető és az informatikai biztonsági felügyelő véleményét.

## Az üzemeltetői biztonsági szabályzat visszavont rendelkezése esetén a hálózatgazdának meg kell határozni a hatályvesztés pontos időpontját, és erről minden érintettet tájékoztatni kell. A visszavont szabályokat archiválni kell, dokumentálva az okokat, a visszavonás kezdeményezőjét és jóváhagyóját, valamint idejét.

## 1. számú függelék

## A dokumentumban használatos (részben EKG-specifikus) alapfogalmak leírása

| Megnevezés | Leírás |

| Hálózatgazda | A közigazgatási informatikáért felelős miniszter, feladatait az infokommunikációért felelős kormánybiztos látja el. |

| Üzemeltető | A hálózatgazdával közszolgáltatási szerződéses viszonyban lévő, a hálózat felügyeletéért és rendelkezésre állásáért felelős szervezet. Külön jogszabály alapján a Kopint-Datorg Zrt. |

| Távközlési szolgáltatók | Mindazok a távközlési szolgáltatók vagy konzorciumok, amelyek az EKG üzemeltetéséhez szükséges infrastruktúrát biztosítják. |

| Csatlakozott intézmény | Mindazok a – jellemzően közigazgatási – intézmények, melyek az EKG valamely szolgáltatását igénybe veszik. |

| Nagy felhasználószámú intézmény | Olyan csatlakozott intézmény, amelyben a munkaállomások száma a 400 darabot meghaladja. |

| ITSEC | Information Technology Security Evaluation Criteria (Információtechnológia Biztonsági Értékelési Kritériumok). |

| UPS | Szünetmentes áramforrás, amely áramkimaradás esetén rövid ideig biztosítja a hozzá kötött eszközök áramellátását. |

| VPN | Virtuális magánhálózat (Virtual Private Network). Használatával a kapcsolódó felek lényegében úgy kommunikálhatnak, külön titkosítás nélkül a nyilvános hálózatokon, mintha külön bérelt, fizikailag elválasztott magánhálózatot hoztak volna létre. |

4. melléklet a 223/2009. (X. 14.) Korm. rendelethez

A központi elektronikus szolgáltató rendszer által nyújtott közszolgáltatások igénybevételének

biztonsági feltételei

1. Általános leírás

1.1. Áttekintés

1.1.1. Szolgáltatás terjedelme

A központi elektronikus szolgáltató rendszer (a továbbiakban: KR vagy központi rendszer) feladata többek között az elektronikus közszolgáltatásról szóló 2009. évi LX. törvényben meghatározott, a központi rendszer azonosítási szolgáltatásait igénybe véve megvalósított elektronikus kapcsolattartás lehetővé tétele azáltal, hogy

–  a központi rendszert igénybe vevő természetes és jogi személyek (a továbbiakban: felhasználók) által előkészített, kitöltött elektronikus űrlapokból – a központi rendszer elektronikus űrlap formátumára vonatkozó szabályoknak megfelelő – üzenetet állít elő;

–  ellenőrzi az elektronikus űrlap formai követelményeknek való megfelelését;

–  a formai követelményeknek megfelelő elektronikus beadványokat érkezteti;

–  az érkeztetés tényét és időpontját bizonyító elektronikus dokumentumot – visszaigazolást – elkészíti és a felhasználó részére kézbesíti;

–  az érkeztetett elektronikus beadványt kézbesíti a címzett elektronikus közszolgáltatást nyújtó vagy abban részt vevő részére olyan eljárással, hogy a szolgáltató a beküldő személyét a jogszabályban meghatározott módon azonosítani tudja;

–  illetve lehetővé teszi a fordított irányú kommunikációt is, ahol biztosítja annak tanúsítását, hogy a címzett átvette-e a neki szóló küldeményt.

A szolgáltatás nem terjed ki

–  a felhasználó, illetve harmadik személy tulajdonát képező, a szolgáltatás igénybevételéhez a felhasználó által használt számítástechnikai eszközökre és szolgáltatásokra, beleértve az internetszolgáltatást is;

–  az elektronikus ügyintézési folyamat – és ezen keresztül a kitöltött elektronikus űrlapok – tartalmi ellenőrzésére, a tartalmi ellenőrzést, érdemi feldolgozást minden esetben a címzett szervezet végzi el.

1.1.1.1. Szolgáltatás személyi hatálya

A szolgáltatást ügyfélkapuval, illetve hivatali (ennek a vállalkozások számára szolgáló változatával a cégkapuval) rendelkező természetes, illetve jogi személyek vagy jogi személyiséggel nem rendelkező, de közhiteles nyilvántartásban szereplő szervezetek vehetik igénybe.

1.1.1.2. Szolgáltatás területi hatálya

A szolgáltatást magyarországi telephelyről nyújtja a központi rendszer működtetője, a Miniszterelnöki Hivatal, a szolgáltatás nyújtásával kapcsolatban a magyar jogszabályok mérvadók. A szolgáltatás igénybevétele területileg nem korlátozott, azonban az 1.1.1. pontban jelzett funkcionális korlátozás e vonatkozásban is érvényes.

1.1.2. Közzététel

Jelen dokumentum a Magyar Közlönyben kerül az elektronikus közszolgáltatás biztonságáról szóló kormányrendelet mellékleteként kihirdetésre, majd a MeH elektronikus úton hozzáférhetővé teszi a http://www.magyarorszag.hu/segitseg internetes címen.

1.1.3. Értelmező rendelkezések

Központi elektronikus szolgáltató rendszer

Az elektronikus közszolgáltatások nyújtásához felhasznált, a kormányzati portálon keresztül elérhető, szolgáltatást, tájékoztatást és egyéb közhasznú szolgáltatásokat nyújtó informatikai rendszerek összessége, beleértve a felhasználók számára hozzáférhetővé tett nyomtatványkitöltő alkalmazást is.

Központi rendszer működtetője – a Miniszterelnöki Hivatal

A központi rendszer által nyújtott szolgáltatásokért jelen dokumentumban meghatározott korlátozásokkal felelősséget vállaló jogi személy.

1.1.4. Kapcsolódó jogszabályok

–  a személyes adatok védelméről és a közérdekű adatok nyilvánosságáról szóló 1992. évi LXIII. törvény (a továbbiakban: Avtv.);

–  a közigazgatási hatósági eljárás és szolgáltatás általános szabályairól szóló 2004. évi CXL. törvény (a továbbiakban: Ket.);

–  Az elektronikus közszolgáltatásról szóló 2009. évi LX. törvény (a továbbiakban: Ekszt.) és végrehajtási rendeletei

–  A hivatalos iratok elektronikus kézbesítéséről és az elektronikus tértivevényről szóló 2009. évi LII. törvény

1.2. Szolgáltatásban részt vevő felek és kötelezettségeik

1.2.1. Miniszterelnöki Hivatal (MeH)

A MeH kötelezettséget vállal arra, hogy mindenkor a jelen dokumentumban meghatározott feltételekkel nyújtja szolgáltatását, különösen tekintettel arra, hogy:

–  a rendszer alapszolgáltatásait az ügyfélkapuval rendelkező ügyfelek térítésmentesen vehetik igénybe;

–  a MeH által felügyelt informatikai rendszerek folyamatos működését és ezáltal a vállalt szolgáltatási szintet a tőle elvárható gondossággal biztosítja;

–  az elektronikus beadványok titkosságát a címzett szervezethez történő beérkezésig biztosítja;

–  a MeH az általában elvárható magatartás szerint szabályzatait betartja, illetve a részt vevő felekkel betartatja.

A MeH az ügyfelekkel való kapcsolattartást központi ügyfélszolgálat (ügyfélvonal) telefonos és internetes és internettelefonos (VoIP) szolgáltatásainak igénybevételével biztosítja.

1.2.2. Felhasználók

A központi rendszer szolgáltatásait igénybe vevő természetes és jogi személyek a biztonságos és zavarmentes ügyintézés érdekében kötelezettséget vállalnak arra, hogy jelen dokumentumot megismerik; a dokumentum, valamint a hatályos jogszabályok a felhasználókra vonatkozó rendelkezéseit betartják; vállalják a felelősséget a felhasználói azonosítójukkal végzett tevékenységekért, különösen az általuk az elektronikus közszolgáltatásokat nyújtó szervezetekhez küldött – a központi rendszer által továbbított – elektronikus üzenetek tartalmáért.

1.2.3. Az elektronikus közszolgáltatást nyújtó szervezetek

A központi rendszerhez jogszabályi kötelezés alapján vagy önkéntesen csatlakozott államigazgatási, önkormányzati vagy más közhatalmi szerv, közüzemi szolgáltató vagy más költségvetési szerv, illetve vállalkozás, amely a központi rendszeren át folytatott kommunikációt a törvényekben rögzített eljárásrend mellett bizonyító erejű kommunikációként kezeli, a központi rendszer által nyújtott azonosítást folyamataiban alkalmazza. Elfogadja a központi rendszer által továbbított elektronikus beadvány beérkezésének időpontját, elvégzi az elektronikus beadvány tartalmi vizsgálatát, ellátja a jogszabályokban és belső szabályzatában meghatározottak szerint az ügyfélkapcsolatot és a felhasználó igénye esetén elektronikusan válaszol a hozzá érkezett üzenetre.

1.2.4. Ügysegéd

Ügysegéd olyan informatikai és/vagy az ügyintézéshez kapcsolódó szakismerettel rendelkező természetes személy, illetve ilyen tevékenységet végző jogi személy vagy jogi személyiséggel nem rendelkező szervezet lehet, amely (aki) az ügyfél megbízásából ügyintézési folyamatokat végez vagy támogatást ad az ügyek intézéséhez, a központi rendszer használatához. A feladatot elláthatja jogszabályban arra feljogosított hatóság is, amely a Ket. 169. § (1) bekezdése alapján ügyfél képviseletében ügyintézést végez, illetőleg internetes kapcsolati lehetőséget biztosít, szakmai és informatikai segítséget nyújt.

Az ügysegéd minden esetben az ügyfél megbízása alapján, az ügyfél igényének megfelelően köteles eljárni. Az ügysegéd köteles az elektronikus ügyintézés során az ügyfél utasításának maradéktalanul megfelelve eljárni, továbbá köteles felhívni ügyfele figyelmét minden tevékenység végrehajtása előtt azokra a problémákra, amelyeket a döntése okozhat. Az ügysegéd az ügyintézés során önállóan a megbízás kereteit túllépve hozott döntésért a Ptk. alapján felel.

Az ügysegéd kötelessége az elektronikus ügyintézés során a jelen dokumentumban az ügyfelekre vonatkozó rendelkezések betartása az általánosan elvárható gondossággal.

2. A szolgáltatás igénybevételének általános szabályai

Az ügyfelek hozzáférés igénylésének és a szolgáltatás használatának szabályait az Ekszt. rögzíti. A szolgáltatás használójának ugyanakkor tekintettel kell arra lennie, hogy az elektronikus beadványok az interneten nem megbízható átviteli közegben, nem garantált szolgáltatási szinten továbbítódnak. Ennek következménye, hogy a központi rendszeren keresztül a szolgáltatás nyújtójához továbbított elektronikus üzenetét csak akkor tekintheti kézbesítettnek, ha a beérkezés tényét a központi rendszer részére visszaigazolta.

2.1. A használat előfeltétele

2.1.1. Ügyfélkapu létesítése

A központi rendszer azonosítást igénylő szolgáltatásait csak ügyfélkapuval rendelkező felhasználó veheti igénybe az ügyfélkapura történő bejelentkezést követően. Az ügyfélkapu létesítésére vonatkozó szabályok részletesen a www.magyarország.hu/ugyfelkapu oldalon érhetők el.

2.1.2. Nyomtatványkitöltő program üzembe helyezése

Az Ekszt 19. § (2) bekezdés b) pontja alapján a rendszer működtetőjének lehetősége van arra, hogy az elektronikus űrlapok és csatolmányaik biztonságos továbbítását lehetővé tevő alkalmazást az ügyfelek rendelkezésére bocsásson. A MeH az elektronikus közszolgáltatást nyújtó szervezetek számára megküldhető elektronikus űrlapok kitöltésére programot bocsát az ügyfelek rendelkezésére, mely

–  alkalmas a címzett szervezetek által kibocsátott vagy általánosabb célú elektronikus űrlapok kitöltésére,

–  elvégzi az elkészített űrlap elsődleges tartalmi ellenőrzését és előkészítését (titkosítását) az elektronikus elküldéshez. Az űrlapot egyébként ki is lehet nyomtatni és postán el lehet küldeni, ahol ezt törvény nem zárja ki,

–  biztosítja az elektronikus beadvány továbbítását a központi rendszer és azon keresztül a címzett szervezet felé.

A felhasználó feladata a www.magyarorszag.hu és a www.apeh.hu honlapról a nyomtatványkitöltő és súgó program aktuális verziójának, szükség esetén további – harmadik személy által készített – programkomponenseknek[^14] letöltése és telepítése a programokhoz mellékelt telepítési útmutató alapján.

Annak érdekében, hogy a felhasználó a nyomtatványkitöltő program sértetlenségéről és épségéről a telepítést megelőzően meggyőződhessen, a program készítője az általános nyomtatványkitöltő program telepítő csomagját elektronikus aláírással látja el, mely tanúsítja, hogy

–  a program a készítőjétől származik,

–  a program nem módosult a közzététel során.

A programot a MeH biztosítja az ügyfelek részére, ugyanakkor a számítógépes szoftverek komplex természetéből adódóan nem garantálja, hogy az átadott szoftver teljesen hibamentesen vagy bárminemű zavar nélkül működik, illetve, hogy minden hardver- és szoftver-konfigurációval kompatibilis. A MeH a szoftverekre vonatkozó általános szavatossági feltételekkel összhangban nem vállal felelősséget a szoftver használatából eredendő esetleges károkért, a használatával kapcsolatos adatvesztésért. Ugyanakkor tömeges, illetve típushibák esetén lehetőségei függvényében biztosítja a javítást a programhoz.

Tekintettel arra, hogy a programot a felhasználó az általa üzemeltetett munkaállomásra telepíti vagy nyilvános internet-hozzáférési ponton veszi használatba (pl. Teleház, internetkávézó, E-pont), a felhasználó feladata a nyomtatványkitöltő alkalmazás megbízható üzemeltetési környezetét biztosítani vagy annak meglétéről meggyőződni, beleértve az általános helyes gyakorlatnak megfelelő vírus- és behatolásvédelmi rendszer működtetését is.

Az általános nyomtatványkitöltő program on-line kapcsolat esetén automatikusan ellenőrzi, hogy újabb verzió mind a programból, mind a feltelepített elektronikus űrlapokból kiadásra került-e, s ha hozzáférhető a program újabb verziója, akkor erről tájékoztatja az ügyfelet. Ha nincs on-line kapcsolat, figyelmezteti az ügyfelet erre a lehetőségre. A felhasználó dönt a frissítés telepítéséről, ugyanakkor a MeH javasolja, hogy a frissítéseket a felhasználó rendszeresen telepítse.

2.2. Használat szabályai

2.2.1. Elektronikus űrlap letöltése, frissítése

A felhasználó az elektronikus közszolgáltatást nyújtó szervezet által készített és hozzá benyújtandó elektronikus űrlap aktuális verzióját a www.magyarorszag.hu honlapról, illetve a címzett szervezet honlapjáról töltheti le és telepítheti. Az űrlapok sértetlenségének ellenőrizhetőségét a kibocsátó biztosítja.

A nyomtatványkitöltő program az elektronikus űrlapok telepítését követően automatikusan ellenőrzi a sértetlenséget és az űrlap sérüléséről tájékoztatja az ügyfelet. Sérült elektronikus űrlapot ne használjon! Ha nem sikerül az űrlapot hibaüzenet nélkül telepíteni, akkor e tényt kérjük, jelezze a központi ügyfélszolgálaton, mely a 189-es hívószámon érhető el.

Tekintettel arra, hogy a hatóságokkal való kommunikációhoz rendszeresített elektronikus űrlapok tartalma, valamint az elektronikus űrlapokhoz kapcsolódó ellenőrzések változhatnak, a www.magyarorszag.hu honlapon mindig az elektronikus közszolgáltatást nyújtó szervezetek által rendszeresített elektronikus űrlapok legújabb változatát publikálja. A nyomtatványkitöltő program a feltöltéseket megelőzően minden esetben megvizsgálja, hogy a használt elektronikus űrlapból létezik-e újabb verzió, amennyiben létezik, erről tájékoztatja az ügyfelet.

A MeH felelőssége ezzel összefüggésben csak az elektronikus űrlapok biztonságos publikálására korlátozódik. Az elektronikus közszolgáltatást nyújtó szervezet jogosult meghatározni, hogy mely verziójú elektronikus űrlapokat fogadja be a felhasználóktól, ezért a MeH javasolja ügyfeleinek, hogy az esetleges kellemetlenségek elkerülése érdekében – ha szükséges – frissítsék az elektronikus űrlapokat és a legújabb verziójú elektronikus űrlapot kitöltve intézzék ügyeiket.

2.2.2. Az elektronikus űrlap kitöltése, a kitöltés ellenőrzése

Az elektronikus űrlapot a felhasználó tölti ki, az űrlapon rögzített adatok helyességéért és pontosságáért a felhasználó vállalja a felelősséget függetlenül attól, hogy a nyomtatványkitöltő program által nyújtott alábbi lehetőségek közül melyiket használja:

–  az elektronikus űrlapok kitöltését egyedileg a nyomtatványkitöltő alkalmazásban;

–  egy megfelelő módon előállított – a címzett szervezet honlapján publikált szintaxisú – XML állományból történő adatbetöltést az elektronikus űrlapra;

–  egyszerre több importállományból történő adatbetöltést egy-egy elektronikus űrlapra;

–  közvetlenül a nyomtatványkitöltő program XML kimeneti állományának előállítására szolgáló más – a felhasználó vagy általa megbízott harmadik személy által fejlesztett – alkalmazással úgy, hogy a kimeneti állomány formai, logikai ellenőrzése történik csak a nyomtatványkitöltő programmal.

Abban az esetben, ha a felhasználó problémát észlel az űrlap kitöltése vagy tartalmi ellenőrzése során, kérjük ezt közvetlenül jelezze az érintett szervezetnek[^15]. A felhasználó – tekintettel arra, hogy az adatok helyességéért teljes felelősséggel tartozik – természetesen jogosult a nyomtatványkitöltő program ellenőrzésének eredményét felülbírálni, illetve figyelmen kívül hagyni (azaz az esetek jelentős részében jogosultak hibajelzés mellett is elküldeni az űrlapot). A szolgáltatást nyújtó szervezetek ugyanakkor bizonyos logikai feltételeknek meg nem felelő űrlapok befogadását jogosultak megakadályozni az értelmezhetetlen adatok feldolgozásának elkerülése érdekében.

Az elkészített és a MeH által publikált elektronikus űrlapokhoz sok esetben külön letölthető egy útmutató vagy helyzetérzékeny segítő fájl, amely segíti az űrlap kitöltését.

Egyes esetekben az elektronikus űrlap mellé az adott ügyintézéshez szükséges elektronikus mellékletek is csatolhatók

2.2.3. Elektronikus beadvány előkészítése feladásra

A 2.2.2. fejezet szerint elkészített kimeneti állományból az elektronikus küldeményt a nyomtatványkitöltő program állítja elő biztosítva, hogy

–  az elektronikus beadvány a központi rendszer által elfogadott formátumú legyen,

–  az elektronikus beadványban továbbítandó, az elektronikus űrlapon rögzített adatok titkossága biztosított oly módon, hogy az adattartalomhoz csak a címzett szervezet férhessen hozzá.

Az elektronikus beadvány előállítása a felhasználó kötelessége, amit a nyomtatványkitöltő program erre vonatkozó funkciójával tehet meg. A kezelésre vonatkozó részletes leírást a kormányzati portál tesz közzé.

A központi rendszer az elektronikus beadvány beérkezésekor megvizsgálja, hogy az elektronikus beadvány megfelel-e a formai követelményeknek, a hibás formátumú elektronikus beadványokat a rendszer visszautasítja és a visszautasítás tényéről az ügyfelet értesíti. Ha a felhasználó a nyomtatványkitöltő programmal készítette el azon elektronikus beadványát, melyet feladáskor a központi rendszer visszautasított és ismeretei szerint minden előírást pontosan betartott, akkor haladéktalanul jelezze a problémát a KÜK felé.

2.2.4. Elektronikus beadvány feladása, érkeztetése

A tényleges küldés megkezdéséhez a felhasználónak be kell lépnie az ügyfélkapun. A felhasználó csak ezt követően jogosult a dokumentum feltöltésére.

A MeH felelősséget vállal azért, hogy a 2.2.3. pontban elkészített elektronikus beadványt tartalmi módosulás nélkül, csak a központi rendszerben használt időbélyegzéssel és érkeztetési számmal ellátva továbbítja a központi rendszeren keresztül a címzett szervezet részére.

A központi rendszer által az elektronikus beadványon elhelyezett időbélyegzés igazolja, hogy az időbélyeg által jelzett időpontban a központi rendszer a feladótól az elektronikus beadványt átvette és a címzett szervezet értesítési tárhelyén elhelyezte.

A címzett szervezet az elektronikus beadvány beérkezésének időpontjaként a központi rendszer által az elektronikus beadványhoz csatolt időbélyegben rögzített időpontot fogadja el.

A felhasználónak kell biztosítania, hogy elektronikus beadványát oly módon adja fel, hogy az – amennyiben ilyen van – a címzett szervezet, hatóság által meghatározott határidő előtt a központi rendszerbe beérkezzen. A felhasználó nem tekintheti elektronikus beadványát a központi rendszer által érkeztetettnek mindaddig, míg erre vonatkozóan a központi rendszer részére visszajelzést nem küldött.

A MeH nyomtatékosan felhívja a központi rendszeren át elektronikus űrlapokat küldő felhasználók figyelmét, hogy mind a kimenő állományt, mind a nyomtatványkitöltő program által abból készített elektronikus beadványt rendszeresen – lehetőleg a küldést követően azonnal – archiválják elektronikusan és szükség esetén papír alapon is, hogy később, vitás esetekben, ezen adatok a rendelkezésére álljanak! A megbízható elektronikus archiválás céljára rendelkezésére áll a központi rendszer által biztosított tartós tár is, amelybe a hivatalokhoz megküldött elektronikus űrlapok és a rájuk vonatkozó értesítések helyezhetők csak el. Az archivált példány megőrzési idejét a felhasználó határozza meg, de a MeH javasolja, hogy minden esetben vegye figyelembe a jogszabályok rendelkezéseit, hasonlóan a papír alapú beadványokhoz.

2.2.5. Visszaigazolás

A visszaigazolás birtokában a felhasználó kijelentheti, hogy beadványa a visszaigazoláson szereplő időpontban a címzett szervezethez megérkezett, a benyújtási kötelezettség esetén ennek a visszaigazolásban jelzett időpontban eleget tett. A visszaigazolást a felhasználó kötelessége oly módon tárolni, hogy a címzett szervezettel esetleg felmerülő vitás kérdésben azt mint bizonyítékot felhasználhassa. A központi rendszer üzemeltetője a kibocsátott visszaigazolásokat csak az érkeztető szám alapján visszakereshető módon tárolja. Az igazolás tartalmaz olyan azonosító információt, amely alapján annak változatlansága ellenőrizhető.

A központi rendszer által kiadott visszaigazolás a felhasználó kérése szerint két formátumban kerülhet továbbításra:

–  az ideiglenes tárhelyre (lásd 2.2.8 fejezet) PDF formátumú visszaigazolást küld a központi rendszer;

–  a felhasználó által az ügyfélkapu nyitásakor megadott (módosítható) elektronikus levelezési címre egyszerű formátumú elektronikus levelet küld a központi rendszer.

2.2.5.1. PDF formátumú visszaigazolás

„Érkeztetés visszaigazolás

Tisztelt <Felhasználó neve>!

Ön a(z) <címzett szervezet neve> részére elküldte a ’<Űrlap típusszáma>’ típusú kitöltött dokumentumát/nyomtatványát. A dokumentumot az elektronikus közigazgatási rendszer befogadta és gondoskodik annak továbbításáról a(z) <címzett szervezet neve> részére.

Az elküldésre került dokumentum file-neve:

<Fájl neve>

a befogadott dokumentum érkeztető száma:

<A központi rendszer által generált, a jogszabályok által meghatározott képzési módot követő érkeztető szám>

a befogadás hivatalos érkeztetési időpontja:

<Év>.<Hónap>.<Nap>. <Óra>:<Perc>

a befogadott dokumentum elektronikus lenyomata (SHA256-os algoritmussal és hexadecimális formában):

<SHA–256 lenyomat hexadecimálisan>

Segítség a nap 24 órájában

Telefon

Magyarországról hívható kék szám (helyi tarifával hívható): 189

Külföldről hívható telefonszám: +36 1 452-3622

Honlap

Mindent az Ügyfélkapuról:

www.magyarorszag.hu/ugyfelkapu/segitseg

www.ugyfelvonal.hu

E-mail

189@ugyfelvonal.hu

Fax

Magyarországról: 1 452-3621

külföldről: +36 1 452-3621

Üdvözlettel,

Közigazgatási és Elektronikus Közszolgáltatások Központi Hivatala

Budapest, <dátum>.”

A visszaigazolás tartalmazza:

–  az elektronikus beadványban továbbított fájl nevét, így segítve az ügyfelet, hogy a későbbiekben is azonosítani tudja, hogy mely visszaigazolás mely elektronikus beadványra, illetve az abban foglalt dokumentumra vonatkozik;

–  az érkeztető számot, mellyel mind a felhasználó, mind a címzett szervezet a későbbiekben hivatkozhat a beadott dokumentumra;

–  a beadás időpontját jelző időbélyegzést, mellyel a felhasználó igazolni képes, hogy a központi rendszer mely időpontban érkeztette az elektronikus beadványát.

2.2.5.2. Elektronikus levél, mint visszaigazolás

Az elektronikus levél tartalma megegyezik az előzőekben ismertetettel, azzal az eltéréssel, hogy nincs formázási információ benne.

2.2.6. Többes jóváhagyás kezelése

Egyes adatszolgáltatások, dokumentumok esetében a benyújtó (jellemzően jogi személy) saját szabályzata többes aláírást követel meg. Ebben az esetben a dokumentum csak akkor tekinthető benyújtottnak, ha azt valamennyi aláíró aláírta már. Addig az elektronikus beadvány (az űrlap) benyújtásra vár, már az érintett hivatalnál. Kivétel ez alól, ha az ügyfelek mindegyike saját, közigazgatásban felhasználható elektronikus aláírásával látja el benyújtás előtt az elektronikus dokumentumot.

A többes jóváhagyás technikai feltételeit a címzett szervezet teremti meg, használatának szabályait is ő rögzíti.

A központi rendszer a többes jóváhagyás kezelését azzal támogatja, hogy lehetővé teszi az elektronikus közszolgáltatást nyújtó szervezet számára, hogy a felhasználó elektronikus tárhelyére, illetve elektronikus levélcímére jóváhagyásra felszólító értesítést küldjön.

2.2.7. Elektronikus beadvány feldolgozása

Az elektronikus beadvány feldolgozása a címzett szervezet feladata, a beadvány feldolgozásával kapcsolatban a központi rendszer kizárólag a dokumentum tartalmának változatlan átadásáért felelős.

2.2.8. Értesítési tárhely használata

Az ügyfélkapu létesítésével párhuzamosan a felhasználó részére értesítési tárhelyet biztosít a központi rendszer, melyet a kormányzati portálon a http://www.magyarorszag.hu/allampolgar/szolgaltatasok/tarhely címre bejelentkezve ér el. A értesítési tárhelyen a felhasználónak lehetősége van a beérkezett üzenetek listázására, olvasására, saját számítógépre letöltésére és törlésére, beleértve a központi rendszer által küldött visszaigazolásokat is. A központi rendszer biztosítja, hogy letöltés esetén az értesítési tárhely kiválasztott üzenetének egy másolati példánya a felhasználó számítógépén jöjjön létre fizikailag.

Az értesítési tárhelyet a MeH átmeneti jelleggel, időben korlátozva bocsátja az ügyfelek rendelkezésére, azaz az üzenetek csak a beérkezéstől számított 30 napig tárolhatók az értesítési tárhelyen.

Az üzenet letöltésével párhuzamosan rendelkezik a felhasználó arról, hogy az értesítési tárhelyről az üzenetet törli vagy megtartja. A határidőt követően az üzenet automatikusan törlésre kerül!

A MeH felhívja ügyfelei figyelmét, hogy a felhasználó értesítési tárhelyének tartalmát vagy annak valamely részét utólag, a felhasználó által kért vagy határidő lejárata miatti törlés után nem képes visszaállítani.

2.2.9. Tartós tárhely használata

Az elektronikus közszolgáltatásokat ügyfélkapuval igénybe vevő felhasználók számára a Miniszterelnöki Hivatal tartós tárhelyet is biztosít a központi rendszerben. Ez a tárhely az értesítési tárhelyhez kapcsolódva a felhasználó számára érkezett, illetve általa az elektronikus közszolgáltatást nyújtó szervezeteknek megküldött elektronikus dokumentumok tárolását szolgálja. Használata időben nem korlátozott, jelenleg ügyfélkapunként 30 Mb tárhely áll a felhasználó rendelkezésére. Ennél nagyobb tárhely biztosítása csak külön megállapodás és díjfizetés alapján lesz lehetséges.

2.3. Használati jog felfüggesztése, megszüntetése

2.3.1. Hozzáférés megszüntetésének szabályai

Tekintettel arra, hogy a jogszabályi előírások szerint a felhasználó felel minden, a felhasználó által nyitott ügyfélkapun keresztül elérhető szolgáltatás helyes használatáért, valamint a hozzáférési jelszó védelméért, a MeH – a jogszabályi előírásoknak megfelelően – lehetővé teszi a felhasználók számára, hogy a jelszó feltételezhető kompromittálódása esetén a hozzáférés megváltoztatását kezdeményezzék.

2.3.1.1. Elveszett jelszó

Az új jelszót a www.magyarorszag.hu honlap ügyfélkapu bejelentkezési felületének elveszett jelszó menüpontjában lehet igényelni. Az eljárás eredményeként a felhasználó egy újabb egyszer használatos jelszót kap a regisztrációkor bejelentett elektronikus levélcímére, amivel az első regisztrációkor kapott egyszer használatos jelszóhoz hasonlóan kell eljárni. A szolgáltatás egy nap csak három alkalommal vehető igénybe.

2.3.1.2. Jelszó megváltoztatása

Az ügyfélkapu bejelentkezési felületén elérhető jelszó változtatása menüpont – amelyben a jelszót meg lehet változtatni – csak a bejelentkezett felhasználó számára áll rendelkezésre.

2.3.2. Újraérvényesítés módja

Amennyiben a felhasználó nem csak a jelszavát vesztette el, hanem a felhasználói nevét is vagy mindkettő kompromittálódott, a korrekcióra – éppen a visszaélések kizárása, adatok jogtalan megismerésének korlátozása érdekében kizárólag az okmányirodában való személyes megjelenéssel van lehetőség. Kérjük ezért, hogy a két azonosítóelemet elkülönítetten és különös gondossággal tárolják.

2.3.3. Ügyfélkapu megszűnése

2.3.3.1. A jelszó lejárata

Az ügyfélkapu a létrehozást követően a megszüntetéséig érvényes. Ugyanakkor a jelszó korlátlan idejű használata biztonsági okokból nem támogatott, azt kétévente meg kell újítani. A jelszó érvényességi idejének lejáratát követően az ügyfélkapu hozzáférése automatikusan megszüntetésre kerül. Ekkor a hozzáférés ismételt biztosítására csak az elveszett jelszóra vonatkozó szabályok szerint vagy új ügyfélkapu létesítését követően nyílik lehetőség. Új ügyfélkapu létesítésével azonban a korábbi tartós tárhoz nem lehet hozzáférést biztosítani. Éppen ezért fontos a lejáratra odafigyelni és még az előtt elektronikusan meghosszabbítani az érvényességet.

2.3.3.2. Ügyfél saját kérésére

Személyes megjelenés esetén az ügyfélkapu megszüntetésének eljárásrendje azonos az ügyfélkapu létesítésére vonatkozó eljárásrenddel. A www.magyarorszag.hu bejelentkezési felületén a felhasználó közvetlenül meg tudja szüntetni a saját ügyfélkapuját.

2.4. Speciális szabályok

2.4.1. Ügyfél elektronikus levelezési címének kezelése

A jogszabályi előírásoknak megfelelően a felhasználó kötelessége, hogy az ügyfélkapuhoz rendelt adataiban – különösen az elektronikus levelezési címében – történő változásokat haladéktalanul átvezesse.

A központi rendszer lehetővé teszi a felhasználó számára, hogy az elektronikus levelezési címét, melyre az értesítéseket a központi rendszer küldi, az ügyfélkapura történő bejelentkezést követően megváltoztassa.

A MeH elhárít minden, a felhasználó által megadott elektronikus levelezési címre történő hibás kézbesítésből származó felelősséget, különösen, ha a kézbesítés

–  az elektronikus levelezési cím hibás voltából,

–  az internet működési zavarából vagy

–  az elektronikus levelezési címhez kapcsolódó szolgáltatás üzemavarából fakadóan

hiúsult meg.

3. Szolgáltatás minőségi feltételei

3.1. Szolgáltatás színvonala

A központi rendszer vállalja, hogy

–  a szolgáltatást 0–24 órás üzemben 99,9% rendelkezésre állással nyújtja. Az üzemzavar esetére a hatósági ügy esetén a Ket 65. § (8) bekezdésében leírtak alapján vagy automatikusan mentesíti az ügyfelet az ebből szármató hátrányok alól vagy kérésére igazolást ad ki az üzemzavar tényéről. Az üzemzavarra vonatkozó információ a www.magyarorszag.hu kezdőlapján felül lenyíló menüben található;

–  egy óra alatt legalább 200 ezer dokumentum fogadását, bejelentkezés kezelését biztosítja;

–  a sikeresen feltöltött beadványokat – ha a nyomtatványkitöltő program sikeresnek minősíti a feltöltést – 1 percen belül érkeztetési számmal és időbélyegzéssel látja el és továbbítja a címzett szervezet tárhelyére, valamint a visszaigazolást a felhasználó ideiglenes tárhelyén elhelyezi, illetve erről az értesítő e-mailt elindítja.

3.2. Üzemzavar kezelése

3.2.1. Üzemzavar fogalmi meghatározása

Üzemzavarnak minősül, ha a központi rendszer az ügyfelek folyamatos kiszolgálását 15 percnél hosszabb ideig nem tudja biztosítani, azaz:

–  a nyomtatványkitöltő program aktuális verziójával készített elektronikus beadványt a központi rendszer tömegesen elutasítja;

–  a központi rendszer bármely okból nem képes fogadni a beadványokat;

–  a központi rendszer a befogadott beadványokról nem képes a visszaigazolásokat visszaküldeni.

Jelen szabályzat szempontjából nem számít üzemzavarnak:

–  az üzemzavar időtartama nem éri el a 15 percet;

–  a címzett szervezet informatikai rendszerének átmeneti vagy tartós működési zavara; ebben az esetben az üzenet befogadásra és visszaigazolásra kerül, csak a szervezet veszi később át;

–  a felhasználó által észlelt nem üzemszerű működés, ha ez a felhasználó informatikai rendszerének, illetve az internet vagy az informatikai eszközök működését biztosító környezet átmeneti vagy tartós működési zavarára vezethető vissza, függetlenül attól, hogy ez a felhasználók milyen körét érinti; ebben az esetben a hatósági ügyeknél a Ket. szabályai szerint a helyi szolgáltatótól lehet, illetve kell igazolást kérni a mulasztás kimentéséhez;

–  a nyomtatványkitöltő program vagy az elektronikus űrlapok működési hibája, ha a hiba jelentkezésének időpontjában már elérhető a kormányzati portálon vagy a címzett szervezet honlapján a program vagy az elektronikus űrlap újabb verziója, illetve a hiba nem akadályozza az űrlap beküldését.

3.2.2. Tájékoztatás üzemzavarról

Üzemzavar esetén a www.magyarorszag.hu kormányzati portálon információ jelenik meg az üzemzavar kezdő és végidőpontjáról, amit egy hónapon keresztül lehet a honlapon megtalálni. Az érintett csatlakozott szervezeteket a MeH közvetlenül tájékoztatja az üzemzavarról. Ennek megfelelően külön igazolást csak abban az esetben indokolt kérni, ha valamilyen egyedi hiba merült fel, ez azonban csak kivételesen lehet a központi rendszer által igazolható.

3.2.3. Üzemzavar következményei

A Ket. 33. §-a értelmében az üzemzavar az ügyintézési határidőbe nem tartozik bele.

Abban az esetben, ha az üzemzavar az APEH felé határidőre történő kötelezettség teljesítésében akadályozza az ügyfelet, mert az üzemzavar a határidő napján jelentkezik, akkor a határidő automatikusan – külön kérelem nélkül – egy teljes nappal elcsúsztatásra kerül.

Minden más esetben

–  a Hatóság saját hatáskörben dönt a határidő megváltoztatásáról, de csak az üzemzavar időtartamával köteles a határidőt módosítani (amennyiben az akadályozza a határidőre történő benyújtást);

–  egyedi üzemzavar (dokumentum megsérülése vagy más hibajelenség esetén) a felhasználó kérelmére a MeH igazolást állít ki az üzemzavar tényéről, rögzítve az üzemzavar kezdetének és végének időpontját.

A központi rendszer üzemeltetője a központi rendszer rendelkezésre állását, az üzemzavarok időpontját és időtartamát hitelesen dokumentálja.

3.2.4. Üzemzavar kezelése

Az üzemzavar elhárítását a MeH azonnal megkezdi. Abban az esetben, ha az üzemzavar következményeként adatvisszaállítás szükséges, akkor megvizsgálja, hogy

–  az adatvisszaállítás mely időpontra lehetséges, illetve adatvesztés előfordulhatott-e,

–  az adatvisszaállítás érinti-e a felhasználói törzsadatokat vagy a benyújtott adatokat.

3.2.4.1. Adatvesztés kezelése

Az elektronikus közszolgáltatást nyújtó szervezet ideiglenes tárhelyét érintő adatvesztés előfordulása esetén a MeH a naplóállományok alapján az ideiglenes tárhelyre és a felhasználó elektronikus levelezési címére együttesen küldött levélben értesíti a visszaállított időpont és az üzemzavar bekövetkezési ideje között a rendszerbe bejelentkezett felhasználókat az általuk küldött elektronikus beadványok esetleges elvesztéséről. A tényről a MeH az érintett csatlakozott szervezeteket is tájékoztatja. A felhasználó kötelessége, hogy megismételje az elektronikus beadvány feladását, ugyanakkor az elektronikus közszolgáltatást nyújtó szervezet felé kötelezettségét az első beküldés időpontjában teljesítette, ha e tényt igazoló visszaigazolás a birtokában van.

A felhasználó ideiglenes tárhelyét a MeH a legutolsó mentett állapotba állítja helyre.

3.2.4.2. Törzsadat visszaállítás

Abban az esetben, ha a felhasználók törzsadatainak visszaállítása szükséges, akkor minden bizonytalan azonosítási állapotú felhasználó jelszavát módosítja új egyszer használatos jelszóra;

– a jelszavakat elküldi a felhasználók elektronikus levelezési címére;

– a felhasználó a következő bejelentkezésnél a regisztrációhoz hasonlóan az új egyszer használatos jelszóval képes bejelentkezni, majd köteles megváltoztatni a jelszavát egy általa választott jelszóra;

– a jelszó változtatását követően a felhasználó a 2.2 pont rendelkezései szerint ismét használhatja a központi rendszer szolgáltatásait.

3.2.5. Bűncselekmény gyanúja esetén követett eljárás

Abban az esetben, ha az üzemzavar feltételezhetően a hatályos jogszabályok értelmében bűncselekménynek tekinthető tevékenység következménye, a MeH büntető feljelentést tesz az illetékes nyomozó hatóságnál.

A MeH a nyomozás hatékony lefolytatása érdekében a nyomozó hatóság által kért minden adatot (lásd 4.4.2. pont) a hatóság rendelkezésére bocsát.

3.3. Panaszkezelés

Az elektronikus közszolgáltatást nyújtó szervezet és a felhasználó közötti vitás ügybe a MeH csak abban az esetben vonható be, ha az információ bizonyíthatóan a központi rendszerbe történt beérkezés és az elektronikus közszolgáltatást nyújtó szervezetnek történt átadás között sérült vagy változott meg. Ez a rendszer működési modelljéből következően a tartalom ismerete nélkül is dokumentálható.

3.3.1. Kapcsolattartás

A MeH a szolgáltatás igénybevétele során felmerülő problémák orvoslására, megválaszolására, reklamációk ügyintézésére központi ügyfélszolgálatot, ügyfélvonalat üzemeltet, melyet a felhasználó telefonon, illetve levélben vagy elektronikus úton kereshet fel.

Az ügyfélszolgálat adatai:

Központi ügyfélszolgálat – ügyfélvonal

Nyitva tartási idő: 0–24 óráig

Elérhetőségek:

Telefon: Magyarországról hívható kék szám (helyi díjszabással): 189

Külföldről hívható telefonszám: +36 1 452 3622

SMS 189

Honlap: www.magyarorszag.hu/ugyfelvonal

www.ugyfelvonal.hu

E-mail: 189@ugyfelvonal.hu

Fax: Magyarországról: 1 452 3621

külföldről: +36 1 452 3621

A központi ügyfélszolgálat lehetővé teszi a felhasználó számára, hogy

–  az elektronikus beadványok kezelésével kapcsolatban tájékoztatást, probléma esetén segítséget kérjen;

–  konkrét – hatósági ügyintézéshez kapcsolódó – panasz esetén a felhasználó a címzett hatóság illetékes munkatársának eléréséhez támogatást kapjon.

3.3.2. Panaszok, kifogások intézése

Amennyiben a felhasználó a központi ügyfélszolgálat munkáját nem ítéli kielégítőnek, úgy lehetősége van levélben (cím: 1094 Budapest, Balázs Béla u. 35.) vagy elektronikus levélben (ekelnh@ahiv.hu) megkeresni a Közigazgatási és Elektronikus Közszolgáltatások Központi Hivatalát, ahol panaszát az erre vonatkozó szabályok szerint kivizsgálják.

3.3.3. Késedelem

Késedelemre visszavezethető vita esetén a felhasználónak rendelkezésére áll a beadványaira a központi rendszer által adott visszaigazolás (lásd 2.2.5. fejezet), mellyel bizonyítja, hogy kötelességének a visszaigazolásban rögzített időpontban eleget tett. Az elektronikus közszolgáltatást nyújtó vagy abban részt vevő szervezetek, hatóságok a visszaigazolásban rögzített időpontot nem kérdőjelezik meg.

3.3.4. Tartalmi problémák

Ha a felhasználó mindenképpen meg kíván bizonyosodni arról, hogy az általa továbbított beadvány sértetlenül érkezett-e meg a szolgáltatást nyújtó szervezethez, akkor jogszabály lehetővé teszi számára, hogy a feladással párhuzamosan saját maga számára is elküldjön egy példányt a feladott dokumentumcsomagból, a saját tartós tárhelyére. Ez kétség esetén bizonyítja, hogy mit küldött el.

Abban az esetben, ha az elektronikus beadványt az elektronikus közszolgáltatást nyújtó szervezet nem képes feldolgozni, akkor a Ket., illetve az adott szervezetre, hatóságra vonatkozó jogszabályokban meghatározott eljárásrend szerint igényelheti a hiánypótlást, a hibás, téves adatok kijavítását, az általa meghatározott ügyrend szerint utasíthatja az ügyfelet az adatok javítására. A hibás adatszolgáltatás következményeit, az alkalmazandó szankciót a Hatóság által alkalmazott gyakorlatot a hatályos jogszabályok határozzák meg.

3.4. Tiltott tevékenységek

Az ügyfél csak a személyéhez rendelt jogosultsággal tevékenykedhet a központi rendszerben és a felhasználói azonosítójával végrehajtott minden tevékenységért felelősséggel tartozik.

A központi rendszer működtetője a felhasználó jogellenes tevékenysége esetén büntetőeljárás lefolytatását kezdeményezi.

4. Biztonsági intézkedések

Jelen fejezet a MeH informatikai biztonsági elkötelezettségét bizonyítja, az ügyfélkapcsolatra vonatkozó biztonsági óvintézkedéseket rögzíti. A központi rendszer részletes biztonsági eljárási szabályait az üzemeltetők nem nyilvános Informatikai Biztonsági Szabályzatai rögzítik.

4.1. Szervezeti és személyi biztonsági intézkedések

4.1.1. Belső eljárásrendek

4.1.1.1. Általános szabályok

A központi rendszer informatikai eszközeit kizárólag felhatalmazott, a feladat ellátásához szükséges szaktudással rendelkező személyzet működteti. A MeH a működtetés folyamatait belső eljárásrendekben rögzítette, előírva, hogy milyen rendszerességgel, milyen módon kell az üzemeltetési és karbantartási feladatokat végrehajtani.

A központi rendszeren történő minden munkavégzés naplózásra kerül.

A MeH a szolgáltatásban és az azt kiszolgáló informatikai rendszerekben bekövetkező módosítások, változások biztonságos és visszakereshető végrehajtása érdekében dokumentált változáskezelési rendet követ.

4.1.1.2. Biztonsági felülvizsgálatok rendje

A rendszeres információ biztonsági felülvizsgálatok célja a kialakított védelmi rendszer működési hatékonyságának mérése az egyenszilárdságot veszélyeztető hiányosságok és sebezhetőségek feltárása, a szükséges helyesbítő és megelőző védelmi intézkedések kidolgozása, előterjesztések elkészítése.

A MeH a központi rendszer kulcsfontosságú komponenseire rendszeresen – évente legalább egyszer – sebezhetőségi vizsgálatot végeztet, melynek végrehajtása során figyelembe veszi a naplózott események feldolgozása során azonosítható támadási kísérleteket és módokat. A sebezhetőségi vizsgálat célja, hogy az egyes komponensek által hordozott biztonsági kockázatok újraértékelése megtörténjen.

A MeH megkívánja továbbá az egyes szoftver komponensek gyártóitól, hogy sebezhetőségi vizsgálatot végezzenek és erre vonatkozóan a bizonyítékokat adják át a MeH részére.

A MeH szúrópróbaszerűen egy-egy esemény felülvizsgálatát havonta többször, általános felülvizsgálatot hathavonta vagy üzemzavart kiváltó rendkívüli eseményt követően azonnal hajt végre, a felülvizsgálatról készült bizonylatokat 15 évig megőrzi. A vizsgálatokat minden esetben a naplóállományokra alapozza.

4.1.2. Fontos és bizalmas munkakörök

4.1.2.1. Biztonsági felelős

Az üzemeltető biztonsági felelőse biztosítja

–  a kockázatok csökkentését célzó védelmi intézkedések kidolgozását, bevezettetését;

–  a már életbe léptetett eljárásrendekben előírt intézkedések érvényre jutását, betartatását;

–  az informatikai rendszerek biztonsági szintjének rendszeres ellenőrzését;

–  az üzemeltetői hozzáférési jogok kiadásának és visszavételének kezelését;

–  a központi rendszer napló archiválását, rendszeres átvizsgálását, biztonsági események feltárását.

4.1.2.2. Adatvédelmi felelős

A MeH adatvédelmi felelőse látja el az Avtv.-ben rögzített feladatokat, beleértve az ügyfelek személyes adatainak kezelésével kapcsolatos tájékoztatási és ellenőrzési kötelezettségeket is.

4.1.2.3. Üzemeltetésvezető

Az üzemeltetésvezető feladata a központi rendszer működtetésének megszervezése, a működés biztonságához szükséges nyilvántartások naprakészségének biztosítása, az üzemeltetési folyamatok kialakítása, a rendszergazdák és operátorok tevékenységének koordinálása, együttműködés a biztonsági vezetővel a védelmi intézkedések kialakításában.

Az üzemeltetésvezető teljes utasítási joggal rendelkezik üzemeltetés területén.

4.1.2.4. Rendszergazda

A rendszergazda feladata központi rendszer egyes alrendszereinek üzemeltetése, beleértve

– az operátor által nem kezelhető incidensek elhárítását;

– az elkészített adat- és rendszermentések belső szabályok szerinti tárolását, utasításra adatvisszaállítás végrehajtását;

– a belső szabályzatokban előírt rendszeres karbantartási tevékenységek végrehajtását;

– a változások élesítését az üzemi környezetben;

– az üzemeltetői hozzáférési jogok beállítását az informatikai rendszereken a biztonsági felelős utasításainak maradéktalan betartásával.

A rendszergazda köteles tevékenységét a belső szabályzatok előírásai szerint bizonylatolni.

4.1.2.5. Operátor

Az Operátor feladata

–  biztonsági események fogadása, elsőszintű kezelése;

–  távfelügyeleti rendszeren a központi rendszer működésének folyamatos monitorozása;

–  mentések végrehajtása.

A operátor köteles tevékenységét a belső szabályzatok előírásai szerint bizonylatolni.

4.1.3. Személyi biztonság

A személyekre vonatkozó biztonsági intézkedések célja a gondatlanságból elkövetett emberi károkozás, valamint a szándékos visszaélések kockázatának csökkentése.

Tekintettel arra, hogy a fontos és bizalmas munkakört betöltők esetében van lehetőség leginkább a visszaélésekre, ezért ezeket a munkaköröket

–  csak erkölcsi bizonyítvánnyal rendelkező, nemzetbiztonsági ellenőrzésen átesett;

–  megfelelő szakképesítéssel és szakvizsgával, az adott szakterületre előírt gyakorlattal rendelkező

személy töltheti be.

A MeH hangsúlyt fektet arra, hogy az ilyen munkakört betöltő személyek szakmai felkészültsége mindenkor megfeleljen a kor követelményeinek, ezért a továbbképzések rendjét belső utasításban határozza meg.

Ilyen munkakört betöltő személy által elkövetett visszaélés esetén a MeH a jogszabályok figyelembevételével a lehető legszigorúbb szankciókat alkalmazza.

4.2. Fizikai biztonsági intézkedések

A központi rendszer alapvető informatikai eszközeinek telephelyét és a működésükhöz szükséges infrastruktúrát a MeH biztosítja. A kialakított környezet az

–  áramellátás,

–  légkondicionálás,

–  tűzmegelőzés és tűzvédelem,

–  villámvédelem,

–  betörésvédelem, beleértve az élőerős védelmet is,

területén a vonatkozó biztonsági előírásoknak maradéktalanul megfelel, a kialakított védelem arányban áll a MeH által kockázatelemzésben azonosított kockázatokkal és biztosítja, hogy:

–  az infrastruktúrát érintő hibák ne veszélyeztessék a vállalt szolgáltatási szintet;

–  természetes személyek gondatlanságból vagy szándékosan ne legyenek képesek kárt okozni a központi rendszer működésében, továbbá

–  ne legyen módjuk veszélyeztetni a központi rendszer által feldolgozott adatok titkosságát és sértetlenségét.

4.3. Adatbiztonság

4.3.1. Mentés

A központi rendszerben tárolt és feldolgozott minden adatról üzemzavar elhárítása céljából adatmentés készül. Ezen mentések biztosítják, hogy adatvesztéssel járó üzemzavar esetén az adatvesztés mértéke még elfogadható mértékű legyen. A kialakított mentési stratégia olyan, hogy legrosszabb esetben is csak korlátozott adatvesztés lehetséges.

4.3.2. Archiválás

4.3.2.1. Archivált adatkörök és megőrzési idejük

Az ügyfél által végzett tevékenységekről készített naplóállományok megőrzési ideje egy hónap, ezen adatok az előírt időpontig archiválásra kerülnek.

Az ügyfélszolgálati és üzemeltetési tevékenységekről készített naplóállományok megőrzési ideje ugyanez.

A dokumentummozgásokhoz (bevallások, adatszolgáltatások, döntések stb. ügyfelek, illetve hivatalok általi küldése) kapcsolódó adatokat pedig a köziratokról, a közlevéltárakról és a magánlevéltári anyag védelméről szóló 1995. évi LXVI. törvény alapján elfogadott levéltári tervek szerint archiváljuk, mivel ezek az iratmozgás alapdokumentumai.

4.3.2.2. Az archivált adatok védelme és hozzáférési szabályok

A MeH az archivált adatok titkosságát és sértetlenségét belső biztonsági szabályzataiban meghatározott módon védi. Az archivált adatokhoz az üzemeltető biztonsági felelőse és az általa feljogosított személyek kizárólag a törvényben meghatározott célokból férhetnek hozzá. A MeH a teljes megőrzési idő alatt biztosítja a jogosultak számára az adatok hozzáférhetőségét és értelmezhetőségét.

4.3.2.3. Az archivált adatok gyűjtésének rendje

Az elektronikusan tárolt adatok naponta kerülnek mentésre oly módon, hogy az adathordozók egy e célra rendszeresített tárolóhelyen kerülnek elhelyezésre.

A nem elektronikus formában keletkező adatok, iratok a MeH irattári tervében meghatározott módon kerülnek tárolásra.

4.4. Logikai biztonsági intézkedések

4.4.1. Üzembiztonság

A központi rendszer szolgáltatásait biztosító informatikai rendszerek ellenállnak az egyszeres hardver meghibásodásnak.

4.4.2. Időforrás és időszinkronizáció

Tekintettel arra, hogy az üzenettovábbító alrendszer által nyújtott szolgáltatás esetében az idő nagy jelentőségű, a központi rendszer minden komponensének belső órája szabványos és hiteles időforráshoz szinkronizált, az időt szolgáltató eszközök a beérkező időadatok egyértelműségét biztosítják.

Az időszinkronizálás jelen szabályzatban meghatározott pontosságánál nagyobb eltérése üzemzavarnak minősül és az eseményt a MeH a 3.2 pont rendelkezései szerint kezeli.

A használt időforrások az UTC-hez képest néhány ezred másodpercet térhetnek el, a rendszer egészének pontossága is jobb, mint az időbélyegzésekben megadott idő.

4.4.3. Az időbélyegzés megoldása

Az időbélyegzés előállítása a központi rendszerben az e célra telepített külön eszközön történik oly módon, hogy az időbélyegzésre használt elektronikus aláíró eszköz megfelel a minősített aláírásra vonatkozó jogszabályi követelményeknek. A minősített időbélyegzés szolgáltatás biztosítása a külön jogszabályban meghatározott feltételek szerint történik.

4.4.4. Határvédelem

A központi rendszert az internettől tűzfal szerverek választják le, melyekre vonatkozó részletes rendelkezéseket a központi elektronikus szolgáltató rendszer informatikai biztonsági szabályzata rögzíti. A határvédelmi rendszer biztosítja az adatáramlás ellenőrzését/szűrését a feldolgozó rendszerek felé megelőzendő a kártékony kódok és szolgáltatásmegtagadás támadások előfordulását, megakadályozza a tiltott adatforgalmat, naplózza mind a tiltott, mind az engedélyezett adatforgalmat.

A határvédelmi rendszer riasztási funkcióval is rendelkezik, mely meghatározott tiltott események bekövetkezése esetén automatikusan jelzést ad. Ezen események rendkívüli eseményként kezelendők. A központi rendszer üzemeltetője folyamatosan monitorozza a központi rendszer adatforgalmát és rosszindulatú tevékenység észlelése esetén értesíti az ezek kezelésére feljogosított hatóságokat.

4.4.5. Biztonsági naplózás

A központi rendszer biztonságos működése csak akkor valósítható meg, ha a rendszerben bekövetkező események visszakereshető és elemezhető módon tárolásra kerülnek. Az ügyfeleknek tudomásul kell venniük, hogy saját és más ügyfelek biztonsága érdekében az általuk végrehajtott tevékenységek jelentős része naplózásra kerül. A MeH a naplózott eseményt kiváltó látogatókat vagy ügyfeleket a naplózás tényéről külön nem értesíti, indokolt esetben azonban be kívánja vonni őket az esemény kivizsgálásának folyamatába. (A MeH kéri tisztelt ügyfeleit, hogy a kivizsgálásában közreműködni szíveskedjenek.)

A központi rendszer a rendszer aktivitását széles körben és részletesen naplózza, beleértve mind a látogató, mind a bejelentkezett ügyfél és Hatóság, mind az üzemeltetők által végzett tevékenységeket.

A naplóbejegyzések minden esetben tartalmazzák az esemény bekövetkezésének dátumát és időpontját, minden, az esemény utólagos kiértékelése szempontjából fontos adatot, beleértve a végrehajtó személy azonosításához szükséges adatokat.

Tekintettel a központi rendszer egyes komponenseinek naplózás tulajdonságaira, bár a naplóállományok nem egy helyen és azonos formában keletkeznek, de tárolásuk és feldolgozásuk központilag egységes szerkezetben történik.

4.4.5.1. Tárolt események típusai

A központi rendszer minden, a látogatók és ügyfelek által végzett tevékenységet naplóz, beleértve

–  bejelentkezés nélkül elérhető honlapok esetében

= a látogatás időpontját,

= a látogató számítástechnikai eszközének IP címét,

= a böngésző típusát;

–  a felhasználó ügyfélkapus bejelentkezésével végezhető eljárások esetében

= a felhasználó nevét és e-mail címét (amit egyébként az ügyintéző rendszereknek átadott),

= a felhasználó bejelentkezésének és kijelentkezésének időpontját anélkül, hogy az aktivitás természetéről rögzítene további adatokat;

–  az előző naplóállománytól teljesen függetlenül tárolja a továbbított üzenetek naplóbejegyzéseit, s benne

= feladó nevét;

= feladó e-mail címét;

= címzett elektronikus közszolgáltatást nyújtó megnevezését;

= a továbbított dokumentum típusát (nyomtatványazonosító);

= az érkeztető számot;

= a fogadás és továbbítás időpontját.

A naplóállományok kezelése a 4.3.2.1. pontban rögzített adatkezelési határidőkig történik, kivéve a dokumentummozgásokhoz (bevallások, adatszolgáltatások, döntések stb. ügyfelek, illetve hivatalok általi küldése) kapcsolódó adatokat, melyek kezelésére a Ket. hatálya alá tartozó eljárási cselekmények Ügyfélkapun keresztül történő intézésekor került sor, s melyek tárolásának időtartama a levéltári törvényben rögzített selejtezési határidőkkel egyezik meg.

Az üzemeltetési tevékenységek és a rendszer belső működésének naplózása szintén megtörténik, beleértve

–  rendszermenedzsment tevékenységeket, mint rendszergazdai be-, illetve kijelentkezés, a rendszer vagy komponensének indítása/leállítása, verziófrissítés, adatbázis-menedzsment tevékenységek;

–  az audit alrendszer menedzsmentjével kapcsolatos tevékenységeket, mint a naplózási funkció konfigurációjának módosítása, leállítása, újraindítása stb.;

–  mentési műveleteket;

–  ügyfélszolgálati tevékenységek, mint ügyfél használati jogának felfüggesztése, újraérvényesítése, ügyfél hozzáférésének törlése stb.;

–  a központi rendszer egyes komponenseiben bekövetkező, naplózást igénylő eseményeket/hibákat, mint adatbázis események, operációs rendszer események stb.

4.4.5.2. Naplóállomány védelme

A központi rendszer naplóállománya védett a jogosulatlan adatmódosítástól, azaz a naplóbejegyzések sorrendje és a bejegyzések adattartalma, beleértve a bejegyzéshez rendelt időt is, nem változtatható meg, a naplóállományból bejegyzés nem törölhető.

A naplóállományt a gondatlanságból vagy szándékosan elkövetett rongálás ellen biztonsági mentések védik. A MeH minden naplóállomány esetében, beleértve a személyes adatokat tartalmazó naplóbejegyzéseket is, gondoskodik az adatok bizalmas tárolásáról. A naplóállományhoz csak a biztonsági vezető által arra feljogosított személyzet férhet hozzá, szigorúan a hibaelhárításhoz szükséges mértékben. A MeH bűncselekmény gyanúja esetén, hatósági megkeresésre a szükséges adatokat, naplóbejegyzéseket a nyomozó hatóság rendelkezésére bocsátja.

[^14]: Jelenleg csak a Java futtató környezet, amely szintén díjtalanul áll rendelkezésre.
[^15]: Az érintett szervezetek ügyfélszolgálati elérhetőségei a www.magyarorszag.hu honlap hivatalkeresőjében találhatók meg.
