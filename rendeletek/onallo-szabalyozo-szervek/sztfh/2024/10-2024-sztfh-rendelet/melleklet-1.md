1. melléklet a 10/2024. (VIII. 8.) SZTFH rendelethez

Dokumentációs követelmények

1. IoT-eszköz azonosító dokumentum

1.1. A megfelelőségi önértékelés vagy megfelelőségértékelési vizsgálat alá vont IoT-eszköz (a továbbiakban: VE) azonosítására szolgáló információkat tartalmazó dokumentum, amely a lehető legrészletesebb információkat tartalmazza a vizsgálat tárgyáról, kiemelten a verziószámok és a konfigurációs lehetőségek tekintetében.

1.2. Az azonosító dokumentum minimális tartalmi elemei:

a) Vizsgált termék megnevezése

b) Márka megjelölése

c) Kereskedelmi forgalomban használt név

d) Modellazonosító

e) Hardverkonfiguráció (beleértve a kiadási számot és a sorozatszámot)

f) Futtatókörnyezet vagy operációs rendszer

g) Firmware verzió gyári állapotban

h) Gyártó adatai:

ha) megnevezése

hb) rövid neve

hc) székhelye

hd) telefonszáma

he) e-mail-címe

hf) kapcsolattartó személy adatai: neve, állampolgársága, telefonszáma, e-mail-címe

i) A VE tervezett éves gyártási darabszáma

j) Annak megjelölése, hogy a vizsgált eszköz mely kereskedelmi piacokon kerül értékesítésre várhatóan a következő 1 évben:

ja) csak Magyarország

jb) EU-tagállamok (ha nem a teljes EU területén, akkor a tagállamok felsorolása) vagy

jc) egyéb

k) Annak megjelölése, hogy a vizsgálat milyen megbízhatósági szintnek megfelelően történik: alap/jelentős/magas

2. Megvalósítási dokumentum

2.1. A megvalósítási dokumentum (a továbbiakban: MD) az 1. pont szerint azonosított IoT-eszköz megvalósítása során alkalmazott, a 2. melléklet szerinti követelmények értékelése szempontjából lényeges, részletes információkat tartalmazza.

2.2. Az MD minimális tartalmi elemei

2.2.1. MD 1-UserInfo: Felhasználói információk

## Az MD felsorolja a dokumentációkat, kiadványokat és a felhasználóknak nyújtott információkat. Ide sorolandó mind a gyártó weboldala és a megfelelő URL, a felhasználói kézikönyv vagy a beépített súgó. A lista a következő egymástól független funkciók, mechanizmusok működése kapcsán elérhető információkat tartalmazza:

|  | A | B |

| 1. | A módosítási mechanizmusok dokumentálása | A hitelesítési értékek módosítási mechanizmusainak dokumentálása a felhasználó számára, beleértve a dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 2. | Az érzékelők dokumentációja | A külső érzékelési képességekkel kapcsolatos információknak a felhasználó számára való dokumentálása, beleértve a dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 3. | A biztonságos beállítás dokumentációja | A VE biztonságos beállítása felhasználói dokumentációjának módszere, beleértve dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 4. | A beállítási ellenőrzés dokumentációja | Annak leírása, hogy a felhasználó számára hogyan dokumentálják a VE biztonságos beállításának ellenőrzésére szolgáló módszert, beleértve a dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 5. | A személyes adatok dokumentálása | A személyes adatok feldolgozására vonatkozó információknak a felhasználó számára történő dokumentálási módja, beleértve a dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 6. | A telemetriai adatok dokumentálása | A telemetriai adatok gyűjtésével kapcsolatos információknak a felhasználó számára történő dokumentálási módja, beleértve a dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 7. | A törlés dokumentálása | A személyes adatok törlési módjának a felhasználó számára történő leírása, beleértve a dokumentációhoz való hozzáféréshez szükséges összes információt. |

| 8. | Modell megnevezése | A VE modell megjelölése és annak rövid leírása, hogy a VE modellmegjelölését a felhasználó hogyan ismerheti fel. Itt kell megadni, ha hálózati lekérdezéssel is lekérdezhető a VE és szoftverkomponensei verziószáma, illetve, hogy az milyen módon történik. Itt kell jelölni nyílt forráskódú szoftverek használata esetén a nyílt forráskódú operációs rendszerek rendszermagjainak és alkalmazásainak verzióit, illetve azt, hogy az rendelkezik hosszú távú támogatási (LTS) idővel. |

| 9. | Támogatási időszak | Az az időtartam, amely alatt a terméket vagy szolgáltatást a gyártó karbantartja, pl. frissítések formájában, ideértve a nyílt forráskódú operációs rendszerek rendszermagjainak és alkalmazásainak verzióit. |

| 10. | A támogatási időszak közzététele | A támogatási időszak közzétételének és dokumentálásának módja a felhasználó számára, beleértve a közzétételhez való hozzáférés összes információját. |

| 11. | A sebezhetőség közzététele | A sebezhetőségek közzétételének módja, beleértve a közzétételhez való hozzáférés összes információját. |

| 12. | A nem frissíthető komponensek közzététele | A szoftverfrissítések hiánya indokolásának leírása, beleértve a közzétételhez való hozzáféréshez szükséges összes információt. |

2.2.2. MD 2-SecDev: Biztonságos fejlesztési folyamatok

## Az MD felsorolja az összes biztonságos fejlesztési folyamatot, amelyet a gyártó a VE-re vonatkozóan végrehajtott vagy végrehajtatott. Az MD a következő bejegyzéseket tartalmazza:

|  | A | B |

| 1. | ID | Folyamatonként egyedi azonosító SecDev-1-gyel kezdődően. |

| 2. | Leírás | A biztonságos fejlesztési folyamat rövid leírása. Ha egy meglévő szabványt használnak, akkor a megfelelő szabványra való hivatkozást kell megadni. Ki kell térni az alkalmazott programozási technikák ismertetésére annak igazolására, hogy az alkalmas a manipulációs, hibát, illetve információszivárgást előidéző (tampering, fault and leakage) támadások mérséklésére. |

2.2.3. MD 3-VulnTypes: Releváns sebezhetőségek

## Az MD felsorolja az összes olyan típusú sebezhetőséget, amely a VE szempontjából lényeges. Az MD a következő bejegyzéseket tartalmazza:

|  | A | B |

| 1. | ID | Sebezhetőségenként egyedi azonosító VulnTypes-1-gyel kezdődően. |

| 2. | Leírás | A VE szempontjából releváns sebezhetőség rövid leírása. |

| 3. | Intézkedés | A sebezhetőség feltárása esetén az ilyen típusú sebezhetőséggel kapcsolatos intézkedés módjának leírása, beleértve az intézkedésben részt vevő összes szervezetet és felelősségüket. |

| 4. | Időkeret | Célzott időkeret, amelyben a sebezhetőség esetén a cselekvés adott lépéseit ütemezik. Példa: 5 nap az első válaszadásra és 90 nap a javítás közzétételéig. |

2.2.4. MD 4-Conf: Nyilatkozatok

## Az MD felsorolja a folyamatok létrehozására vonatkozó nyilatkozatokat. Az MD a következő, egymástól független bejegyzéseket tartalmazza, amelyek kapcsán egyértelmű IGEN vagy NEM válaszokat kell jelölni.

|  | A | B |

| 1. | A sebezhetőségi intézkedések megerősítése | Annak megerősítése, hogy az MD 3-VulnTypes-ban leírt minden egyes „Intézkedés” esetében a szükséges infrastruktúra rendelkezésre áll, és az üzemeltetők tájékoztatást kaptak a megcélzott „Időkeret” elérése érdekében. |

| 2. | A sebezhetőségi felügyelet megerősítése | Annak megerősítése, hogy az MD 5-VulnMonban leírt minden egyes sebezhetőség figyelemmel kíséréséhez, azonosításához és kijavításához a szükséges infrastruktúra rendelkezésre áll, és az üzemeltetők tájékoztatást kaptak. |

| 3. | A frissítési eljárások megerősítése | Annak megerősítése, hogy az MD 6-UpdProc-ban leírt minden egyes frissítési eljáráshoz a szükséges infrastruktúra rendelkezésre áll, és az üzemeltetők tájékoztatást kaptak a célzott „Időkeret” elérése érdekében. |

| 4. | A biztonságos irányítás megerősítése | Annak megerősítése, hogy az MD 15-SecMgmt dokumentumban leírt biztonságos irányítási folyamatokat létrehozták. |

| 5. | A biztonságos fejlesztés megerősítése | Annak megerősítése, hogy az MD 2-SecDevben leírt biztonságos fejlesztési folyamatokat létrehozták. |

2.2.5. MD 5-VulnMon: Sebezhetőség monitorozás

## Az MD felsorolja a sebezhetőségek ellenőrzésére, azonosítására és kijavítására szolgáló összes eljárást, a következő bejegyzéseket tartalmazza.

|  | A | B |

| 1. | ID | Eljárásonként egyedi azonosító VulnMon-1-gyel kezdődően. |

| 2. | Leírás | A termékek és szolgáltatások biztonsági rései nyomon követésének, azonosításának és kijavításának leírása. |

2.2.6. MD 6-UpdProc: Frissítési eljárások

## Az MD felsorolja a gyártó eljárásait a biztonsági frissítések kiadására vonatkozóan a következő adatokkal:

|  | A | B |

| 1. | ID | Eljárásonként egyedi azonosító UpdProc-1-gyel kezdődően. |

| 2. | Leírás | A biztonsági frissítések kiadására vonatkozó eljárás rövid leírása, beleértve az összes szervezetet és felelősséget. |

| 3. | Időkeret | Az eljárás befejezésének tervezett időkerete. |

2.2.7. MD 7-Intf: Interfészek

## Az MD a VE összes hálózati, fizikai és logikai interfészét felsorolja a következő paraméterekkel:

|  | A | B |

| 1. | ID | Interfészenként egyedi azonosító Intf-1-gyel kezdődően. |

| 2. | Leírás | Az interfész leírása, beleértve annak célját is. Fizikai interfészek esetében azt is le kell írni, hogy az interfészre mindig szükség van-e, vagy csak bizonyos, a leírásban kifejtett esetekben (pl. időszakos használat), illetve azt is, ha arra soha nincs szükség. |

| 3. | Típus | Annak jelzése, hogy az interfész hálózati, fizikai (beleértve a vezeték nélküli interfészeket is), logikai vagy többféle típusú. |

| 4. | Állapot | Annak jelzése, hogy az interfész engedélyezve vagy letiltva van az inicializált állapotban. Engedélyezett interfészek esetén indokolás szükséges. |

| 5. | Állapotváltozás | Az interfész állapotainak listája, azzal, hogy az állapotváltozásokat milyen módon és milyen szerepkörű felhasználó – hivatkozva az MD 9-Role szerinti szerepkörre – idézheti elő. |

| 6. | Kapcsolat felépítése | Annak a leírása, hogy az interfész a kapcsolatot milyen módon építi fel, milyen validálási és hitelesítési mechanizmusokat használ, utóbbi esetén hivatkozva az MD-10-Auth szerinti hitelesítési mechanizmusra. |

| 7. | Közzétett információk | Ha az interfész hálózati interfész: az inicializált állapotban hitelesítés nélkül nyilvánosságra hozott információk leírása és a nyilvánosságra hozatal oka, továbbá annak feltüntetése, hogy a nyilvánosságra hozatal információbiztonsági szempontból releváns-e. |

| 8. | Hibakeresési interfész | Ha az interfész fizikai interfész: az interfész használható-e hibakeresési interfészként. |

| 9. | Védelem | Ha az interfész fizikai interfész: az interfész kitettségének korlátozásához szükséges védelmi módszerek leírása. A hibakeresési interfészek esetében elvárás az interfész letiltására használt szoftvermechanizmus leírása. |

2.2.8. MD 8-DevID: Eszközazonosítók

## Az MD-ben szerepeltetni kell a VE összes, az eszköz azonosítására szolgáló azonosítóját.

|  | A | B |

| 1. | ID | Eszközazonosítónként egyedi azonosító DevID-1-gyel kezdődően. |

| 2. | Azonosító típusa | Az azonosító formájára (címke, fizikai vagy logikai azonosító) és annak egyediségére vonatkozó információk. |

| 3. | Azonosító hozzáférhetősége | Az azonosító az eszköz egyes állapotaiban (gyári csomagolt, gyári alapértelmezett és beüzemelt) milyen úton, milyen szerepkörrel rendelkező felhasználó által és milyen módon ismerhető meg. Ha az azonosító interfészen keresztül elérhető, hivatkozni szükséges az MD 7-Intf szerinti interfészre. |

| 4. | Azonosító forrása | „Előre telepített” vagy „Felhasználó által hozzáadható”. |

| 5. | Azonosítógeneráló mechanizmus | Az azonosító generálására használt algoritmus rövid leírása, ismertetve azokat az intézkedéseket, amelyek kockázatarányosan biztosítják, hogy az azonosítók csökkentik a nyilvánvaló szabályszerűségeken, közös karakterláncokon, nyilvánosan elérhető információkon vagy nem megfelelő összetettségen alapuló automatikus támadások kockázatát. |

| 6. | Műveletvégzés | Az azonosító ismeretében végrehajtható műveletek leírása és azok végrehajtásának módja, hivatkozással a műveletvégzésben érintett, az MD 7-Intf szerinti interfészekre. |

| 7. | Biztonsági célok | A megvalósított biztonsági célok és a mechanizmus által elhárítandó fenyegetések leírása. |

| 8. | Brute Force védelem | Ha az azonosító közvetlenül egy hálózati interfészről elérhető, az annak megakadályozására kialakított módszer leírása, hogy a támadó a hálózati interfészeken keresztül brute force támadással megszerezze az azonosító adatokat. |

| 9. | Timing attack elleni védelem | Ha az azonosító közvetlenül egy hálózati interfészről elérhető, az annak megakadályozására kialakított módszer leírása, hogy a támadó időzítések kihasználásával szerezzen jogosulatlan felhatalmazást. |

2.2.9. MD 9-Role: Szerepkörök

## Az MD-ben szerepeltetni kell a VE által gyári állapotban kezelt szerepköröket, ideértve a nem azonosításkötelezett szereplőket és gép-gép közötti kapcsolatokat is.

|  | A | B |

| 1. | ID | Szerepkörönként egyedi azonosító Role-1-gyel kezdődően. |

| 2. | Leírás | A szerepkör rövid leírása. |

| 3. | Cél | A szerepkörbe tartozó felhasználók általános célja. |

| 4. | Műveletek | A szerepkörbe tartozó felhasználók által elvégezhető műveletek listája. |

2.2.10. MD 10-AuthMech: Hitelesítési mechanizmusok

## Az MD-ben szerepeltetni kell a VE összes hitelesítési mechanizmusát. Az MD a következő bejegyzéseket tartalmazza:

|  | A | B |

| 1. | ID | Hitelesítési mechanizmusonként egyedi azonosító AuthMech-1-gyel kezdődően. |

| 2. | Leírás | A hitelesítési mechanizmus és a hozzá tartozó engedélyezési folyamat rövid leírása. Meg kell adni, hogy a mechanizmust a felhasználó vagy a gép-gép közötti hitelesítésre használják-e, és hogy az közvetlenül egy hálózati interfészről érhető-e el. Harmadik feles megvalósítás esetén ismertetni kell, hogy az ellátási lánc tervezése miképpen akadályozza meg a VE-specifikus hitelesítő adatok kiszivárgását. |

| 3. | Authentikációs faktor | A hitelesítéshez használt attribútum típusa. Jelszavak esetében azt is jelezni kell, hogy a jelszót a felhasználó állítja-e be, és használja-e az inicializált állapotban. |

| 4. | Jelszógeneráló mechanizmus | Ha a hitelesítési tényező egy jelszó, amelyet nem a felhasználó állít be, a jelszó generálására szolgáló mechanizmus leírása, azzal, hogy részletes leírás nem szükséges. A leírásban meg kell adni, hogy a jelszó eszközönként egyedi-e, és hogy előre telepített-e, ismertetni kell azokat az intézkedéseket, amelyek biztosítják, hogy a jelszavak a gyári alapértelmezettől eltérő bármely állapotban eszközönként egyediek legyenek, és csökkentik a nyilvánvaló szabályszerűségeken, közös karakterláncokon, nyilvánosan elérhető információkon vagy nem megfelelő összetettségen alapuló automatikus támadások kockázatát, ha előre telepített és eszközönként egyedi jelszóként használják. |

| 5. | Biztonsági garanciák | A megvalósított biztonsági célok és a mechanizmus által elhárítandó fenyegetések leírása. |

| 6. | Kriptográfiai részletek | A kulcskezelés figyelembevételével a hitelesítési mechanizmus biztosítására és a leírt „biztonsági garanciák” megkönnyítésére használt kriptográfiai módszerek (protokollok, műveletek, primitívek, módok és kulcsméretek) leírása. |

| 7. | Brute Force védelem | Ha a hitelesítési mechanizmus közvetlenül egy hálózati interfészről elérhető, annak megakadályozására kialakított módszer leírása, hogy a támadó a hálózati interfészeken keresztül brute force támadással megszerezze a hitelesítő adatokat. |

| 8. | Timing attack elleni védelem | Ha a hitelesítési mechanizmus közvetlenül egy hálózati interfészről elérhető, az annak megakadályozására kialakított módszer leírása, hogy a támadó időzítések kihasználásával szerezzen jogosulatlan felhatalmazást. |

| 9. | Testreszabás | A hitelesítési mechanizmushoz kapcsolódó beállítási lehetőségek. |

| 10. | Alkalmazás | A hitelesítési mechanizmust használó interfészek és felhasználók szerepköre, hivatkozással az MD 7-Intf szerinti interfészekre és MD 9-Role szerepkörökre. |

| 11. | Kezelés | A hitelesítő azonosító megváltoztatása folyamatának leírása. |

2.2.11. MD 11-Account: Fiókkezelés

## Az MD-ben szerepeltetni kell a felhasználói fiókok kezeléséhez kapcsolódó megoldásokat.

|  | A | B |

| 1. | ID | Műveletenként és megoldásonként egyedi azonosító Account-1-gyel kezdődően. |

| 2. | Művelet | Művelet megnevezése. |

| 3. | Leírás | A megvalósított művelet mechanizmusának részletes leírása. |

| 4. | Konfiguráció | Annak leírása, hogy a fiókkezelési műveletben milyen adatok konfigurálhatóak és milyen MD 9-Role szerinti szerepkörrel rendelkező felhasználók számára. |

2.2.12. MD 12-SoftComp: Szoftverkomponensek

## Az MD a VE összes szoftverkomponensét felsorolja. Az alkalmazott részletezettségi szint a vizsgált szoftver szoftverkomponensekre való felosztására vonatkozóan azt a célt szolgálja, hogy esetleges sérülékenységvizsgálat esetén azonosítani lehessen, hogy mely komponensek frissíthetőek, és melyek nem. Az MD a következő bejegyzéseket tartalmazza:

|  | A | B |

| 1. | ID | Szoftverkomponensenként egyedi azonosító SoftComp-1-gyel kezdődően. |

| 2. | Leírás | A szoftverkomponens rövid leírása. Külön jelezni kell, ha a szoftverkomponens frissítése érzékeny adatot tartalmaz. |

| 3. | Frissítési mechanizmus | Hivatkozás az MD 13-UpdMech frissítési mechanizmusaira, amelyeket a szoftverkomponens frissítésére használnak. A frissítési mechanizmusok üres listája a szoftverkomponens frissítésének hiányát jelzi, amelynek elmaradását indokolni szükséges. |

| 4. | Kriptográfiai felhasználás | Jelzi, hogy a szoftverkomponens használ-e kriptográfiai algoritmusokat vagy primitíveket (igen/nem), és ha igen, akkor azt is tartalmazza, hogy a gyártó figyelembe vette-e ezen algoritmusok és a primitívek frissítésének mellékhatásait (igen/nem). |

2.2.13. MD 13-UpdMech: Frissítési mechanizmusok

## Az MD felsorolja a VE összes frissítési mechanizmusát, amelyek kapcsán a következő bejegyzéseket tartalmazza:

|  | A | B |

| 1. | ID | Frissítési mechanizmusonként egyedi azonosító UpdMech-1-gyel kezdődően. |

| 2. | Leírás | A frissítési mechanizmus rövid leírása, beleértve annak főbb jellemzőit. Ezenkívül meg kell adni, hogy a frissítés kézbesítése hálózati alapú-e. |

| 3. | Biztonsági garanciák | A megvalósított biztonsági célkitűzések és a mechanizmus által elhárítandó fenyegetések leírása. A hitelesség és az integritás érdekében ezenfelül azt is fel kell tüntetni, hogy a biztonsági garanciát maga a VE adja-e. |

| 4. | Kriptográfiai részletek | A kulcskezelést figyelembe vevő frissítési mechanizmus biztonságának biztosítására és a leírt „Biztonsági garanciák” megkönnyítésére használt kriptográfiai módszerek (protokollok, műveletek, primitívek, módok és kulcsméretek) leírása. Az ellenőrzésre használt nyilvános kulcsok telepítésének módja. |

| 5. | Kezdeményezés és interakció | A frissítéskezdeményezés módjának, valamint a frissítés kezdeményezéséhez és alkalmazásához szükséges felhasználói interakció rövid leírása, jelezve, hogy automatikus frissítési mechanizmusról van-e szó. |

| 6. | Konfiguráció | Rövid leírás arról, hogy a felhasználó hogyan konfigurálhatja a szoftverfrissítések automatizálását és értesítését, és milyen lehetőségek (pl. engedélyezés, letiltás, elhalasztás) közül választhat. Az alapértelmezett konfigurációt is itt kell megadni. |

| 7. | Frissítés ellenőrzése | A biztonsági frissítések elérhetősége lekérdezési mechanizmusának és ütemezésének rövid leírása, továbbá annak rögzítése, hogy a biztonsági frissítés elérhetőségének ellenőrzését maga a VE végzi-e. |

| 8. | Felhasználói értesítés | Rövid leírás arról, hogy a felhasználót hogyan tájékoztatják az elérhető frissítésről és a frissítési mechanizmus által okozott zavarokról, pl. bizonyos funkciók korlátozott elérhetőségéről, megjelölve, hogy az értesítés milyen információkat tartalmaz, és hogy az értesítést maga a VE valósítja-e meg. |

| 9. | Verziókezelés | Rövid leírás arról, hogy a VE miként ellenőrzi és érvényesíti a frissítés verzióját a telepítés előtt. |

2.2.14. MD 14-SecParam: Biztonsági paraméterek

## Az MD felsorolja az összes olyan érzékeny (nyilvános és kritikus) biztonsági paramétert, amelyet a rendeltetésszerű használat során tartósan tárolnak a VE-n, az alábbi paraméterekkel:

|  | A | B |

| 1. | ID | Paraméterenként egyedi azonosító SecParam-1-gyel kezdődően. |

| 2. | Leírás | A biztonsági paraméter rövid leírása, beleértve annak célját is, megjelölve, hogy az adott biztonsági paraméter az eszközben biztonsági célokra használt, hard kódolt egyedi eszközönkénti azonosító, illetve az eszköz szoftverének forráskódjában hard kódolt. |

| 3. | Tárolás helye | A biztonsági paraméter tárolásának helye és módja. |

| 4. | Típus | Annak rögzítése, hogy a biztonsági paraméter nyilvános vagy kritikus. |

| 5. | Biztonsági garanciák | A megvalósított alapvető biztonsági célkitűzések és a fenyegetések leírása, amelyekkel szemben a biztonsági paraméter a tartós tárolás során védelmet élvez. |

| 6. | Védelmi rendszer | A biztonsági garanciák elérése érdekében alkalmazott intézkedések leírása, ideértve azokat a felhatalmazásokat és szerepköröket, amelyeken keresztül a paraméterhez való hozzáférés lehetséges, továbbá az egyes szerepkörökhöz kapcsolódó jogosultságokat. |

| 7. | Elosztási mechanizmus | Ha a „Típus” azt jelzi, hogy a paraméter kritikus: annak a mechanizmusnak a leírása, amelyen keresztül a paraméter értéket kap. |

| 8. | Kommunikációs mechanizmusok | Hivatkozás az MD 16-ComMech-ben a paraméterek közlésére használt kommunikációs mechanizmusokra és annak feltüntetése, hogy a kommunikáció távolról elérhető interfészeken keresztül történik-e. |

| 9. | Létrehozási mechanizmus | Ha a „Típus” azt jelzi, hogy a paraméter kritikus, vagy a szoftverfrissítések integritásának és hitelességének ellenőrzésére vagy a kapcsolódó szolgáltatásokkal való kommunikáció védelmére használják: a paraméter értékeinek létrehozására használt mechanizmus leírása és ezenfelül annak feltüntetése, hogy a paramétert a szoftverfrissítések integritásának és hitelességének ellenőrzésére vagy a kapcsolódó szolgáltatásokkal való kommunikáció védelmére használják. |

2.2.15. MD 15-SecMgmt: Biztonságos irányítási folyamatok

## Az MD felsorolja a kritikus biztonsági paraméterekre vonatkozó összes biztonságos kezelési folyamatot, amelyet a gyártó megvalósított a VE életciklusa során.

|  | A | B |

| 1. | ID | Folyamatonként egyedi azonosító SecMgmt-1-gyel kezdődően. |

| 2. | Leírás | A biztonságos kezelési folyamat rövid leírása a kritikus biztonsági paraméterek teljes életciklusára vonatkozóan egy meglévő szabvány használata esetén a megfelelő szabványra való hivatkozás megadásával. A kritikus biztonsági paraméterek életciklusa jellemzően a generálást, a rendelkezésre bocsátást, a tárolást, a frissítéseket, a kivonást, az archiválást, a megsemmisítést, a lejáratot kezelő folyamatokat és a paraméter veszélyeztetettségét veszi figyelembe. A generálás során a felhasznált véletlenszámok előállításának, annak entrópiájának mérési módját is ismertetni kell. Ha fájl-integritásellenőrzést alkalmaz az eszköz, annak módját is ismertetni kell. |

2.2.16. MD 16-ComMech: Kommunikációs mechanizmusok

## Az MD felsorolja a VE összes kommunikációs mechanizmusát a következő részletes információkkal:

|  | A | B |

| 1. | ID | Mechanizmusonként egyedi azonosító ComMech-1-gyel kezdődően. |

| 2. | Leírás | A kommunikációs mechanizmus rövid leírása, beleértve a célját és a használt protokoll leírását. Szabványosított protokollok esetén elegendő egy hivatkozás verziószámmal. Ezenkívül fel kell tüntetni, hogy a mechanizmus távolról elérhető-e. |

| 3. | Biztonsági garanciák | A megvalósított biztonsági célkitűzések és a mechanizmus által elhárítandó fenyegetések leírása. |

| 4. | Kriptográfiai részletek | A kommunikációs mechanizmus biztosításához használt kriptográfiai módszerek (protokollok, műveletek, primitívek, módok és kulcsméretek) leírása a kulcskezelés figyelembevételével, a leírt „Biztonsági garanciák” céljainak elérése érdekében. |

| 5. | Ellenállási intézkedések | Az intézkedések leírása, amelyek biztosítják, hogy a kapcsolat létrehozása rendezett módon történik, beleértve a stabil kapcsolat elérését eredményező, elvárt, működőképes és stabil állapotot. |

2.2.17. MD 17-NetSecImpl: Hálózati és biztonsági megvalósítások

## Az MD felsorolja a VE hálózati és biztonsági funkcióinak összes megvalósítását.

|  | A | B |

| 1. | ID | Elemenként egyedi azonosító NetSecImpl-1-gyel kezdődően. |

| 2. | Leírás | A hálózati vagy biztonsági funkció megvalósításának rövid leírása, beleértve a célját és a hatókörét. |

| 3. | Felülvizsgálati/értékelési módszer | A végrehajtás felülvizsgálatára vagy értékelésére alkalmazott módszer leírása, beleértve az alapelveket is (pl. audit, szakértői értékelés, automatikus kódelemzés), és a módszer által lefedett megvalósítás hatókörének ismertetése. |

| 4. | Jelentés | A felülvizsgálat vagy értékelés eredménye vagy hivatkozás a tanúsítványra vagy az értékelő jelentésre, amely bizonyítja, hogy a végrehajtást sikeresnek értékelték. |

2.2.18. MD 18-SoftServ: Szoftverszolgáltatások

## Az MD felsorolja a VE összes szoftverszolgáltatását a következők szerint:

|  | A | B |

| 1. | ID | Szolgáltatásonként egyedi azonosító SoftServ-1-gyel kezdődően. |

| 2. | Leírás | A szolgáltatás rövid leírása, beleértve annak célját, feltüntetve, hogy a szolgáltatás elérhető-e és mely MD 7-Intf szerinti hálózati interfészen keresztül, és azt, hogy ez az inicializált állapotban is így van-e. |

| 3. | Állapot | Annak jelzése, hogy a szolgáltatás engedélyezett vagy letiltott az inicializált állapotban. |

| 4. | Indokolás | Ha a szolgáltatás engedélyezett, annak indokolása, hogy a szolgáltatás miért szükséges a VE rendeltetésszerű használatához vagy működéséhez. |

| 5. | Konfiguráció | Ha a szolgáltatás hálózati interfészen keresztül elérhető: tájékoztatás arról, hogy a szolgáltatás lehetővé teszi-e a konfiguráció biztonsági szempontból fontos módosítását, és ha igen, a lehetséges konfiguráció rövid leírása. Harmadik feles szoftverkomponens esetén nyilatkozat a szolgáltatás alapértelmezés szerinti tiltásáról. |

| 6. | Hitelesítési mechanizmus | Ha a szolgáltatás hálózati interfészen keresztül elérhető: hivatkozás az MD 10-AuthMech-ben a hitelesítési mechanizmusokra, amelyeket a szolgáltatás használata előtti hitelesítésre használnak. |

| 7. | Harmadik feles SW | Annak jelölése, hogy a szoftverkomponens harmadik féltől származik-e. Ha igen, akkor az elkülönítésre vonatkozó eljárás leírása. |

2.2.19. MD 19-CodeMin: Kódminimalizálás

## Az MD felsorolja a kódok minimalizálására alkalmazott módszereket.

|  | A | B |

| 1. | ID | Módszerenként egyedi azonosító CodeMin-1-gyel kezdődően. |

| 2. | Leírás | A kódnak a szükséges funkcionalitásra való minimalizálására használt módszer rövid leírása. |

2.2.20. MD 20-PrivlCtrl: Jogosultságszabályozás

## Az MD felsorolja az összes jogosultságszabályozási mechanizmust a következők szerint:

|  | A | B |

| 1. | ID | Mechanizmusonként egyedi azonosító PrivlCtrl-1-gyel kezdődően. |

| 2. | Leírás | A VE-n lévő szerepkörök és szoftverek jogosultságainak ellenőrzésére szolgáló mechanizmus rövid leírása. |

| 3. | Mátrix | Az adott jogosultság-ellenőrző mechanizmus által kezelt jogosultsági mátrix. |

| 4. | Hitelesítés | Az adott jogosultság-ellenőrző mechanizmus által elvárt hitelesítési mechanizmusra való hivatkozás. |

2.2.21. MD 21-AccCtrl: Hozzáférés-védelem

## Az MD felsorolja a memóriához való hozzáférés-védelmi mechanizmusokat hardveres szinten a következők szerint:

|  | A | B |

| 1. | ID | Mechanizmusonként egyedi azonosító AccCtrl-1-gyel kezdődően. |

| 2. | Leírás | A hardverszintű hozzáférés-szabályozási mechanizmus rövid leírása, amely tartalmazza azt is, hogy a VE operációs rendszere hogyan támogatja azt. |

2.2.22. MD 22-SecBoot: Biztonságos rendszerindítási mechanizmusok

## Az MD felsorolja a VE összes biztonságos indítási mechanizmusát a következők szerint:

|  | A | B |

| 1. | ID | Mechanizmusonként egyedi azonosító SecBoot-1-gyel kezdődően. |

| 2. | Leírás | A VE biztonságos indítási folyamatához használt mechanizmus rövid leírása (beleértve a biztonsággal kapcsolatos feltételezéseket) és a szoftver védett részének azonosítása. Külön ki kell térni mindazon vezérlési lehetőségekre, API-hívásokra, amelyek a mechanizmus működését befolyásolják. Ha a VE alkalmaz biztonsági másolatot a védett szoftverről, annak használati módja is a leírás része. |

| 3. | Biztonsági garanciák | A mechanizmus megvalósított biztonsági célkitűzéseinek leírása. A mechanizmusok az operációs rendszerek rendszermagjának hitelességét és integritását valósítják meg. |

| 4. | Érzékelési mechanizmusok | A VE szoftverének jogosulatlan módosítását észlelő mechanizmus leírása. |

| 5. | Felhasználói értesítés | Rövid leírás arról, hogy hogyan értesül a felhasználó a szoftver jogosulatlan módosításáról, kiegészítésként feltüntetve, hogy az értesítés milyen információkat tartalmaz. |

| 6. | Értesítési funkciók | A felhasználó értesítéséhez szükséges hálózati funkciók rövid leírása. |

2.2.23. MD 23-Store: Tárolás és visszaállítás

## Az MD felsorolja, hogy a VE által kezelt adatok milyen módon kerülnek tárolásra, illetve az adatok visszaállíthatóságának módját a következők szerint:

|  | A | B |

| 1. | ID | Tárolási módonként egyedi azonosító Store-1-gyel kezdődően. |

| 2. | Tároló | A VE által kezelt adatok tárolásának módja és helye. |

| 3. | Redundancia | A tárolási mechanizmusban bekövetkező hiba esetén annak pótmechanizmusa. |

| 4. | Az adatok visszaállításának módja | Az elsődleges tároló vagy a VE meghibásodása esetén a korábbi adatok visszaállításának módja. |

| 5. | Titkosítás | A tárolón alkalmazott titkosítási algoritmus, feltüntetve, hogy gyári alapértelmezett állapotban a titkosítás engedélyezett-e, továbbá hogy a titkosított tárolás milyen módon és milyen szerepkörrel rendelkező felhasználó által állítható be. |

2.2.24. MD 24-DataSec: Adatvédelem

## Az MD felsorolja a VE által feldolgozott összes adatot – a telemetriaadatok kivételével – a következők szerint:

|  | A | B |

| 1. | ID | Adatonként egyedi azonosító DataSec-1-gyel kezdődően. |

| 2. | Leírás | A VE által feldolgozott adatok kategóriájának rövid leírása. Személyes adat bármely azonosított vagy azonosítható, természetes személyre vonatkozó információ. |

| 3. | Feldolgozási tevékenységek | Az adatok feldolgozásának leírása, ismertetve az összes érintett felet, továbbá annak leírása, hogy milyen célból történik az adatfeldolgozás. |

| 4. | Kommunikációs mechanizmusok | Hivatkozás az adatok közlésére használt MD 16-ComMech kommunikációs mechanizmusokra, valamint annak feltüntetése, hogy a kommunikációs partner társított szolgáltatás-e (igen/nem). A kommunikációs mechanizmusok üres listája azt jelzi, hogy az adatokat nem továbbítják. |

| 5. | Érzékenység | Annak jelzése, hogy az adatok érzékeny adatok-e. Érzékeny adat az az adat, amelynek nyilvánosságra hozatala nagy valószínűséggel kárt okozhat az érintettnek. Az, hogy mi minősül érzékeny adatnak, termékenként és felhasználási esetenként eltérő lehet, de példaként említhetőek a fizetési információk, kommunikációs adatok tartalma és az időbélyegzővel ellátott helymeghatározási adatok. |

| 6. | Hozzájárulás megszerzése | Ha a személyes adatok feldolgozása az érintett hozzájárulása alapján történik: annak leírása, hogy a hozzájárulás megszerzése hogyan történik. |

| 7. | A hozzájárulás visszavonása | Ha a személyes adatok feldolgozása az érintett hozzájárulása alapján történik: leírás arról, hogy az érintett hogyan vonhatja vissza a személyes adatok feldolgozásához adott hozzájárulását. |

| 8. | Kriptográfiai védelem | A személyes adatok védelme érdekében alkalmazott kriptográfiai algoritmus MD 12-SoftComp hivatkozással. |

| 9. | Tároló | Az adatokat tároló MD 23-Store szerinti tároló(k). |

2.2.25. MD 25-ExtSens: Külső érzékelők

## Az MD felsorolja a VE összes külső érzékelési képességét a következők szerint:

|  | A | B |

| 1. | ID | Érzékelőnként egyedi azonosító ExtSens-1-gyel kezdődően. |

| 2. | Leírás | Az érzékelési képesség rövid leírása. |

2.2.26. MD 26-ResMech: Ellenálló képességi mechanizmusok

## Az MD felsorolja az összes ellenálló képességi mechanizmust a VE hálózati kapcsolatának megszakadására vagy áramkimaradás esetére a következők szerint:

|  | A | B |

| 1. | ID | Mechanizmusonként egyedi azonosító ResMech-1-gyel kezdődően. |

| 2. | Leírás | Annak az ellenálló képességi mechanizmusnak a leírása, amely hozzájárul a VE ellenálló képességéhez a hálózati, illetve áramkimaradásokkal szemben. |

| 3. | Típus | Az ellenálló képességi mechanizmus a hálózati kapcsolat megszakadására, az áramkimaradás esetére vagy mindkettő kezelésére szolgál. |

| 4. | Biztonsági garanciák | A megvalósított biztonsági célok és a mechanizmus által elhárítandó fenyegetések leírása. |

2.2.27. MD 27-TelData: Telemetriai adatok

## Az MD a VE által gyűjtött összes telemetriai adatot felsorolja a következők szerint:

|  | A | B |

| 1. | ID | Adatonként egyedi azonosító TelData-1-gyel kezdődően. |

| 2. | Leírás | A VE által gyűjtött és a gyártónak szolgáltatott telemetriai adatok rövid leírása. |

| 3. | Cél | Rövid leírás arról, hogy milyen célból gyűjtik az adatokat. |

| 4. | Biztonsági vizsgálat | Ha az adatokat biztonsági vizsgálatra használják, annak leírása, hogy a telemetriai adatokat hogyan és ki (eszköz vagy kapcsolódó szolgáltatás) vizsgálja biztonsági rendellenességek szempontjából. |

| 5. | Adatkapcsolatok | A telemetriai adatokban feldolgozott adatokra való hivatkozás az MD 24-DataSecben. |

2.2.28. MD 28-DelFunc: Törlési funkciók

## Az MD felsorolja a felhasználó adatainak összes törlési funkcióját a következők szerint:

|  | A | B |

| 1. | ID | Törlési funkciónként egyedi azonosító DelFunc-1-gyel kezdődően. |

| 2. | Leírás | A felhasználó adatainak törlésére használt funkció rövid leírása. Ha a „Céltípus” azt jelzi, hogy egy kapcsolódó szolgáltatásnak van címezve, a funkció által lefedett kapcsolódó szolgáltatást is fel kell tüntetni. |

| 3. | Céltípus | Annak megjelölése, hogy a funkció az eszközön lévő felhasználói adatokra vagy a kapcsolódó szolgáltatásokban kezelt személyes adatokra vagy mindkettőre vonatkozik. |

| 4. | Kezdeményezés és interakció | A törlési funkció elindításához és alkalmazásához szükséges felhasználói interakció rövid leírása. |

| 5. | Megerősítés | Rövid leírás arról, hogy a felhasználó a törlési funkció alkalmazása után hogyan kap jelzést arról, hogy az érintett adatok törlésre kerültek. |

2.2.29. MD 29-UserDec: Felhasználói döntések

## Az MD felsorolja a telepítés és karbantartás során meghozandó összes döntést a következők szerint:

|  | A | B |

| 1. | ID | Döntésenként egyedi azonosító UserDec-1-gyel kezdődően. |

| 2. | Leírás | A felhasználó által a telepítési és karbantartási folyamatokon belül meghozandó döntések leírása, rögzítve a felhasználó telepítési vagy karbantartási folyamaton belüli szerepkörét is. |

| 3. | Lehetőségek | A felhasználó által választható, biztonság szempontjából fontos opciók leírása és az alapértelmezett érték megjelölése. |

| 4. | Döntés | Rövid leírás arról, hogy a döntéshozatal hogyan történik, rögzítve, hogy a döntést a végfelhasználó is megteheti-e. |

2.2.30. MD 30-UserIntf: Felhasználói interfészek

## Az MD felsorolja a VE összes olyan felhasználói felületét, amely lehetővé teszi a felhasználó általi bevitelt a következők szerint:

|  | A | B |

| 1. | ID | Felületenként egyedi azonosító UserIntf-1-gyel kezdődően. |

| 2. | Leírás | A felhasználó által történő adatbevitelt lehetővé tevő felhasználói felület céljának, funkciójának, beviteli mezőinek leírása, ismertetve azt is, hogy a felhasználó hogyan férhet hozzá a felülethez. |

| 3. | Konfigurációs interfész | Annak rögzítése, hogy az interfész a VE konfigurációjára használható-e. |

| 4. | Kommunikációs mechanizmus | Ha az interfész a VE konfigurációjára használható, akkor hivatkozás a kommunikációs mechanizmusokra az MD 16-ComMech-ben, amelyet az interfész védelmére használnak. |

2.2.31. MD 31-ExtAPI: Külső API-k

## Az MD felsorolja a VE összes API-ját, amely lehetővé teszi a külső forrásokból történő adatbevitelt a következők szerint:

|  | A | B |

| 1. | ID | API-nként egyedi azonosító ExtAPI-1-gyel kezdődően. |

| 2. | Leírás | A VE külső forrásból történő adatbevitelt lehetővé tevő API leírása. A külső API-kat jellemzően a gép-gép közötti kommunikációra használják. |

2.2.32. MD 32-InpVal: Adatbeviteli érvényesítés

## Az MD felsorolja a VE összes adatbeviteli érvényesítési módszerét a következők szerint:

|  | A | B |

| 1. | ID | Módszerenként egyedi azonosító InpVal-1-gyel kezdődően. |

| 2. | Leírás | A felhasználói felületeken keresztül bevitt vagy API-kon keresztül, illetve a hálózatok között a szolgáltatásokban és eszközökben továbbított adatok érvényesítésére szolgáló módszer leírása, beleértve a váratlan adatok kezelését. Meg kell adni azt is, hogy a módszer az adatbevitel forrásai közül melyeket célozza meg. Az adatbevitel érvényesítéséhez ellenőrizni lehet, hogy az adat megengedett típusú (formátum és szerkezet), megengedett értékű, megengedett számosságú vagy megengedett sorrendű. |

2.2.33. MD 33-Notif: Értesítések

## Az MD-ben szerepeltetni kell a felhasználói értesítések összes módját a következők szerint:

|  | A | B |

| 1. | ID | Értesítési módonként egyedi azonosító Notif-1-gyel kezdődően. |

| 2. | Értesítés módja | Annak leírása, hogy az értesítés mely, az MD 7-Intf szerinti interfészen jelenik meg és mely felhasználók számára. |

| 3. | Értesítés kezelése | A felhasználó által elvégzendő műveletek az értesítés kapcsán. |

| 4. | Tartalom | Az értesítések tartalmi elemei, ha konfigurálhatóak, akkor annak leírása, hogy milyen MD 9-Role szerinti szerepkörrel rendelkező felhasználó és milyen mélységben konfigurálhatja az adattartalmat. |

2.2.34. MD 34-AuditLog: Naplóadatok

## Az MD felsorolja a VE összes naplózási módszerét a következők szerint:

|  | A | B |

| 1. | ID | Naplóelemenként egyedi azonosító AuditLog-1-gyel kezdődően. |

| 2. | Leírás | A naplózási tevékenység hatóköre, a naplók tartalma. |

| 3. | Biztonsági garanciák | A megvalósított alapvető biztonsági célkitűzések és a fenyegetések leírása, amelyekkel szemben a naplóadatok a tartós tárolás során védelmet élveznek. |

| 4. | Védelmi rendszer | A biztonsági garanciák elérése érdekében alkalmazott intézkedések leírása, ismertetve azokat a felhatalmazásokat és szerepköröket, amelyeken keresztül a paraméterhez való hozzáférés lehetséges, beleértve az egyes szerepekhez kapcsolódó jogosultságokat. |

3. Értékelést megalapozó dokumentum

3.1. A gyártó a tesztelendő VE vizsgált megbízhatósági szintje szempontjából a 2. melléklet szerint meghatározott követelményeknek való megfelelést megalapozó, értékelést megalapozó dokumentumot (a továbbiakban: ÉMD) állít ki.

3.2. A dokumentum tartalmazza a cél megbízhatósági szintre vonatkozó, 2. melléklet szerinti követelmények listáját, továbbá a következő adatokat:

a) gyártói besorolás: a gyártó nyilatkozata az adott követelmény teljesítése vonatkozásában. Értékei lehetnek:

aa) „Nem alkalmazható”: akkor jelölhető, ha a VE vonatkozásában a követelmény nem értelmezhető, a VE fizikai kialakítása, tervezett funkciói és felhasználási területe a követelmény teljesítését nem teszi lehetővé.

ab) „Alkalmazható és teljesített”: akkor jelölhető, ha a VE vonatkozásában a követelmény értelmezhető, és a VE a követelményt teljesíti;

b) teljesítés módja: „Alkalmazható és teljesített” jelölés esetén annak leírása, hogy a követelmény kapcsán az MD-ben szereplő mely komponensek érintettek, és azok a követelményt egyesével vagy együtt hogyan teljesítik;

c) indokolás: „Nem alkalmazható” jelölés esetén annak indokolása az összes körülményre tekintettel.
