## 15–16. §[^1]

1. melléklet a 467/2017. (XII. 28.) Korm. rendelethez

1. KAK Hoszting szolgáltatás

A szolgáltatás keretében a központi szolgáltató a Kormányzati Adatközpontban zárt, folyamatos felügyelet alatt működő géptermi környezetben nyújtott területhasználati vagy technológiai betelepülési lehetőséget biztosít. A szolgáltatás célja, hogy lehetőséget biztosítson a felhasználók számára saját informatikai eszközök elhelyezésére a szolgáltató által működtetett géptermekben. A központi szolgáltató a Kormányzati Adatközpontot a TIER-3-as követelményeknek megfelelően alakítja ki, amely által nagybiztonságú fizikai és műszaki üzemeltetési környezetet biztosít a kijelölt eszközök számára.

2. KAK Felhő szolgáltatások

A KAK Felhő egy informatikai felhő, mely az alábbi szolgáltatásokat nyújtja:

2.1 Infrastruktúra szintű ellátási szolgáltatások (IaaS)

3. Virtuális szerver szolgáltatás

A virtuális szerver szolgáltatás keretében definiálásra kerül egy virtuális gép (szoftveresen szimulált számítógép), a gépekhez tartozó minimum és maximum értékek közötti paraméterekkel együtt. A gépek különböző zárt virtuális hálózati szegmensekbe szervezhetők, melyek között az adatáramlást – tűzfalon keresztül – szabályok alapján lehet korlátozni. A virtuális szerverre telepítendő operációs rendszerekről, alkalmazásokról és ezeknek forrásairól, licenceiről a felhasználónak szükséges gondoskodnia. Erőforrások későbbi módosítása technológiailag megvalósítható szerződésmódosítás és előzetes jóváhagyást követően. A könnyebb telepíthetőség és biztonsági előírásoknak való megfelelés, valamint a hatékonyabb üzemeltetés érdekében a központi szolgáltató által biztosított képfájlokat, template-eket biztosít a telepítéshez.

4. Virtuális adatközpont szolgáltatás

A virtuális adatközpont szolgáltatás keretében definiálásra kerülnek erőforrás limitek, amiken belül tetszőlegesen létrehozható egy vagy több virtuális gép a felhasználó számára. A gépek különböző zárt virtuális hálózati szegmensekbe szervezhetők, melyek között az adatáramlást – tűzfalon keresztül – szabályok alapján lehet korlátozni. Az előre definiált limitek határáig lehetőség van az erőforrások dinamikus használatára.

5. Docker konténer szolgáltatás

A virtuális szerver szolgáltatáshoz hasonló szolgáltatás, mely esetben a szolgáltatások esetenként kedvezőbb licenc konstrukcióban érhetők el. Docker konténer esetében a központi szolgáltató üzemeltetése csak a Docker konténeren végez műveleteket (például konténer indítása vagy leállítása), a konténeren belül nem, ezért a konténeren belül használt technológiára nincs megkötés, de a központi szolgáltató üzemeltetése segítséget nem nyújt a konténeren belüli hibák elhárításához. A Docker konténer állapotmentes, így mentésre nincs szükség. Alternatívaként tárhely alapú kiegészítő szolgáltatásokra lehet felhasználói paraméterezéssel mentéseket elhelyezni.

5.1 Adatbázis kiszolgáló szolgáltatások (DBaaS)

DBaaS szolgáltatást infrastruktúra tervezési és biztonságtechnikai okokból a központi szolgáltató kizárólag kiegészítő szolgáltatásként biztosít. Ennek megfelelően a szolgáltatások leírásai a „22. Adatbázis kiszolgáló szolgáltatás (DBaaS)” pontnál találhatóak.

5.2 Platform szintű ellátási szolgáltatások (PaaS)

A PaaS szolgáltatás olyan szoftver-keretrendszert futtató környezetet biztosít, amely alkalmazásokat képes futtatni. A szolgáltatás igénybevételével előre definiált alkalmazás sablon alapú alkalmazás-kiszolgálót lehet igénybe venni virtuális gép alapon. Az alkalmazás szerver felhasználói elhatárolása az IaaS-hoz hasonlóan virtuális szerver és virtuális hálózati szinten valósul meg. A szolgáltatás erőforrásainak paraméterei, a virtuális géphez hasonlóan választható ki.

A PaaS szintű szolgáltatások esetén általánosan elmondható, hogy a központi szolgáltató által biztosított szintig az üzemeltetést a központi szolgáltató végzi. Ez azt is jelenti többek között, hogy a központi szolgáltató rendszeres, előre bejelentett, tervezhető időközönként telepíti a javítócsomagokat (patch) először a fejlesztői, teszt, oktatói környezetekben, majd az éles környezetben is. A központi szolgáltató csak egy stabil verziójú szoftver kiadást üzemeltet a platform szolgáltatásokban.

Szolgáltatás keretében Java (JVM), .NET kiszolgáló, Python kiszolgáló és PHP kiszolgáló környezeteket biztosítja a központi szolgáltató.

5.3 SaaS szintű ellátási szolgáltatások

Szoftver szintű szolgáltatások esetében a szolgáltatást biztosító alkalmazás, illetve az alatta levő operációs rendszer rendszeres frissítéséről és mentéséről központi szolgáltató gondoskodik. A mentés visszaállítást külön Service Desk jegyben lehet kérni.

6. Levelezés, csoportmunka szolgáltatás

A központi szolgáltató olcsó, könnyen skálázható, modern, web alapú levelező- és csoportmunka szolgáltatást biztosít, amely megfelelően támogatja a felhasználókezelést. A szolgáltatásként történő igénybevétel és a gyors bevezetés különösen újonnan alakuló, vagy elavult rendszert használó szervezetek számára lehet előnyös. A szolgáltatás célja, hogy teljeskörűen kiváltsa az ingyenes, illetve publikus levelezési szolgáltatások kormányzati célú felhasználását.

7. Dokumentumkezelő szolgáltatás

A központi szolgáltató olcsó, könnyen skálázható, modern, web alapú dokumentumkezelő szolgáltatást biztosít, amely keretében minden felhasználó számára külön alkalmazás környezet kerül kialakításra virtuális infrastruktúra szinten. A szolgáltatást biztosító szabad szoftveres alkalmazáshoz adminisztrátor jogosultságot kap a tenant adminisztrátor, azonban a dokumentumkezelő alkalmazás alatt levő operációs rendszerben és adatbázis kezelőben nem kap jogosultságokat. A szolgáltatás beépítetten tartalmaz vírusvédelmi szolgáltatást.

8. Tartalomkezelő szolgáltatás

A szolgáltatás keretében a központi szolgáltató Drupal alapú tartalomkezelőt szolgáltat. A tenant kezelést nem a Drupalon belül kerül megoldásra, hanem minden tenant külön szeparált Drupal környezetet vagy környezeteket kap. A Drupal adminisztrátor jogosultságot megkapja a tenant adminisztrátor, a Drupal alatt levő operációs rendszerben, illetve adatbázis kezelőben viszont nem kap jogosultságokat. A Drupal szolgáltatás ClamAV vírusvédelmi megoldást tartalmaz beépítetten.

9. E-Learning szolgáltatás

A Szolgáltatás célja egy közös kormányzati platform kialakítása, amely használata hatékonnyá és követhetővé teszi a belső képzések lebonyolítását. E-Learning szolgáltatásként a központi szolgáltató a Moodle nyílt forráskódú platformot szolgáltatja. Minden felhasználó külön szeparált Moodle környezetet vagy környezeteket kap. A Moodle adminisztrátor jogosultságot megkapja a tenant adminisztrátor, a Moodle alatt levő operációs rendszerben, illetve adatbázis kezelőben viszont nem kap jogosultságokat. A Moodle szolgáltatás ClamAV vírusvédelmi megoldást tartalmaz.

9.1 Kiegészítő szolgáltatások

Kiegészítő szolgáltatásnak nevezzük azon szolgáltatásokat, amelyek önállóan nem, csak valamely ellátási szolgáltatás kiegészítéseként lehet igénybe venni. Az ellátási szolgáltatások mellé igényelhető kiegészítő szolgáltatásokat a központi szolgáltató ellátási szolgáltatáskatalógusa tartalmazza.

10. Adatközponti alap szoftver infrastruktúra szolgáltatások

Az adatközpontokban szokásos szoftver infrastruktúra elemek szolgáltatásait nyújtja a kialakított megoldás:

– SMTP szolgáltatás belső- vagy Internet felé küldendő levelezéshez,

– NTP szolgáltatás,

– DNS szolgáltatás.

11. Több privát IP cím

Amennyiben valamelyik szolgáltatás szükségessé teszi több privát IP cím felvételét, úgy a virtuális gépeknek automatikusan kiosztott IP címek mellé a VLAN méretéig további IP címek foglalhatóak.

12. Fix publikus IP cím

A kiegészítő szolgáltatás keretében fix külső, publikus IP cím szolgáltatás rendelhető korlátozott mennyiségben. A nyilvános IP címekkel történő gazdálkodást és a címek Felhasználó részére történő kiosztását a központi szolgáltató végzi. Maga a publikus IP cím a felhő esetén a perimeter eszközön lesz beállítva, mint ami a szolgáltatást publikálja. A hosting környezet esetében az ügyfél valamelyik eszközén (legtöbb esetben tűzfalán) történik a beállítás.

13. Tárhely szolgáltatás [IaaS (block device) alapú kiegészítő szolgáltatás]

Block device tárhely szolgáltatás keretében további diszk volume-ok (például vmware alatt vmdk-k) adhatók meglevő virtuális gépekhez. A tárterület bekonfigurálása, csatolása, illetve fájlrendszer létrehozás a tárterület felett annak a feladata, aki az operációs rendszer szintet üzemelteti. Azaz IaaS szolgáltatásnál a felhasználó feladata, magasabb szintű szolgáltatásnál a központi szolgáltató feladata.

Technikai okok miatt egy diszk volume mérete korlátozott. A korlátnál nagyobb méret esetén több volume-ot kell igényelni, és azokat (guest) operációs rendszer szinten kell összefogni.

14. Objektumtár szolgáltatás (IaaS alapú kiegészítő szolgáltatás)

A felhő által biztosított OpenStack Object Storage (SWIFT) egy magas rendelkezésre állású, elosztott, konzisztens object, illetve blob tároló. Az objektumok létrehozása, módosítása és kivétele Object Storage API-n keresztül történik, ami Representational State Transfer (REST) web szervizekként került implementálásra.

15. Fájlkiszolgáló (NAS) (IaaS alapú kiegészítő szolgáltatás)

A KAK Felhőbe települő alkalmazások számára gyakran szükséges közös hálózati tárhely. A preferált megoldás ilyenkor az előző pontban említett objektumtár használata, de szükség esetén CIFS és NFSv4 alapú tárhelyet központi NAS (Network Attached Storage) segítségével tudják biztosítani.

NAS storage-ból technikai korlátok miatt tenantonként egy darab NFSv4 és egy darab CIFS vehető igénybe.

16. Terheléselosztás

A szolgáltatás nagyteljesítményű hardveres terheléselosztást biztosít a felhő határát képező perimeter eszköz segítségével L4 vagy L7 szinten.

17. SSL terminálás, kliens oldali tanúsítvány kezelés

A KAK Felhőn belül az adatok alapesetben titkosítás nélkül kerülnek továbbításra. Az SSL terminálást, azaz az SSL kapcsolatok (mint például a HTTPS kapcsolatok) esetén a komoly számítási kapacitást igénylő titkosítási folyamat központi kezelését a felhő határát képező perimeter eszköz biztosítja, így az alkalmazás szerverek felé már csak a titkosítás nélküli forgalom kerül elküldésre.

Ennek a szolgáltatásnak egy alesete, amikor a felépített SSL csatornán a kliens (a kezdeményező) is SSL tanúsítvánnyal azonosítja magát annak bizonyítása érdekében, hogy jogosult igénybe venni a szolgáltatást. A kliens lehet, egy Internet felől érkező ügyfél, de lehet egy szolgáltatást igénybe vevő alkalmazás szerver is. Ilyen esetben megadható, hogy az SSL terminálást végző eszköz ellenőrizze, hogy

– a kapott kliens oldali tanúsítvány érvényes-e (nem járt le, nem vonták vissza),

– az előre beállított aláíró tanúsítvánnyal írták-e alá.

Lehetséges olyan megoldás, amikor az alkalmazás titkosított adatfolyamát nem a perimeter eszköz terminálja, hanem csak átengedi L4 szinten és a titkosítást az alkalmazás oldja fel. Az ilyen esetekben azonban – lévén az alkalmazás VLAN-jában nem csak titkosítatlan adatok forgalmazása történik – a kötelező NKI EWS (Early Warning System – korai riasztási rendszer)-hez való csatlakozás a tenant felhasználójának a feladata, egyéb esetekben ezt a KAK Felhő megoldja.

18. Naplózási szolgáltatás

A központi szolgáltató a szolgáltatási katalógusban szereplő IaaS, PaaS és SaaS szinteken maga végzi a napló állományok gyűjtését és elemzését.

Az előző pontban nem meghatározott napló állományok felett létrejött naplók kezelésére a Felhasználó kiegészítő szolgáltatásként igénybe vehet naplógyűjtő szolgáltatást a szolgáltatási katalógusban meghatározott feltételek szerint.

Naplóállományok hozzáférhetősége:

Az igénybe vett kiegészítő szolgáltatáshoz a központi szolgáltató 30 napos hozzáférhetőséget biztosít a Felhasználó számára.

– A központi szolgáltató a Felhasználó számára a napló állományokhoz való hozzáférést kizárólag olvasási jogosultsággal biztosítja.

– A központi szolgáltató rögzíti a Felhasználó által a napló állományokhoz való hozzáférés módját, idejét és tevékenységét.

IaaS, PaaS és SaaS szinten keletkezett napló állományok kiadását csak hatósági megkeresés alapján biztosítja a központi szolgáltató. Felhasználók számára a hozzáférhetőség nem biztosított.

Megszűnő szolgáltatások esetén a Felhasználó bérleményében tárolt naplóállományok megsemmisítésre kerülnek.

19. Webalkalmazás-tűzfal (WAF)

A KAK Felhő határát képező perimeter eszköz beépítve tartalmazza az elterjedtebb általános web-alapú támadások elleni védelmet.

20. Mentés szolgáltatás

A KAK Felhő által biztosított felhő alapú működési környezetben Ellátási szolgáltatásonként külön-külön módon definiált formában beállítható mentés mind komplett virtuális gép (image szintű mentés), illetve agent alapú mentés formájában. A mentés DDT (disc-to-disc-to-tape: lemezről – lemezre – majd szalagra) formában kerül megvalósításra. A mentéseknek a VTL (Virtual Disk Library – virtuális lemezkötet) – ről a szalagos kötetre kerülésének ütemezését a központi szolgáltató végzi.

21. Archiválás szolgáltatás

Két típusú archiválási funkciót kínál a KAK Felhő:

– egy-egy kiválasztott mentés hosszú távú megőrzését, és

– API-t ahhoz, hogy az alkalmazások megvalósítsák saját archiválási funkciójukat.

A második esetben az alkalmazásnak magának kell gondoskodnia arról, hogy képes legyen az adatok egy körében csak a metaadatokat, illetve kumulált értékeket élő adatbázisban tartani és a valós, ritkán használt adatokat a biztosított API-n keresztül lassabb elérésű tárolóra írni. Amennyiben hivatkozás történik ezekre az adatokra, szintén a biztosított API-n keresztül lehet visszaolvasni. A szolgáltatás csak az archiválás technikai feltételeit biztosítja, az archiválás egyéb funkcióit az alkalmazói rendszernek kell biztosítania.

22. Adatbázis kiszolgáló szolgáltatás (DBaaS)

A DBaaS szintű kiegészítő szolgáltatások esetén általánosan elmondható, hogy a központi szolgáltató által biztosított szintig az üzemeltetést a központi szolgáltató végzi. Ez azt jelenti, hogy a központi szolgáltató rendszeres, előre bejelentett, tervezhető időközönként telepíti a javítócsomagokat (patch) először a fejlesztői, teszt, oktatói környezetekben, majd az éles környezetben is. Központi szolgáltató csak egy stabil verziójú szoftver kiadást üzemeltet a platform szolgáltatásokban.

Mivel az adatbázis szolgáltatás kiegészítő szolgáltatás,

– szükséges egy olyan ellátási szolgáltatás elem megléte, amelyik igénybe veszi majd az adatbázis szolgáltatásait;

– felhőn kívülre nem szolgáltatjuk.

22.1.1.1 Zárt forráskódú Adatbázis kiszolgáló szolgáltatások

a) A nagy tárolási és feldolgozási igényű, online tranzakció-feldolgozó adatbázis alkalmazásokhoz adattároló és – kezelő fürt van kialakítva. A két telephelyen azonos méretű hardvereken, redundáns fürtök adják a fizikai erőforrásokat. A szolgáltatás szintű magas rendelkezésre állást az adatbázis kiszolgálókon futó klaszter, míg a két telephely közötti adattárolási redundanciát a központi szolgáltató IP feletti aszinkronszinkron replikációval biztosítja.

Szolgáltatás keretében a központi szolgáltató biztosít izolációs megoldást. Minden olyan beállítást, ami ez alatt a szint alatt van (például adatbázisok létrehozása) a tenant felhasználójának a saját adminisztrációs eszközét használva kell beállítania a szükséges jogosultságokkal.

b) Nagyvállalati szintű relációs adatbázis kezelő platform szolgáltatás a felhasználói alkalmazások on-line tranzakciós igényeinek (OLTP) kezelését támogatja, ahol a szolgáltatás műszaki kialakítása a nagy adattárolási és feldolgozási igényű alkalmazások kiszolgálását is biztosítja. A platform szolgáltatás futtatásához szükséges számítási erőforrásokat dedikált szerverek, míg az adatok tárolására szolgáló tárterület a szerverekhez SAN (Storage Area Network) hálózaton keresztül csatolt külső, központi tároló egységek biztosítják.

A szolgáltatás keretében megtörténik az elvárt felhasználói izoláció. Minden olyan beállítást, ami ez alatt a szint alatt van (például adatbázisok létrehozása) a tenant felhasználója a saját adminisztrációs eszközét használva fog beállítani, az adott instance-ra vonatkozó DBA Admin joggal.

22.1.1.2 Nyílt forráskódú Adatbázis kiszolgáló szolgáltatások

a) a központi szolgáltató adatbázis-kezelő rendszer szintű szolgáltatásokat nyílt forráskódú szabad szoftver adatbázis platformszolgáltatások által is biztosít.

Az adatbázis szerver platform felhasználói szolgáltatásonként külön virtuális környezetre települ, így a szerver virtualizáció a szeparációt és a magas rendelkezésre állást is fizikai szinten biztosítja. A magas rendelkezésre állás és katasztrófa elhárítás követelményeit a platform szinten elérhető Multi-Master replikáció támogatja magasabb szinten. Minden felhasználói szolgáltatás esetén – az igényekhez illeszkedően – több szinkron és aszinkron példány alkalmazható oldal irányú skálázás biztosítására, illetve a telephelyek közötti aszinkron replikációval a katasztrófa jellegű meghibásodások kezelésére.

b) A nem relációs adatbázis kezelő a webes alkalmazások jelentős mennyiségű párhuzamos feldolgozási igényeinek kiszolgálását, a gyorsító tárak hatékonyabb és az adatstruktúrák rugalmasabb kezelését, valamint azok jobb skálázási lehetőségeit biztosító adatbázis platform szolgáltatás. Az adatbázis belső tárolási struktúrája kulcs-érték párok és dokumentumok tárolására, illetve kezelésére optimalizált.

3. Adatmegőrzési szolgáltatás

Az adatmegőrzési szolgáltatás keretében a nemzeti adatvagyonba tartozó, továbbá jogszabály által kötelezően megőrzésre kijelölt informatikai alkalmazások, adatok és információk elektronikus formában történő tárolását és megőrzését biztosítja a Kormányzati Adatközpont.

Az állam működése szempontjából létfontosságú adatvagyon védelme, ezek hasonló módon való biztonságos tárolása, kezelése kiemelt fontosságú. Ezen adatok vonatkozásában a különböző rendszerekben tervszerű és jogszabályban előírt módon történő mentési és archiválási feladatokat kell végrehajtani. A lementett állományokat el kell juttatni a redundáns adatközpontokba, mely azt fogadja és megfelelő módon biztonságosan tárolja. Katasztrófa helyzet esetében az adatok biztonságos megőrzéséről gondoskodik és ezen adatok felhasználásával újra építhetővé teszi a különböző informatikai rendszereket az előírt protokollok alapján.

A katasztrófatűrő, nagy megbízhatóságú működési szempontok és az adatok biztonságos archiválásának, valamint mentésének megvalósításához a geo-redundancia elvei figyelembevételével elkülönített, megfelelő védettségű redundáns helyszínen kerülnek elhelyezésre. A feladata a hosszú távú archiválási feladatok ellátása. Az itt kialakított kapacitások legfontosabb célja a biztonsági mentési kapacitások és hosszú idejű archiválási kapacitások biztosítása.

Adatmegőrzési szolgáltatáskeretében kezelt adatokkal kapcsolatban a szakrendszerek végponti felhasználói számára közvetlen adatkiszolgálás nincs, ez a terület a külvilágtól (a kormányzati, vagy a közcélú adatátviteli hálózatoktól) hermetikusan el lesz választva.

[^1]: A 15–16. § a 2010: CXXX. törvény 12. § (2) bekezdése alapján hatályát vesztette.
