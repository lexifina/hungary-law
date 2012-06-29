## 3. A központi szerver

6. § (1) A központi szervert Magyarország területén, korlátozott hozzáférésű, biztonságos területen kell elhelyezni (szerverterem). A központi szerver kialakítása során szünetmentes tápellátást és illetéktelen személyek hozzáférését megakadályozó felépítést kell biztosítani. A központi szervert megfelelő fizikai és logikai behatolás elleni védelemmel (többek között vírusvédelemmel, tűzfallal) kell ellátni a jogosulatlan hozzáférések megakadályozása céljából. Egy szerverteremben kizárólag egy központi szerver helyezhető el és üzemeltethető, illetve a központi szerver tranzakciós szerverét és játékszerverét ugyanazon szerverteremben kell elhelyezni.

(2) A szerverterembe kizárólag az állami adóhatóság részére előzetesen írásban bejelentett személyek léphetnek be. A belépésről elektronikus beléptető rendszer által vezetett nyilvántartást kell vezetni, amely tartalmazza a belépő személyazonosító adatait, a belépés és távozás idejét és a belépés célját. A közigazgatási hatóságok hatósági ellenőrzéssel kapcsolatban a szerverterembe bármikor beléphetnek, a szerver működtetőjének biztosítania kell, hogy a központi szerver ellenőrzése bármikor akadálymentesen megtörténhessen.

(3) A központi szerver játékszerverét és tranzakciós szerverét másodlagos szerverrel kell ellátni, amely az elsődleges szerver szoftver- vagy hardveregységeinek meghibásodása esetén azonnal rendelkezésre áll és automatikusan, adatvesztés nélkül folytatja az elsődleges szerver működését. Az elsődleges szerverre alkalmazandó előírások a másodlagos szerverre is megfelelően irányadóak.

(4) A központi szervert úgy kell kialakítani, hogy az hiba esetén megvédje a kapcsolódó adatok integritását. Az ellenőrzési naplókat, a rendszer adatbázisokat és minden más kapcsolódó adatot ésszerű adatvédelmi módszerek alkalmazásával kell tárolni. A biztonsági mentést legalább naponta egyszer automatikusan el kell végezni.

(5) A központi szervernek naplóznia kell különösen

a) a kezdeti beállításokat és a változásokat,

b) a lejátszott játékokkal kapcsolatos összes lényegi információt, beleértve a tét/nyeremény adatokat, bonusz játékokat, a nyerőkombinációt, a nyeremény-kifizetés módját, a jackpot-változásokat,

c) az összes sikeres és sikertelen kapcsolódási kísérletet és eseményt,

d) a küldő és a cél azonosítási adatait (pl. IP cím, MAC cím, Port száma),

e) felhasználói belépéseket és kilépéseket,

f) biztonsági incidenseket,

g) minden olyan eseményt, amely indokoltan azt jelzi, hogy a rendszer nem az elvárásoknak megfelelően működik (pl. memóriahiba, öndiagnosztikai probléma).

(6) A naplónak tartalmaznia kell az esemény megnevezését, dátumát, idejét másodperc pontossággal és az eseményt egyértelműen azonosító minden egyéb információt. A naplóban minden egyes eseményt másodperc alapú időbélyeggel kell tárolni. A szerver működtetőjének biztosítania kell az ellenőrző hatóságok számára a naplók ellenőrizhetőségéhez szükséges hozzáférést.

(7) Az eredményként kapott naplókat megváltoztathatatlanná kell tenni. Az informatikai rendszernek biztosítania kell a naplók biztonságos, adatvesztés nélküli archiválását. Az archiválás során ki kell zárni az utólagos módosítás lehetőségét.

(8) A szerver és az ahhoz csatlakoztatott helyhez kötött szerver alapú pénznyerő automaták, illetve nem helyhez kötött pénznyerő rendszerek rendszeridejét valamelyik internetes atomórához naponta szinkronizálni kell.

(9) A központi szervernek biztosítania kell, hogy arra kizárólag az állami adóhatóság által engedélyezett helyhez kötött szerver alapú pénznyerő automata, illetve nem helyhez kötött szerver alapú pénznyerő rendszer csatlakozzon. Ennek érdekében a kommunikáció során a szervernek vizsgálnia kell a szerver alapú műszaki egység azonosítóját (különösen: szoftver és hardver azonosítás, hardver kulcs, MAC cím és PCB szám).

(10) A helyhez kötött szerver alapú pénznyerő automata, illetve a nem helyhez kötött pénznyerő rendszer működése során kizárólag a központi szerveren tárolható a játéklogika és a véletlenszám-generátor, ennek megfelelően a játékok eredményét kizárólag a központi szerveren lévő szoftver határozhatja meg.

(11) A szerveren az alábbi célokból hozzáférési jogosultságokat kell kialakítani:

1. Az állami adóhatóság jogosult bármikor a helyszínen, a központi szerveren található összes adat megtekintésére, valamint távoli hozzáféréssel az 1. melléklet szerinti adatok valós idejű és visszamenőleges lekérdezésére, ellenőrzésére, valamint a központi szerver, illetve az egyes játékok működtetésének azonnali felfüggesztésére, letiltására. A hozzáférésnek lehetővé kell tennie az adatok olvasását, másolását és a kimásolt adatok feldolgozását.

2. A helyhez kötött szerver alapú pénznyerő automata, illetve a nem helyhez kötött szerver alapú pénznyerő rendszer üzemeltetője jogosult távoli hozzáféréssel, jelszavas védelemmel és naplózással az adatbázisból a rá vonatkozó pénzügyi adatok és játékprogramok konfigurációs adatainak lekérdezésére.

3. A központi szerver működtetője jogosult a szerveren elhelyezett öndiagnosztikai programok futtatására, a szerver állapotára vonatkozó adatok lekérdezésre, tűzfal és vírusvédelem más jogosultsági szinthez nem tartozó beállításainak elvégzésére. A központi szerver működtetője jogosult távoli hozzáféréssel a szerveren elhelyezett öndiagnosztikai programok futtatására és az állapotra vonatkozó adatok lekérdezésére.

(12) A hatóságok akadálymentes hozzáférését és az adatok biztonságát garantáló szoftvert a központi szerver működtetőjének kell biztosítania.

(13) A központi szervernek öndiagnosztikai eljárást kell végeznie minden kritikus interfész elemnél (pl. hálózati eszközök, tűzfalak, harmadik felek csatlakozásai), és képesnek kell lennie eredményesen értesíteni a rendszeradminisztrátort az adott állapotról, amennyiben nem katasztrofális állapotról van szó. A központi szervernek képesnek kell lennie ezt az eljárást legalább 24 óránként egyszer elvégezni.

(14) A központi szervernek bármilyen kommunikációs hiba esetén azonnal értesítenie kell az működtetőt a hibásan működő részegységről, a rendszer minden egyes kritikus interfész eleme felé (központi szerver, tranzakciós szerver, hálózati eszközök, tűzfalak) jelentenie kell az öndiagnosztikai eljárás eredményeit.

(15) A központi szerver játékszerverének vezérlőprogramjait elektronikus aláírással kell ellátni, amely integritása a program, vagy programrészlet betöltésekor automatikus öndiagnosztikai eljárással ellenőrzésre kerül. Integritási hiba észlelése esetén az adott program, vagy programrészlet nem futtatható. A rendszernek automatikusan naplóznia kell a sikertelen hitelesítés dátumát, idejét és eredményét.

(16) A központi szerver működtetőjének az állami adóhatóság részére az 1. mellékletben előírt adatokat naponta, az állami adóhatóság által meghatározott formátumban a tárgynapot követő nap reggel 5.00 óráig továbbítania kell, illetve a továbbítás sikertelenségéről haladéktalanul értesítenie kell az állami adóhatóságot. Az adatokat tartalmazó fájlt elektronikus aláírással és titkosítással kell az állami adóhatóság részére továbbítani.
