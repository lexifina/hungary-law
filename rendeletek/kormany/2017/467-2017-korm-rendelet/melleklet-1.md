1. melléklet a 467/2017. (XII. 28.) Korm. rendelethez[^12]

1. KAK Hoszting szolgáltatás

A szolgáltatás keretében a központi szolgáltató a Kormányzati Adatközpontban zárt, folyamatos felügyelet alatt működő géptermi környezetben nyújtott területhasználati vagy technológiai betelepülési lehetőséget biztosít. A szolgáltatás célja, hogy lehetőséget biztosítson a felhasználók számára saját informatikai eszközök elhelyezésére a szolgáltató által működtetett géptermekben. A központi szolgáltató a Kormányzati Adatközpontot úgy alakítja ki, hogy általa nagybiztonságú fizikai és műszaki üzemeltetési környezetet biztosítson a kijelölt eszközök számára.

2. KAK Virtuális adatközpont szolgáltatás

A KAK – Virtuális adatközpont szolgáltatás keretében erőforráskvóták kerülnek definiálásra. Az erőforráslimiteken (erőforráskvótákon) belül tetszőlegesen hozhatók létre az erőforráskvótákat felhasználó alszolgáltatások és kiegészítő szolgáltatások.

2.1. Alszolgáltatások

Alszolgáltatásnak nevezzük azon szolgáltatásokat, amelyeken keresztül a KAK Virtuális adatközpont erőforrásai igénybe vehetők. Az alszolgáltatások részletes leírását a központi szolgáltató ellátási szolgáltatáskatalógusa tartalmazza.

2.1.1. KAK – Virtuális szerver alszolgáltatás

A Szolgáltató az Adatközponti szolgáltatásban kötelezően igénybe veendő alszolgáltatás keretében biztosítja a Felhasználói számára a KAK Felhő erőforrásait IaaS szolgáltatási formában.

A gépek különböző zárt, virtuális hálózati szegmensekbe (VLAN) szervezhetők, melyek között az adatáramlást – tűzfalon keresztül – szabályok alapján lehet engedélyezni. A létrejövő architektúrán üzembe állítható a Felhasználó számára a saját infrastruktúrája.

2.1.2. KAK – Konténer alszolgáltatás

A szolgáltatás az iparágban szabványos konténer futtatását biztosítja egy vezérlési és skálázási réteg segítségével. Ez a réteg lehetővé teszi a konténerek automatizált üzembe helyezését, szükség esetén egy előző verzióra történő visszaállítását, terheléselosztót biztosít a konténerek elé, valamint figyeli a konténerek állapotát, és ha hibát észlel, újraindítja azokat.

A központi szolgáltató üzemeltetése nem végez műveleteket a konténeren belül, ezért a konténeren belül használt technológiára nincs megkötés. Azonban a különböző, nem konténerizálható szolgáltatásokat (például az adatok perzisztens tárolása NAS-eszközön vagy SQL-adatbázisban) a sztenderd KAK alszolgáltatások és kiegészítő szolgáltatások közül kell igénybe venni.

2.1.3. KAK – Alkalmazáskiszolgáló alszolgáltatás

Az alszolgáltatás keretében a Szolgáltató Alkalmazáskiszolgáló szolgáltatás keretében biztosítja a Felhasználó számára a KAK Felhő erőforrásait PaaS szolgáltatási formában.

Szolgáltatás keretében komplex konténerszolgáltatásként gyártói támogatással rendelkező konténerkezelő környezet elhelyezését biztosítja a központi szolgáltató. Ez azt jelenti, hogy biztosítja a virtuális futtatókörnyezethez az olyan, alkalmazásprogramozási felület (API) szintű hozzáférést a konténerkezelő környezet számára, amely lehetővé teszi konténereket futtató virtuális gépek (az úgynevezett worker node-ok) automatikus fel- vagy leskálázását konténerkezelő platform oldalról. A Szolgáltató licenceket konténerkezelő platform futtatásához nem biztosít.

2.1.4. KAK – Levelezés, csoportmunka alszolgáltatás

A központi szolgáltató olcsó, könnyen skálázható, modern, webalapú levelező és csoportmunka alszolgáltatást biztosít, amely megfelelően támogatja a felhasználókezelést. Az alszolgáltatás célja, hogy teljeskörűen kiváltsa az ingyenes, illetve publikus levelezési szolgáltatások kormányzati célú felhasználását.

2.1.5. KAK – Dokumentumkezelő rendszer alszolgáltatás

A központi szolgáltató olcsó, könnyen skálázható, modern, webalapú dokumentumkezelő alszolgáltatást biztosít, amely keretében minden felhasználó számára külön alkalmazáskörnyezet kerül kialakításra virtuális infrastruktúra szinten. Az alszolgáltatást biztosító szabad szoftveres alkalmazáshoz adminisztrátor jogosultságot kap a tenant adminisztrátor, azonban a dokumentumkezelő alkalmazás alatt levő operációs rendszerben és adatbázis-kezelőben nem kap jogosultságokat. Az alszolgáltatás beépítetten tartalmaz vírusvédelmi szolgáltatást.

2.1.6. KAK – Tartalomkezelő rendszer alszolgáltatás

A Szolgáltató Tartalomkezelő rendszer szolgáltatás keretében biztosítja a Felhasználó számára a KAK Felhő erőforrásait SaaS szolgáltatási formában. Az alszolgáltatás keretében a Szolgáltató külön VM-en települő tartalomkezelő alkalmazás szolgáltatást nyújt.

2.1.7. KAK – E-Learning rendszer alszolgáltatás

Az alszolgáltatás célja egy közös kormányzati platform kialakítása, amely használata hatékonnyá és követhetővé teszi a belső képzések lebonyolítását. E-Learning alszolgáltatásként a központi szolgáltató nyílt forráskódú platformot szolgáltat. Minden felhasználó külön szeparált környezetet vagy környezeteket kap.

2.1.8. KAK – Naplógyűjtő rendszer alszolgáltatás

Az alszolgáltatás keretében a Szolgáltató külön VM-en települő naplóállomány-gyűjtő alkalmazás szolgáltatást nyújt Felhasználói számára a Felhasználó saját környezetében. Az alkalmazás szeparációja VM és hálózati (VLAN) szinten valósul meg. Az alszolgáltatás által lefoglalt erőforrások a KAK – Virtuális Adatközpont szolgáltatás kvótáiból kerül felhasználásra.

2.2. Kiegészítő szolgáltatások

Kiegészítő szolgáltatásnak nevezzük azon szolgáltatásokat, amelyek önállóan nem, csak valamely ellátási szolgáltatás vagy alszolgáltatás kiegészítéseként lehet igénybe venni. Az ellátási szolgáltatások mellé igényelhető kiegészítő szolgáltatások részletes leírását a központi szolgáltató ellátási szolgáltatáskatalógusa tartalmazza.

2.2.1. KAK – Tárterület – Blokk alapú kiegészítő szolgáltatás

A Szolgáltató a Tárterület – Blokk alapú kiegészítő szolgáltatás keretében additívdiszk-erőforrásokat biztosít a Felhasználó számára a KAK Felhőből, kiegészítő szolgáltatás formájában a KAK – Virtuális Adatközpont szolgáltatásban meghatározott felső korlát erejéig. Block device tárhelyszolgáltatás keretében további diszk erőforrások adhatók meglevő virtuális gépekhez. Az addicionális tárterület bekonfigurálása, csatolása, illetve fájlrendszer létrehozása az operációs rendszer szintet üzemeltető feladata (IaaS szolgáltatás esetén a Felhasználó feladata).

2.2.2. KAK – Tárterület – NAS alapú kiegészítő szolgáltatás

A Szolgáltató a Tárterület – NAS alapú kiegészítő szolgáltatás keretében hálózati tárhelyet biztosít a Felhasználó számára a KAK Felhőből a KAK Felhő – Virtuális Adatközpont szolgáltatásban meghatározott felső korlát erejéig. A KAK Felhőbe települő alkalmazások számára gyakran szükséges közös, hálózati tárhely. A hálózati tárhelyet Szolgáltató CIFS és NFS alapú tárhely alapján központi NAS (Network Attached Storage) segítségével biztosítja.

2.2.3. KAK – Tárterület – Objektumtár alapú kiegészítő szolgáltatás

A Szolgáltató a Tárterület – Objektumtár alapú kiegészítő szolgáltatás keretében – objektumalapú adattárolást biztosít a Felhasználó számára a KAK Felhőből a KAK – Virtuális Adatközpont szolgáltatásban meghatározott felső korlát erejéig. A Felhő által biztosított OpenStack Object Storage (SWIFT) egy magas rendelkezésre állású, elosztott, konzisztens object/blob tároló. Az objektumok létrehozása, módosítása és kivétele Object Storage API-n keresztül történik, ami Representational State Transfer (REST) webszervizekként került implementálásra. Az objektumok dedikált konténerben kerülnek elhelyezésre.

2.2.4. KAK – Mentés-visszaállítás kiegészítő szolgáltatás

A Szolgáltató a Mentés-visszaállítás kiegészítő szolgáltatás keretében agent és image alapú mentést és mentés-visszaállítást biztosít Felhasználó számára. A KAK Felhő által biztosított felhő alapú működési környezetben beállítható mentés mind komplett virtuális gép (image szintű mentés), mind agent alapú mentés formájában. A mentés DDT (disc-to-disc-to-tape) formában kerül megvalósításra. A mentéseknek a VTL-ről a tape library-ba való ütemezését Szolgáltató végzi.

2.2.5. KAK – Archiválás kiegészítő szolgáltatás

Törvényességi vagy egyéb funkcionális szempontoknak megfelelően szükség lehet teljes szolgáltatások vagy akár a komplex alkalmazási rendszerek és kapcsolódó adatbázisok együttes állapotának hosszú távú, konzisztens és bizalmas megőrzésére. A Felhasználók számára a felhő ezt a típusú/szintű archiválást az előző alfejezetben részletezett mentés analógiájára, teljes konfigurációk (adatbázis és alkalmazási platformok), adatbázisok vagy egyéb tárterületek teljes körű mentésének hosszú távú megőrzésével biztosítja.

2.2.6. KAK – Nagyvállalati szintű relációs adatbázis-kezelő, zárt forráskódú adatbázis kiszolgáló szolgáltatás

A Szolgáltató a kiegészítő szolgáltatás keretében biztosítja a Felhasználó számára a KAK Felhő erőforrásait. A kiegészítő szolgáltatás futtatásához szükséges számítási erőforrásokat a Szolgáltató egy dedikált virtuális erőforrás pool-ból vagy fizikai gépeken szolgáltatja. Az erőforrás pool-ban a számítási kapacitást rack szerverek, a tárolási kapacitást pedig a központi tároló által kerülnek biztosításra. A Felhasználók adatbázisainak futtatásához virtuális gépek kerülnek létrehozásra a két telephelyen. A szolgáltatás szintű, magas rendelkezésre állást és a katasztrófatűrő megoldást is a telephelyek között átnyúló fürtözési technológia adja.

2.2.7. KAK – Nyílt forráskódú relációs SQL adatbázis kezelő szolgáltatás

A Szolgáltató SQL adatbázisszolgáltatás (MariaDB, PostgreSQL) keretében biztosítja a Felhasználó számára a KAK Felhő erőforrásait PaaS/DBaaS jellegű szolgáltatási formában. A szolgáltatás által lefoglalt erőforrások a KAK – Virtuális Adatközpont szolgáltatás kvótáiból kerül felhasználásra. Az alszolgáltatás keretében a Szolgáltató külön VM-ken MariaDB és PostgreSQL alapú image-eket biztosít, amelyeken adatbázis-szolgáltatást nyújt a Felhasználó számára.

A szerver virtualizáció a szeparációt és a magas rendelkezésre állást is fizikai szinten biztosítja. A magas rendelkezésre állást, a horizontális skálázást és a hibatűrést (katasztrófaelhárítást) a platform szinten elérhető Multi-Master replikáció valósítja meg. Minden Felhasználói szolgáltatás esetén több példány alkalmazható a horizontális skálázás biztosítására, illetve a telephelyek közötti replikációval a katasztrófa jellegű meghibásodások kezelésére.

2.2.8. KAK – Nyílt forráskódú nem relációs adatbázis kezelő szolgáltatás

A nem relációs adatbáziskezelő a webes alkalmazások jelentős mennyiségű párhuzamos feldolgozási igényeinek kiszolgálását, a gyorsító tárak hatékonyabb és az adatstruktúrák rugalmasabb kezelését, valamint azok jobb skálázási lehetőségeit biztosító adatbázis platform szolgáltatás. Az adatbázis belső tárolási struktúrája kulcs-érték párok és dokumentumok tárolására, illetve kezelésére optimalizált. A Szolgáltató NoSQL adatbázis (MongoDB) alszolgáltatás keretében biztosítja a Felhasználó számára a KAK Felhő erőforrásait PaaS/DBaaS jellegű szolgáltatási formában. A szolgáltatás által lefoglalt erőforrások a KAK – Virtuális Adatközpont szolgáltatás kvótáiból kerül felhasználásra. A külön VM-eken települő MongoDB alapú adatbázis szolgáltatást nyújt a Felhasználói számára. A szerver virtualizáció a szeparációt infrastruktúra szinten, és a magas rendelkezésre állást is alapszinten biztosítja. A magas rendelkezésre állást és katasztrófatűrést a platform szinten elérhető replikációs megoldás támogatja.

2.2.9. KAK – Perimeter kiegészítő szolgáltatás

A Szolgáltató a Perimeter kiegészítő szolgáltatás keretében tűzfal, webalkalmazás-tűzfal, SSL-terminálás, terheléselosztás funkciót biztosít.

2.2.9.1. Webalkalmazás-tűzfal (WAF)

A perimeter eszköz beépítve tartalmazza az elterjedtebb, általános, webalapú támadások, például XSS, SQL-Injection elleni védelmet.

2.2.9.2. Tűzfal funkciók

A perimeter eszközön ezzel a funkcionalitással lehetséges szabályozni a Felhasználó VLAN-jai és a különböző zónák (a felhőben levő egyéb VLAN-ok, NTG, Internet, hostingban levő szerverek) közötti adatáramlást.

2.2.9.3. Terheléselosztás

A szolgáltatás nagy teljesítményű hardveres terheléselosztást biztosít a felhő határát képező perimeter eszköz segítségével.

2.2.9.4. SSL terminálás, kliens oldali tanúsítványkezelés

A központi szolgáltató a 186/2015. kormányrendelet alapján biztosítja az SSL terminálást.

Ebben az esetben az ügyfélnek adatkezelési megállapodást kell kötnie a Szolgáltatóval. Az adatkezelés részeként az ügyfél a Szolgáltató részére átadja az SSL/TLS-bontáshoz a tanúsítványhoz tartozó privát kulcsot, amit a Szolgáltató kizárólagosan a titkosítás feloldásához használ fel. A Szolgáltató által biztosított eszközön történő, titkosított kapcsolat terminálása és felépítése a bérlő részére nem jelent járulékos feladatot. A tanúsítvánnyal kapcsolatos adminisztratív teendők: lejárat figyelése, megújítás, visszavonás az ügyfél felelőssége és feladata.

Az SSL/TLS terminálásával szerverek felé a KAK belső hálózatán már csak a titkosítás nélküli forgalom kerül elküldésre.

2.2.10. KAK – Fix publikus IP-cím kiegészítő szolgáltatás

A Szolgáltató a Fix publikus IP-cím kiegészítő szolgáltatás keretében fix, publikus IP-címet biztosít a Felhasználó számára a KAK – Virtuális Adatközpont szolgáltatásban meghatározott felső korlát erejéig. A kiegészítő szolgáltatás keretében a Szolgáltató fix, publikus IP-címet biztosít a Felhasználó számára, a rendelkezésére álló IP-címtartományából. Ez az IP-cím jellemzően a határvédelmi (perimeter) eszközön lesz beállítva, és azt biztosítja, hogy a Felhasználó által kialakított szolgáltatások az Internet felől is elérhetőek legyenek.

[^12]: Az 1. melléklet az 572/2020. (XII. 9.) Korm. rendelet 118. § (1) bekezdésével megállapított szöveg.
