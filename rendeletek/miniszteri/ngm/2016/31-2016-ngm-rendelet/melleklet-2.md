## Az AFE-re, illetve a felügyeleti szolgáltató informatikai rendszerére és munkafolyamatára vonatkozó műszaki követelmények

## A) A Felügyeleti Szolgáltató (a továbbiakban: FSZ) informatikai rendszerére vonatkozó követelmények

## 1) Az élelmiszer értékesítését kezelőszemélyzet nélkül végző étel- és italautomata beruházásainak védelmében a FSZ az egyes automata típusok sajátosságaihoz igazodóan alakíthatja ki a jelen melléklet követelményeiben meghatározott képességekkel rendelkező AFE és saját központja közötti kommunikációt. A kommunikációt úgy kell kialakítani, hogy a jelen rendelet 3. mellékletében definiált NAV felé történő kommunikáció és adatszolgáltatás megvalósítható legyen.

## 2) Az FSZ elektronikus információs rendszerét legalább az állami és önkormányzati szervek elektronikus információbiztonságáról szóló 2013. évi L. törvényben meghatározott technológiai biztonsági, valamint a biztonságos információs eszközökre, termékekre, továbbá a biztonsági osztályba és biztonsági szintbe sorolásra vonatkozó követelményekről szóló 41/2015. (VII. 15.) BM rendelet alapján úgy kell kialakítani hogy megfeleljen a védelmi intézkedések területén az következő biztonsági osztályok:

## a) Adminisztratív védelmi intézkedések – 3. biztonsági osztály

## b) Fizikai védelmi intézkedések – 3. biztonsági osztály

## c) Logikai védelmi intézkedések

## i. bizalmasság – 3. biztonsági osztály,

## ii. sértetlenség – 3. biztonsági osztály,

## iii. rendelkezésre állás – 3. biztonsági osztály.

## 3) Az AFE-k és a FSZ között zárt APN-t kell kialakítani. Az AFE és a FSZ közötti kommunikációs csatornát a telemetriai, műszaki felügyeleti valamint fizetési tranzakciók lebonyolítására is igénybe lehet venni. Ezen információk leválasztását az értékesítési információkról a FSZ központi rendszere végzi.

## 4) Az AFE és a FSZ közötti kommunikációban biztosítani kell az AFE-k device certificate alapú azonosítását, az adatok SSL titkosítással történő biztonságos küldését valamint az AFE-k által generált aláíró kulccsal történő adat aláírást a sértetlenség érdekében. Az alkalmazott kulcsok hossza RSA algoritmus esetén legalább 2048 bit legyen. Ezzel egyenértékű biztonságot adó más algoritmus is használható, amennyiben azt a 7-8. § szerinti tanúsítványt kiállító tanúsító szervezet elfogadja.

## 5) A biztonsági követelményeknek való megfelelőséget a 8. §-nak és a 9. §-nak megfelelő tanúsító szervezet által kiállított tanúsítvánnyal kell igazolni, melyet az engedélyezési kérelemhez kell csatolni.

## 6) A FSZ és a NAV között két egymástól független útvonalon megvalósított VPN kapcsolatot kell felépítenie a FSZ-nak. Az adatkapcsolat minimális sávszélessége a felügyelt AFE-k mennyisége szorozva 16 kbit/s-mal.

## 7) A felügyeleti szolgáltatónak

## a) az AFE-k által gyűjtött adatokat zárt informatikai rendszerben kell kezelnie,

## b) az e rendelet által szolgáltatandó adatok és AFE által gyűjtött egyéb adatok logikai elválasztását biztosítania kell,

## c) rendelkeznie kell telephely biztonsági tanúsítvánnyal,

## d) a tárolt adózói adatok közvetlen módosítására nem lehet jogosultsága, az informatikai rendszerét úgy kell kialakítania, hogy az adózói adatokat kizárólag a NAV szerveréről érkező utasítás alapján módosíthassa,

## e) a felügyeleti szolgáltatói feladatainak ellátása céljából működtetett rendszereit az Európai Unió területén, korlátozott hozzáférésű, biztonságos területen kell elhelyeznie, amelynek kialakítása során szünetmentes tápellátást és illetéktelen személyek hozzáférését megakadályozó felépítést kell biztosítania, valamint a központi szervert megfelelő fizikai és logikai behatolás elleni védelemmel, vírusvédelemmel, tűzfallal kell ellátnia a jogosulatlan hozzáférések megakadályozása céljából,

## f) gondoskodnia kell arról, hogy a szervertermébe az üzemeltetés és a karbantartás elvégzésére jogosultakon kívül kizárólag a NAV részére előzetesen írásban bejelentett személyek léphetnek be, a belépésről elektronikus beléptető rendszer által vezetett nyilvántartást kell vezetnie, amely tartalmazza a belépő személyazonosító adatait, a belépés és távozás idejét és a belépés célját; valamint arról, hogy a közigazgatási hatóságok hatósági ellenőrzéssel kapcsolatban a szerverterembe bármikor beléphetnek, és a biztosítania kell, hogy rendszereinek ellenőrzése bármikor akadálymentesen megtörténhessen.

## g) rendszerének minimálisan 99,5 %-os rendelkezésre állást kell garantálnia, nagy hibatűrésű rendszer alkalmazásával,

## h) a felügyeleti szolgáltatói feladatainak ellátása céljából működtetett rendszerét naplóznia kell, amely naplók megváltoztathatatlanságáról gondoskodnia kell; valamint a naplóbejegyzéseknek tartalmazniuk kell az események megnevezését, dátumát, idejét ezredmásodperc pontossággal és az eseményt egyértelműen azonosító minden egyéb információt,

## i) biztosítania kell az engedélyező hatóság, illetve a NAV számára a naplók ellenőrizhetőségéhez szükséges hozzáférést,

## j) biztosítania kell, hogy felügyeleti szolgáltatói feladatainak ellátása céljából működtetett rendszeréhez kizárólag a felügyeleti szolgáltató informatikai rendszerének megfelelőségét igazoló tanúsítványban megnevezett AFE kapcsolódhasson,

## k) az AFE által rögzített értékesítési adatokból (tranzakciós adatok) létrejött adatcsomagokat zárt számadású, kihagyás és ismétlés nélkül növekvő sorozatszámmal, valamint az AFE-ban tárolt kulcs felhasználásával védett hardver és szoftver környezetben elektronikus aláírással kell ellátnia, amelyhez az aláíró kulcsot a felügyeleti szolgáltató adja ki saját rendszeréből ,

## l) a beérkező adózói adatokat és a központi rendszerének működési naplóit olyan módon kell archiválnia, hogy az a lenyomatképző algoritmusok biztonsági gyengülése ellen védett legyen, és az archiválás megfeleljen a digitális archiválás szabályairól szóló 114/2007. (XII. 29.) GKM rendeletben meghatározott hosszú távú megőrzésre alkalmas archiváló rendszer feltételeinek.

## B) Az AFE-ra vonatkozó követelmények

## 1. Az AFE-nek alkalmasnak kell lennie az értékesítés, illetve az e rendeletben meghatározott egyéb események adatainak rögzítésére, tárolására és továbbítására a FSZ központjába annak érdekében, hogy a FSZ a B) részben megadott adatszolgáltatási követelményeknek ezen adatok birtokában eleget tudjon tenni a B) pontban meghatározott tartalommal, módon és szerkezetben.

## 2. Az AFE alkalmas lehet az automata működésével kapcsolatos olyan adatok rögzítésére és továbbítására is, amelyeket e rendelet nem követel meg.

## 3. Az automata nem rendelkezhet olyan funkcióval, amely révén az üzemeltető, vagy más személy törölheti, módosíthatja, vagy kiegészítheti az AFE-ben már rögzített adatokat, ide nem értve, ha erre vonatkozó utasítás a NAV szerveréről érkezik.

## 4. Az automata nem lehet alkalmas értékesítés végrehajtására az értékesítés adatainak rögzítése nélkül.

## 5. Az AFE-vel felszerelt automatához tilos csatlakoztatni, illetve egybeépíteni olyan egységgel, berendezéssel, amely korlátozza annak e rendeletben szabályozott funkcióit, kivéve az e rendeletben kifejezetten engedélyezett eseteket.

## 6. Az automata – az e rendeletben meghatározott kivételektől eltekintve – csak akkor végezhet értékesítést, ha az automatában AFE működik.

## 7. Értékesítéskor az AFE rögzíti az értékesítés adatait. A rögzített adatokat az AFE mindaddig tárolja, amíg azokat nem tudta az FSZ számára sikeresen továbbítani.

## 8. Az AFE-t az automatába olyan módon kell beépíteni, hogy az elválaszthatatlanul kapcsolódjon az automata vezérlőpaneljéhez. Az AFE beépítést úgy kell megvalósítani, hogy az bekötésében, vezérlési logikában valamint rögzítési kivitelezésében az automata vezérlésének, pénzvizsgáló, banki tranzakciós terminál, illetve egyéb csatlakozó elemeinek tekintetében roncsolás nélkül megbonthatatlan zárt rendszert képezzen. A beépítést úgy kell megvalósítani, hogy a vezérlési és fizető eszköz kezelést megvalósító elemeinek megbontása esetén, illetve az AFE kiktatása esetén az automatának működésképtelennek és árukiadásra alkalmatlannak kell lennie.

## BA) Automata blokkolt állapota

## 9. Az automatának blokkolt állapotba kell kerülnie, amennyiben

## a) az AFE bármilyen okból nem működik megfelelően, különösen amennyiben az AFE nem képes biztonságosan ellátni a lezajlott események rögzítésének és/vagy FSZ felé továbbításának feladatát, ide nem értve, ha az adatok FSZ felé történő továbbítása az elektronikus hírközlő hálózat elérhetőségének hiányából adódik,

## b) az AFE felnyitási kísérletet érzékelt,

## c) a kapcsolat sérül az AFE és az automata többi egysége között,

## d) a NAV szerveréről blokkolási utasítás érkezett a FSZ-hoz az adott automata működésének blokkolására és ezt a FSZ továbbította az érintett AFE részére,

## 10. Blokkolt állapotban az automata értékesítést nem végezhet.

## 11. A 9. pont a)-c) alpontja szerinti blokkolt állapotot kizárólag szervizelési tevékenysége keretében a FSZ szervize oldhatja fel.

## 12. A 9. pont d) alpontja szerinti blokkolt állapotot kizárólag a NAV szerveréről érkező, és a FSZ által az AFE-be továbbított ezirányú utasítás oldhatja fel.

## BB) Az AFE fizikai jellemzői és elhelyezése

## 13. Az AFE-t fizikailag az automata burkolatán belül kell elhelyezni. Ha az elhelyezés a burkolaton belül nem valósítható meg, akkor az AFE az automata burkolatához rögzítetten kell elhelyezni úgy, hogy az AFE felnyitása vagy eltávolítása csak roncsolással legyen megvalósítható.

## 14. Az AFE-nek meg kell felelnie az elektromágneses összeférhetőségről szóló 62/2006. (VIII. 30.) GKM rendelet előírásainak. Az AFE adattartalma UV sugárzással nem lehet törölhető.

## 15. Az AFE-t úgy kell kivitelezni, hogy kizárólag az AFE burkolat roncsolásával lehet nyitható. A burkolat roncsolásakor az AFE-nek blokkolt állapotba kell kerülnie.

## 16. Az AFE-t úgy kell elhelyezni az automatában, hogy értékesítés ne legyen lehetséges az értékesítés adatainak AFE-ben való rögzítése nélkül, illetve a 3. mellékletében nevesített események bekövetkezése az AFE-ben minden esetben rögzítésre kerüljön.

## BC) Az adatok rögzítése és kiolvasása

## 17. Az AFE-nek az értékesítésre vonatkozó adatok mellett rögzítenie kell az automata alábbi adatait és eseményeit is:

## a) az automata be- és kikapcsolása,

## b) az automata blokkolt állapotba kerülése, illetve a blokkolt állapot feloldása,

## c) az AFE áramellátásának megszűnése és újraindulása,

## d) a NAV szerverével való kommunikáció,

## e) az AFE órájának átállítása.

## 18. az automata, illetve az AFE működésére, állapotára, illetve kommunikációjára vonatkozó adatok a 3. mellékletben foglaltak szerint.

## BD) Hardverkövetelmények

## 19. Az AFE-nek legalább akkora saját, a tápellátás megszűnésekor adatot megőrző tárkapacitással kell rendelkeznie, ami lehetővé teszi a FSZ által kialakított naplózási struktúrában legalább 10 napnyi szokásos üzletmenetre vonatkozó adat tárolását abban az esetben, ha a az AFE és a FSZ közötti adatkapcsolat az elektronikus hírközlő hálózat elérhetőségének hiányából nem építhető ki. Az alkalmazott technológiának legalább 10 000 újraírást kell lehetővé tennie.

## 20. Az AFE adattartalmához való hozzáférés és az adattartalmon végzett bármilyen külső beavatkozás kizárólag az e rendeletben foglaltak szerint, a FSZ által vagy annak engedélyével lehetséges.

## 21. Az AFE-t úgy kell kialakítani, hogy az AFE tápellátásának megszűnésekor a tápellátás megszűnésének tényét a naplóállományba bejegyezni és az aktuálisan nyitott naplóállományt annak sérülési veszélye nélkül lezárni legyen képes.

## 22. Az AFE minden bejegyzését ellenőrző kóddal látja el és azokat naplózza.

## 23. Az AFE-nek képesnek kell lennie legalább három magyarországi elektronikus hírközlési szolgáltató mobil földfelszíni hálózatára felkapcsolódni, és az így létrejött adatkapcsolattal az AFE-ben naplózott adatoknak továbbítására a FSZ számára.

## 24. Az AFE-nek a gyártó által beépített, és kizárólagosan a FSZ szerverével való adatkapcsolat biztosítására alkalmas, áramkörbe eltávolíthatatlanul integrált SIM-modult (MIM , SIM-chip) kell tartalmaznia.

## 25. Az AFE-t alkalmassá kell tenni külső antenna csatlakoztatására.

## 26. Az AFE-re csak az e rendeletben megengedett eszközöket lehet csatlakoztatni az alábbiak szerint:

## a) egy-egy adatkapura az automata központi egységét, illetve az egyes fizetőeszköz vizsgáló egységeket (érmevizsgáló, kártyaterminál, stb.),

## b) a külső antenna csatlakozóját,

## c) az AFE-n a műszerész által végzett műveletek céljából adatbevitelre szolgáló csatlakozót.

## 27. Az AFE-n a 26. pontban megjelölteken túl további vezérlőket, ki- vagy bemeneti csatlakozókat elhelyezni tilos.

## 28. Az AFE engedélyezett vezérlő és csatlakozó portjai az automatáról kaphatnak tápellátást, azokat az AFE tápellátása nem táplálhatja.

## 29. Az AFE-t saját órával kell ellátni a dátum és a pontos idő mérésére. Az AFE naplóállományaiban a bejegyzések időpontját az AFE órája szerint kell feltüntetni. Az órát legalább hetente egyszer szinkronizálni kell a mobilhálózattal és/vagy a FSZ által biztosított idő szerverrel úgy, hogy a téli és nyári időszámítások közötti váltások alkalmával az AFE óra átállítására haladéktalanul, de legkésőbb az óraállítás hivatalos időpontját követő első értékesítés előtt sor kerüljön.

## 30. Az AFE-be a gyártónak ipari beágyazású, magyarországi mobilhálózaton csomagkapcsolt adatátvitelre alkalmas GSM modult kell beépítenie, legalább multi-slot class 12 besorolással.

## BE) Az AFE adatszolgáltatásának technológiája

## 31. Az AFE a FSZ rendszerén keresztül a NAV szerverrel vel titkosított kapcsolatot alakít ki, amelynek publikus és privát kulcsát az AFE gyártó kezdeményezésére a FSZ szolgáltatja. A titkosított kapcsolat kialakításához szükséges publikus és privát kulcs rendelkezésre bocsátásának rendjét a FSZ holnapján közleményben teszi közzé. Az AFE és a FSZ szerver közötti titkosított kapcsolathoz szükséges kulcskezelő és nyilvántartó rendszert (PKI) a FSZ biztosítja. Az AFE-nek képesnek kell lennie ezzel a rendszerrel együttműködni.

## 32. Az AFE-nek nem lehet érvényes, nyilvános hálózaton való azonosítást lehetővé tevő IP-címe. Az AFE kizárólag a FSZ-val folytathat kommunikációt kivéve a kártyás fizetési banki kommunikációt.

## BF) Biztonsági követelmények

## 33. Biztosítani kell az automata és AFE megbonthatatlan egységét és egyedi azonosíthatóságát. Az AFE automatába történő be, fel illetve onnan történő ki vagy leszerelését kizárólag az e rendelet szerint a FSZ végezheti.

## 34. Az AFE-nek képesnek kell lennie

## a) a FSZ által kibocsátott Device Certificate biztonságos tárolására és kezelésére,

## b) a TLS 1.1 vagy újabb verziójú szabvány szerinti titkosítási eljárás támogatására. A támogatott legfrissebb verzió számát a FSZ honlapján teszi közzé,

## c) Device Certificate alapon azonosítania magát,

## d) az adatkapcsolat kiszolgálására a meglévő nyilvános mobilkommunikációs hálózatokon keresztül,

## e) a TCP/IP protokollt alkalmazására az AFE szabványos kommunikációhoz,

## f) a rajta futó szoftver, vagy a naplófájlokat tároló hardverelem megváltozásának érzékelésére, ilyen esetben az AFE-nak blokkolt állapotba kell kerülnie,

## 35. Az AFE a kriptográfiai funkciók (rejtjelezés, hitelesítés, kulcstárolás) megvalósításában biztonsági modulra kell támaszkodjon, amely áramköri (chip) szinten FIPS 140-2 szabvány szerint legalább Level 1 vagy common criteria EAL3 minősítéssel rendelkezik.

## 36. Az AFE kriptográfiai modulnak képes kell lennie a 2048 bit hosszúságú RSA aszimmetrikus kulcsok kezelésére

## 37. Az AFE-ben a naplófájlok és egyéb adatok tárolását titkosítottan kell megvalósítani úgy, hogy azok hatóság számára a sértetlen tárolóegységről az automata, illetve az AFE meghibásodása esetén is kinyerhetőek legyenek a FSZ által (hatósági kiolvasás).

## BG) Az AFE beágyazott GSM moduljával szembeni követelmények:

## 38. Az AFE-nek képesnek kell lennie a magyarországi mobilhálózatokon GPRS technológiával, valamint az EDGE, HSDPA, UMTS, LTE technológiák egyikével történő adattovábbításra (továbbiakban: csomagkapcsolt adatátvitel),

## 39. Az AFE-be épített SIM modulnak meg kell felelni az ETSI M2M UICC standard (TS 102.671) szabványban foglaltaknak.

## 40. Az AFE minimum vételi teljesítményszintje -102dBm, a készülék bemeneti kapcsaira vonatkoztatva, valamint a szükséges C/I (jel/interferencia viszony) 10 dB, az ETSITS0508V050100, valamint az ETSI EN 151.010 szabványoknak megfelelően,

## 41. A SIM hálózatkeresési preferencialistáját, mellékelni kell az AFE engedélyezési dokumentációjához.

## BH) AFE működtető szoftver tanúsítása

## 42. Az AFE-ben működő szoftver működésének helyességét és a rejtett funkcióktól való mentességét, a FSZ-tól és az AFE gyártójától független értékelésen alapuló, 8-9. § szerinti tanúsító szervezet által kiállított tanúsítvánnyal kell alátámasztani.

## 43. Az AFE gyártási folyamatának végén a független tanúsító szervezet kontrollja alatt működtetett biztonsági inicializálást kell végrehajtani.

## BI) AFE szoftverének frissítése

## 44. Az AFE-nek alkalmasnak kell lennie a benne működő szoftver egyes komponenseinek, vagy egészének a FSZ szerveréről történő távoli frissítésére. Az AFE-n futó szoftver csak egy folyamatban frissíthető.

## C) Az euró átálláshoz kapcsolódó szabályok

## 45. Az euró bevezetésének, azaz a forint forgalomból való kivonásának és az euró hivatalos pénznemmé tételének időpontja előtt az AFE naplóállományaiban szereplő, pénzösszegre vonatkozó adatokat forintban, egész számként kell feltüntetni. Ezen időpontot követően az adatokat euróban, két tizedesjegy pontossággal kell feltüntetni.

## 46. Az euró hivatalos pénznemmé tételének időpontját követően, de még az ezt követő első értékesítést megelőzően az AFE-nek napzárást kell végrehajtania, amiben az (előző) ponttól eltérően a pénzösszegeket forintban tünteti fel. Az euró módban történő első értékesítés csak akkor hajtható végre, ha az üzemeltető az AFE-be történő manuális adatbevitellel jelezte, hogy az automata összegeinek eurós értékesítésre történő átprogramozása megtörtént.

## 47. Az euró átállás végrehajtásának az AFE-ben megfordíthatatlannak kell lennie.

## 48. Az euró átállás végrehajtását az AFE-ben vezetett naplóállományban az „Euró üzemmód beállítása” esemény bejegyzésével kell rögzíteni a 4. mellékletben foglaltak szerint.

## 49. Az euró átállás dátumát a NAV üzenetben közli az AFE-vel a 3. mellékletben foglaltak szerint. Az AFE-nek képesnek kell lennie ezen üzenet alapján az esemény időpontját megfelelően beállítani.

2. melléklet a 31/2016. (IX. 2.) NGM rendelethez
