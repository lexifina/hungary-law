2. § Ez a rendelet a kihirdetését követő 10. napon lép hatályba, rendelkezéseit a folyamatban lévő munkáknál is alkalmazni kell.

Melléklet a 21/1995. (VI. 29.) FM rendelethez

SZABÁLYZAT

A DIGITÁLIS FÖLDMÉRÉSI ALAPTÉRKÉPI ADATÁLLOMÁNYOK KÉSZÍTÉSÉRE ÉS KEZELÉSÉRE

Tartalomjegyzék

1. Sajátos célú földmérési munkák végrehajtása

2. Közigazgatási határok adatbázisa

3. Térképi adatállományok létrehozása

4. A községi koordináta-állomány

5. A térképi adatállományok rétegfelépítése

6. A digitális adatállományok földhivatali kezelése

6.1. A jogosultság

6.2. A térképi adatállomány könyvtár-szerkezete

6.3. A koordinációs vizsgálat, nyilvántartás, változásvezetés

6.3.1. Koordinációs vizsgálat, előzetes nyilvántartás

6.3.2. A változások végleges átvezetése

6.4. Adatállományok rendszerezése és mentése

Szabályzat

a digitális földmérési alaptérképi adatállományok készítésére és kezelésére

1. Sajátos célú földmérési munkák végrehajtása

1.1. Az egységes digitális földmérési adatállományok előállítása érdekében — tekintettel a földprivatizáció során keletkezett digitális adatállományokra — a Szabályzat hatálybalépése után a külterületeken csak számszerű (numerikus) felmérések végezhetők.

1.2. Az intézkedés vonatkozik a külterületeken végzett állami alapmunkákra, továbbá minden külterületi sajátos célú, a földmérési alaptérkép tartalmát érintő földmérési munkára. A rendelkezést minden olyan folyamatban lévő geodéziai munkára alkalmazni kell, amely készültségi foka ezt lehetővé teszi.

1.3.[^3] Az 1.1. pont szerinti numerikus munkavégzést kell alkalmazni a volt zártkertek esetében akkor, ha a felmérendő terület nagysága eléri vagy meghaladja a 2 ha-t.

1.4. A belterületen végzett sajátos célú földmérési munkát a vonatkozó szabályzatok és jogszabályok szerint kell elvégezni. Állami alapmunka keretében végzett belterületi új felmérést vagy a meglévő földmérési alaptérkép digitális átalakítását a Földművelésügyi és Vidékfejlesztési Minisztérium[^4] külön rendelkezése szerint kell végrehajtani.

1.5. A külterületi numerikus felméréseket a vonatkozó műszaki szabályzatok általános előírásai szerint kell végrehajtani. A természetben mért és koordinátákból számítható távolságok közötti megengedett legnagyobb eltérések a következők lehetnek:

0— 60 m között 20 cm

60—100 m között 30 cm

100—200 m között, illetve 200 m felett 40 cm

1.6.[^5] A koordináta-számítások során számítógéppel létrehozott koordináta-állományokat, a későbbi felhasználás érdekében, megfelelő számítógépes adathordozón kell megőrizni, illetve a létrehozott koordináta-állományt megfelelő számítógépes adathordozón a földhivatalnak át kell adni. A koordináták adatállományában a pont rendűségére és minőségére utaló kódszámot — az 1. számú függelék szerinti pontkódot — minden esetben meg kell adni.

1.7. A digitális földmérési alaptérkép készítése, valamint a földprivatizáció és a sajátos célú földmérési munka során létrehozott számítógépes térképi adatállományok rétegkiosztását a 2. számú függelék szerint kell kialakítani.

1.8. A sajátos célú földmérési munkák során készített térképi adatállományok megfelelő adathordozón is átadhatók a földhivatalnak. Ebben az esetben csak azokat a rajzi munkarészeket kell a földhivatal részére elkészíteni, amelyek szükségesek a digitális térképi adatállományok értelmezéséhez. Ilyenek lehetnek többek között:

— az alappontsűrítési munkarészek,

— a mérési jegyzetek,

— a pontszámos vázlatok stb.

2. Közigazgatási határok adatbázisa

2.1. A községek, a városok, a földhivatali körzetek, a megyék közigazgatási határainak és az állam határának (a továbbiakban: közigazgatási határ) töréspontjait számítógépes adatállományban kell tárolni (a továbbiakban: közigazgatási határ adatbázis).

2.2. A közigazgatási határ adatbázis koordináta-állományának létrehozása — az államhatár kivételével — a földhivatal feladata. Az államhatárra vonatkozó adatbázist a Földmérési és Távérzékelési Intézet (a továbbiakban: FÖMI) hozza létre. A koordináta-állományok kialakításának költségeit az állami alapmunka keret terhére kell biztosítani. Az így létrehozott koordináta-állományban bekövetkező változások átvezetését az intézmények alapfeladataik ellátása keretén belül végzik.

2.3.[^6] A közigazgatási határ adatbázis létrehozásához szükséges adatgyűjtést községenként és városonként, valamint a hatályos ingatlan-nyilvántartási jogszabályokban meghatározott megyei jogú városokban kerületenként (a továbbiakban: község), külön adatállományban kell végezni. Az állomány nevét a KSH település azonosítójának felhasználásával kell képezni. Az állomány kiterjesztésének a koordináta-állomány vetületi rendszerére kell utalni. Az adatokat ASCII 852 kódtábla alkalmazásával kell rögzíteni.

(1) A vetületi rendszerek jelölésére

BOV Budapest Önálló Városi sztereografikus vetületi rendszer

EOV Egységes Országos Vetületi rendszer

HER Henger-Észak vetületi Rendszer

HDR Henger-Dél vetületi Rendszer

HKR Henger-Közép vetületi Rendszer

STG SzTereoGrafikus vetületi rendszer

VTN VetüleT Nélküli rendszer

betűkombinációkat kell használni. A kiterjesztésben kis- vagy nagybetű használható (pl. ,,bov'' vagy ,,BOV'', ,,eov'' vagy ,,EOV'', ,,her'' vagy ,,HER''), azonban sem a könyvtárnévben, sem az állománynévben, sem pedig a kiterjesztésben ékezetes karaktert — számítástechnikai okok miatt — alkalmazni nem szabad.

(2) A közigazgatási határpontok adatállományát körzeti földhivatalonként szervezett könyvtárban kell elhelyezni. A könyvtár nevét a 3. számú függelék szerinti földhivatali számjel rendszer alapján kell meghatározni.

(3) Példák a közigazgatási határpontok könyvtár és állomány elnevezésére:

------------------------------------

Könyvtár- és állománynév | Jelentése

------------------------------------

a) :\10020\30261.eov | Heves megye (10), Földhivatal Füzesabony (020), Dormánd község (30261), EOV rendszer (eov);

b) :\10030\19123.stg | Heves megye (10), Földhivatal Gyöngyös (030), Gyöngyössolymos község (19123), sztereografikus vetületi rendszer (stg);

c) :\20011\24271.vtn | Zala megye (20), Földhivatali Kirendeltség Zalaszentgrót (011), Pakod község (24271), vetület nélküli rendszer (vtn);

d) :\13011\24013.stg | Pest megye (13), Földhivatali Kirendeltség Érd (011), Diósd község (24013), sztereografikus vetületi rendszer (stg).

2.4. Ha egy községnek szigetszerű domíniuma van egy másik község területén, vagy egy községen belül több vetületi rendszer fordul elő, ezek határpontjait az anyaközségtől külön állományban kell gyűjteni. Az állomány nevét az anyaközség KSH azonosítójából kell képezni a ,,_1'' karakterekkel való bővítéssel. Több domínium vagy kettőnél több vetületi rendszer esetén a bővítést 1-gyel növelni kell (,,_2'').

(1) Példák a domínium koordináta-állományának könyvtár és állomány elnevezésére:

------------------------------------

Könyvtár- és állománynév, Jelentése

------------------------------------

a) :\13090\04570_1.stg Pest megye, Földhivatal Vác, Márianosztra község, Márianosztra domíniuma;

b) :\10020\27517_1.stg Heves megye, Földhivatal Füzesabony, Besenyőtelek község, Besenyőtelek domíniuma.

2.5. A közigazgatási határpont azonosítója (pontszáma) kilenc karaktert tartalmaz, amelyből az első öt karakter a község KSH település azonosítóját, a következő négy karakter pedig a pont sorszámát jelenti. Amennyiben a település KSH kódjának első karaktere 0 (02015—09991), a KSH település azonosítóból csak a következő négy karaktert kell használni, tehát a határpont azonosítója nyolc karakterből fog állni.

2.6. Egy községen belül a határpontokat — tekintet nélkül a korábbi számozásra — az óramutató járásával egyező értelemben, egy tetszőlegesen kiválasztott hármashatár pont után következő első törésponttól kiindulva 1001-től (7999-ig) folyamatosan kell sorszámozni, függetlenül az esetleg eltérő vetületi rendszertől [azokat a pontokat is be kell számozni, amelyek más vetületi rendszerben vannak; lásd még a 2.10., illetve a 2.12. (3) pontot].

2.7. A település hármashatár pontjainak sorszámozását 0301-gyel (0399-ig) kell kezdeni. A domínium határpontjainak sorszámozását 8001-től (9999-ig) kiindulva kell elvégezni. Ha egy községnek több domíniuma van, a második domínium határpontjainak számozását az első domíniumban lévő határpontok sorszámai után következő 101-től, de legalább 50 szám kihagyásával kell folytatni (pl. 8301-től). A közigazgatási határpontok sorszámozását a hármashatár pontokkal kell kezdeni.

2.8. A közigazgatási határ pontjait I. rendű részletpontnak kell tekinteni. Minden határpont koordinátája után a pontkódot fel kell tüntetni. Az egységes kezelés érdekében az államhatár töréspontjait I. rendű részletpontnak — vagy elméleti pontnak — kell elfogadni és ennek megfelelően kell a koordináták után a pontkódokat alkalmazni.

2.9. Azokban a községekben, amelyekben a felmérés még nem az EOTR-ben készült, a határpontok adatállományát az ingatlan-nyilvántartási térkép vetületi rendszerében kell létrehozni. Az EOV-ba való transzformálást egységesen a FÖMI végzi el. A település határvonalának a jogilag érvényes állapotot kell tekinteni, függetlenül az esetleges területi és határvitáktól.

2.10. Ha két szomszédos község közül az egyikben a határpontok EOV rendszerben adottak, a másikban pedig még a régi vetületi rendszert használják, a régi vetület szerinti koordinátákat nem kell feltüntetni a koordináta-állományban a két hármashatár között. Ebben az esetben a hármashatár pontokat a 2.7. szerinti sorszámmal kell ellátni, a koordináta-állományban pedig a két hármas határpont között egy sort üresen kell hagyni. Hasonlóképpen kell eljárni államhatár esetében, vagyis az államhatár két hármas határpont közötti közbenső töréspontjainak koordinátáit nem kell megadni, de a pontokat sorszámozni kell.

2.11. Az adatállományoknak a sorok szerint (egy sor egy rekord) a következőket kell tartalmaznia:

(1) Az állomány első sorában a község nevét, a KSH rendszerben és a Magyar Köztársaság Helységnévtárában regisztrált módon kell megadni, amely max. 20 karakter lehet. Két karakterhely kihagyása után (a 23. karakter-helytől) a község ingatlan-nyilvántartás szerinti területét is — hektárban, négy tizedes élességgel — meg kell adni.

(2) Minden közigazgatási határpontot külön sorban — egy sor egy rekord — kell feltüntetni az alábbiak szerint (a sorokat nem kell számozni):

---------------------------------------------------

nnnnnnnnn yyyyyyy.yy xxxxxxx.xx zzzzzz.zzz kkkk

---------------------------------------------------

pont- y x z kód

azonosító koordináta koordináta koordináta

A rekordot a következők szerint kell értelmezni:

nnnnnnnnn pontazonosító (pontszám): 9 karakter

szóköz 2 karakter

yyyyyyy.yy y koordináta (előjellel), cm élességgel: max. 10 karakter

szóköz 2 karakter

xxxxxxx.xx x koordináta (előjellel), cm élességgel: max. 10 karakter

szóköz 2 karakter

zzzzzz.zzz z koordináta (ha szükséges): max. 10 karakter

szóköz 2 karakter

kkkk pontkód: max. 4 karakter

(3) A közigazgatási határpontok koordináta-állományában az egyes pontok magasságát nem kell megadni, illetve a z koordináta helyét nem kell 0-val kitölteni.

(4) Példa az adatállomány elnevezésére és a pontszámozásra

A:\13040\22035.stg (Megjegyzés: Pest megye, Földhivatal Gödöllő)

Zsámbok 2334.6580

220350301 —39918.32 —9336.78 3103

220351001 —40086.14 —9227.98 3103

(…)

220351061 —45666.50 —7337.20 3103

220350302 —45705.12 —7305.44 3102

(a két hármas határpont közötti sor üresen marad, mert eltérő vetületi rendszerben adottak a pontok, a köztük lévő pontokat azonban folyamatosan kell sorszámozni. Ilyenek a 220351062 és a 220351063 sorszámú pontok — lásd még a pontszámos vázlatot)

220350303 —45560.57 —6948.21 4142

220351064 —45498.94 —6770.19 4143

(…)

220350304 —43693.83 —4017.49 4143

220351097 —43479.27 —4240.10 4143

220351098 —43233.32 —4390.76 4143

(…)

220351146 —39912.25 —9328.47 4143

(5) A határpontokról alkalmas méretarányban községenként szerkesztett pontszámos vázlatot kell készíteni.

(6) A közigazgatási határ pontszámos vázlatán — az államhatár pontjai kivételével — azokat a határpontokat is fel kell tüntetni, amelyeket a 2.10. pont szerint a koordináta-állományban nem kell szerepeltetni (ezek EOV rendszerben adottak vagy az államhatár pontjai).

2.12. Abban a községben (és szomszédos községben), amelyben a határpontokra vonatkozó koordináta-jegyzék nem lelhető fel, a határpontok koordinátáit — az ingatlan-nyilvántartási térkép felhasználásával — manuális digitalizálással kell meghatározni. A digitalizálás pontossági előírásait a vonatkozó szakmai szabályzatok tartalmazzák. A digitalizálással meghatározott pontokat pontkóddal is kell ellátni.

2.13. Egy megyén belüli, ugyanazon vetületi rendszerben lévő községek közös határpontjainak azonosságát az illetékes földhivatalnak kell vizsgálni és az ellentmondásokat megszüntetni. A megyehatár töréspontjait a szomszédos megyék és a FÖMI is ellenőrzi. Az esetleges ellentmondásokat a megyei földhivatalok bevonásával szünteti meg.

2.14. A határpontok EOV-ba történő transzformálása után a község összterületét a FÖMI számítja és hasonlítja össze a nyilvántartott területtel. Amennyiben a területi hiba nagyobb mint a vonatkozó szakmai szabályzatok szerint megengedett legnagyobb eltérés, az eltérés okát a földhivatalnak kell megvizsgálni, illetve megszüntetni.

2.15. A határpontok EOV szerinti koordináta-állományát a FÖMI megküldi a földhivataloknak. A területi nagyságra is elfogadott (az eredeti vetületi rendszerben és az EOV-ben is) koordináta-állományokat kell a közigazgatási határok eredeti adatállományának tekinteni, és azok községenkénti egy-egy példányát az illetékes megyei földhivatalnál tárolni.

2.16. Az eredeti állomány egy másolata szolgál a változások vezetésére, amely az illetékes földhivatal feladata. Egyebekben a vonatkozó szabályzat előírásai szerint kell eljárni.

2.17. A közigazgatási határ adatbázisának létrehozásával egy időben meg kell határozni a község és a megye geokódját (centroidját) is. A geokód meghatározását és ábrázolását a vonatkozó jogszabályi előírások szerint kell elvégezni.

2.18. A község geokódját lehetőleg a polgármesteri hivatalra (kerületekben a kerületi polgármesteri hivatalra), a megye geokódját pedig a megyei önkormányzati hivatalra (Budapest főváros esetében a főpolgármesteri hivatalra) vonatkozóan kell meghatározni.

2.19. A Magyar Köztársaság, a megye és a község geokódjának pontszáma, a 2.5. pontban meghatározott elvek alapján, kilenc karakterből áll. A geokódot pontkóddal is el kell látni.

(1) A Magyar Köztársaság geokódjának pontszáma 100000000, amelyet az Országházra kell meghatározni.

(2) A megye geokódjának pontszáma 100000001—100000020 terjedhet. A karaktersorozat utolsó két elemét a KSH megye azonosítója szerint kell kialakítani (pl. 100000001 Budapest főváros; 100000016 Jász-Nagykun-Szolnok megye stb.).

(3) Község esetében az első öt karakter az érintett közigazgatási egység KSH település azonosítója (domínium esetében az anyaközség azonosítójával egyező), a következő négy karakter pedig a geokód sorszámát jelenti, amelyre 0501-től 0599-ig sorszámot lehet felhasználni (pl. 220350501 Zsámbok község geokódja). Domínium vonatkozásában a sorszámozást az anyaközség után folyamatosan kell végezni (pl. 225170502 Besenyőtelek község domíniumának geokódja).

3. Térképi adatállományok létrehozása

3.1.[^7] A térképi adatállományok létrehozása előtt a közigazgatási határt, a 2. pont szerinti adatok felhasználásával, ezen belül pedig a fekvéshatárokat is meg kell szerkeszteni, az előírt rétegkiosztás szerint.

3.2. A térképi adatállományokat az ingatlan-nyilvántartási térkép vetületi rendszerében kell létrehozni. A térképi adatállománynak a jogi állapotot kell tartalmaznia, ezért a digitális földmérési alaptérkép és a digitális ingatlan-nyilvántartási térkép azonos térképi adatállományt képez.

3.3. A földhivatalhoz megfelelő számítógépes adathordozón benyújtott földmérési munkákat (kárpótlási, részarány-tulajdoni, egyéb bejelentésre kötelezett munkák) a 6.3. pont szerint lehet a térképi adatállományba bevinni. Az analóg formában leadott munkákat a vizsgálatot és a záradékolást követően kell a térképi adatállományba betölteni.

4. A községi koordináta-állomány

4.1. A községben előforduló bármely pont csak az eredetére és minőségére utaló pontkód feltüntetésével szerepelhet a számítógépen kezelt koordináta-állományban.

4.2. A vízszintes koordinátákat cm élességgel kell feltüntetni. Magassági alappontok esetében a magasságokat, a III. rendű magassági alappontokkal bezárólag, mm élességgel kell megadni.

4.3. A koordináta-állomány része a digitális térképnek, külön koordináta-állományban csak a közigazgatási határpontok koordinátáit kell nyilvántartani jelen szabályzat 2. pontja szerint.

5. A térképi adatállományok rétegfelépítése

5.1. A számítógépen kezelhető földmérési alaptérképi adatállományok vonalait különböző rétegekben kell tárolni aszerint, hogy azok milyen funkciót töltenek be. Elsődlegesen a vonal magasabb funkciója szerint kell a megfelelő réteget kiválasztani, de jelentése alapján a (határ)vonalat több rétegben is ábrázolni kell.

5.2. A rétegkiosztást a digitális földmérési alaptérkép készítése, analóg földmérési alaptérkép digitalizálással vagy szerkesztéssel történő digitális átalakítása, valamint annak tartalmában változást eredményező minden földmérési (kárpótlás, részaránytulajdon, sajátos célú, mérnökgeodéziai stb.) munka során kötelezően kell alkalmazni.

5.3. A rétegek megnevezését minden térképi adatállományban fel kell tüntetni. Az előírt rétegkiosztás — a felhasználó igényei szerint — bővíthető.

5.4. Amennyiben az adatállomány előállításakor további rétegek is felhasználásra kerülnek, az új rétegek megnevezését mind az adatállományában, mind pedig a műszaki leírásban — röviden ismertetve a jelentését is — meg kell adni. Ennek hiányában a földhivatal a munkát nem veszi át.

6. A digitális adatállományok földhivatali kezelése

6.1. A jogosultság

(1) A földhivatalban a digitális (koordináta és térképi) adatállományokat csak az arra feljogosított személy(ek) kezelheti(k). A jogosultságot jelszó használatával kell biztosítani.

6.2. A térképi adatállomány könyvtár-szerkezete

(1) A térképi adatállomány könyvtárait az alábbiak szerint kell kialakítani.

(2) Főkönyvtár: :\[község azonosító (max. 8 karakter)]

amelyet a KSH megye és település azonosító számából, továbbá ,,T'' kiterjesztésből (,,T'' a térképre utal) kell képezni [pl. :\1220190.T (Nógrád megye, Lucfalva község)]. Domíniumok könyvtárnevét az anyaközség KSH azonosítóinak felhasználásával és a ,,T'' kiterjesztés számbővítésével kell kialakítani [pl. :\1304570.T1 (Márianosztra község domíniuma)]. Több domínium esetében a 2.4. pont rendelkezéseit kell értelemszerűen alkalmazni.

(3) Alkönyvtárak:

------------

Könyvtárnév

Jelentése

------------

a) :\[község azonosító]\JOGEROS

a digitális ingatlan-nyilvántartási térkép, az előírt rétegkiosztás szerint, amely azonos a digitális földmérési alaptérképpel;

b) :\[község azonosító]\ELOZETES

a jogerőre még nem emelkedett változások előzetes átvezetése a község térképi adatállományban;

c) :\[község azonosító]\VALTOZAS

a községben készített koordinációs vizsgálatra leadott sajátos célú földmérési munka az előírt pontkódokkal és rétegkiosztással;

d) :\[községnév]\MUNKA

közbenső állomány a koordinációs vizsgálathoz és rétegműveletekhez;

e) :\[község azonosító]\NAPLO

a térképi állományban végzett műveletek naplózásához.

6.3. A koordinációs vizsgálat, nyilvántartás, változásvezetés

(1) A koordinációs vizsgálatra beérkezett munkát az alábbiak szerint kell kezelni:

6.3.1. Koordinációs vizsgálat, előzetes nyilvántartás

(1) A vizsgálatra leadott, az alaptérkép tartalmában változást eredményező sajátos célú geodéziai munka földhivatali iktatószámát az ,,ELOZETES'' alkönyvtár adatállományába, a megfelelő réteg bekapcsolásával, az érintett földrészletekbe be kell vezetni. Amennyiben a földmérési munka bejelentésre kötelezett, a bejelentés iktatószámát a földhivatali visszaigazolással egy időben kell az ,,ELOZETES'' alkönyvtárban, az érintett földrészleteken belül feltüntetni.

(2) A beérkezett munkát az adatlemezről, a vírusvizsgálat elvégzése után, a ,,VALTOZAS'' és a ,,MUNKA'' alkönyvtárakba kell másolni. A bemásolásra kerülő adatállománynak a vizsgálatra benyújtott munka iktatószámából kialakított nevet kell adni. Az állomány kiterjesztése a benyújtás évére utal.

Például

:\[főkönyvtár]\[alkönyvtár]\file-név<iktatószám>.<kit>

:\1220190.T\VALTOZAS\12_25.94

:\1220190.T\MUNKA\12_25.94

(3) A koordinációs vizsgálat lefolytatásához a változással érintett területhez csatlakozó részeket a ,,JOGEROS'' (és esetleg az ,,ELOZETES'') alkönyvtárból be kell másolni a ,,VALTOZAS'' és a ,,MUNKA'' alkönyvtárba, majd a vizsgálatot el kell végezni. Az észlelt hibákról vizsgálati jegyzőkönyvet kell készíteni. Az átvételre alkalmatlan változási munkát a vállalkozónak vissza kell adni, és az adatokat mind a ,,VALTOZAS'', mind pedig a ,,MUNKA'' alkönyvtárból törölni kell.

(4) A hibátlan, de jogerőre még nem emelkedett munkát (pl. telekmegosztás) az ,,ELOZETES'' alkönyvtárban lévő adatállományba kell másolni, a megfelelő rétegek felhasználásával. A vizsgálat után jogerőre emelkedett változásokat (pl. épület feltüntetés) a ,,JOGEROS'' alkönyvtár adatállományába kell bemásolni, azonban az ,,ELOZETES'' alkönyvtárban a záradékolás iktatószámát meg kell tartani.

(5) A ,,JOGEROS'' vagy az ,,ELOZETES'' alkönyvtárban átvezetett változásokat a ,,VALTOZAS'' és a ,,MUNKA'' alkönyvtárból törölni kell.

(6) A javításra visszaadott munkát a ,,MUNKA'' alkönyvtárban mindaddig meg kell tartani, amíg a hibajavítás nem történik meg. A javítás végrehajtását ellenőrizni kell. A javítás elfogadása után a 6.3.1. (4) és (5) pontok szerint kell eljárni.

(7) Az adatállománnyal végzett minden műveletet naplózni kell. A naplózást úgy kell végrehajtani, hogy abból egyértelműen megállapítható legyen a műveletet végző személye, illetve az általa végzett művelet. A naplózást mind a ,,JOGEROS'', mind pedig az ,,ELOZETES'' alkönyvtárban végzett bármely műveletnél el kell végezni, azonban a vizsgált adatállomány törlése előtt a naplót a ,,NAPLO'' alkönyvtárba kell másolni. A napló file-nevét (2) pont szerint kell megadni. A ,,NAPLO'' alkönyvtárban levő naplófile-okat törölni nem szabad.

6.3.2. A változások végleges átvezetése

(1) A változási okirat jogerőre emelkedése után az ,,ELOZETES'' alkönyvtárban ki kell keresni az adott földrészlet állományát. A változott részletekről le kell választani a jogerős részleteket és a változást a ,,JOGEROS'' alkönyvtárba kell másolni. Ügyelni kell arra, hogy átmásolás után a határvonalak (az élek) mindenütt meglegyenek.

(2) Az átvezetés helyességét a csoport (tömb) földrészlet szintű területszámításával is ellenőrizni kell.

(3) A végleges átvezetés folyamatát is naplóban kell rögzíteni.

(4) A ,,JOGEROS'' alkönyvtárban levő adatállományokat minden negyedév első hónapjának 15. napjáig kell a megyei földhivatalnak megküldeni. Ha a tárgyévben változás nem történt, a jogerős adatállományt a következő év január 15-ig kell a másodfokú földhivatalba megküldeni, azonban negyedévenként írásban tájékoztatni kell a megyei földhivatalt az állományok változatlanságáról.

6.4. Adatállományok rendszerezése és mentése

(1) A digitális (koordináta és térképi) adatállományokat községenként kell a megfelelő számítógépes adathordozón tárolni, külön adathordozón a közigazgatási határ koordináta-állományát és külön adathordozón a térképi adatállományt. Az eredeti adatállományokból két példányt kell készíteni, amelyeket egymástól fizikailag is elkülönítetten — a megyei és körzeti földhivatalban — kell elhelyezni. A körzeti földhivatal az eredeti adatállományokról egy példány másolatot készít, amely az állományokban bekövetkezett változások vezetésére szolgál.

(2) A 6.3.2. (4) pont szerint a megyei földhivatalba küldött jogerős adatállományokat három példányban kell elkészíteni, amelyből egy a megyei földhivatalhoz kerül, egy a későbbi feldolgozásra használható, egyet pedig további ,,mester'' lemezként kell megőrizni. A jogerős adatállományokról negyedévenként akkor is el kell készíteni a három példány másolatot, ha az adott időszakban az állományokban változás nem következett be. A ,,mester'' lemezek tartalma nem írható felül.

(3) A napi munka befejezésével a kezelt állományokat — számítástechnikailag megfelelő módon — naponta két példányban kell kimenteni, amelyekből az egyik példányt a 6.3.2. (4) pontban megjelölt határidőig változatlan tartalommal meg kell őrizni.

(4) A számítógépbe csak a napi munkához szükséges munkaterületet lehet betölteni. Más munkaterületre való átlépés előtt vagy a napi munka befejeztével a számítógépben levő adatállományt — a (3) pontban előírt módon — ki kell menteni. Mentés után a számítógépből a munkaterületet törölni kell.

(5)[^8] Az adatállományokról nyilvántartást (katalógust) kell vezetni. A katalógusnak tartalmaznia kell minden olyan adatot, amely egyértelműen elősegíti a számítógépes adathordozó tartalmának azonosítását. A nyilvántartásban fel kell tüntetni a földhivatali körzet számjelét és nevét, a község KSH település azonosítóját és nevét, valamint az állomány megnevezését, példányszámát, a változás dátumát, a változást átvezető személy nevét, továbbá azt, hogy a jogerős adatállomány mikor lett a másodfokú földhivatalba küldve.

1. számú függelék[^9]

PONTKÓDOK

a digitális állami földmérési alaptérképi adatállományokban

PONTKÓDOK

a digitális állami földmérési alaptérképi adatállományokban

| Sor- szám | A pont | Az állandósítás | Határpont | DAT T_ KOZEP- HIBA kód |

| rendűsége | kódja | módja | kódja | jellege | kódja |

| karakterhelyek |

| 1. (–2.) |  | 2. (3.) |  | 3. (4.) |

| 1. ALAPPONTOK |

| 1.1. Vízszintes alappontok |

| 1.1.1. | OGPSH1 | 20 |  |  |  |  | 1 |

| 1.1.2. | I–III. rendű | 5 |  |  |  |  | 2 |

| 1.1.3. | IV. rendű | 1 |  |  |  |  | 3 |

| 1.1.4. | V. rendű | 2 |  |  |  |  | 4 |

| 1.1.5. | felmérési, földi | 3 |  |  |  |  | 5 |

| 1.1.6. | felmérési, fotós | 4 |  |  |  |  |  |

|  |  |  | ideiglenes jelölés | 0 |  |  |  |

|  |  |  | kő | 1 |  |  |  |

|  |  |  | kő halom | 2 |  |  |  |

|  |  |  | vb. mérőtorony | 3 |  |  |  |

|  |  |  | templomtorony | 4 |  |  |  |

|  |  |  | vasszekrény | 5 |  |  |  |

|  |  |  | gyárkémény | 6 |  |  |  |

|  |  |  | egyéb | 7 |  |  |  |

|  |  |  | csap, Hilti | 8 |  |  |  |

|  |  |  | egyéb felszíni2 | 9 |  |  |  |

|  |  |  |  |  | nem határpont | 0 |  |

|  |  |  |  |  | államhatár pont | 1 |  |

|  |  |  |  |  | megyehatár pont | 2 |  |

|  |  |  |  |  | községhatár pont | 3 |  |

|  |  |  |  |  | fekvéshatár pont | 4 |  |

|  |  |  |  |  | földrészlet határpont | 5 |  |

|  |  |  |  |  | egyéb részletpont | 6 |  |

| 1.2. Magassági alappontok |

| 1.2.1. | gravimetriai alappont3 | 6 |  | 0 |  | 0 | 24 |

| 1.2.2. | 0. rendű kéregmozgási4 | 6 | földalatti jel | 0 |  |  | 26 |

| 1.2.3. | I. rendű | 7 |  |  |  |  | 27 |

| 1.2.4. | II. rendű | 8 |  |  |  |  | 28 |

| 1.2.5. | III. rendű | 9 |  |  |  |  | 29 |

| 1.2.6. | IV. rendű | 10 |  |  |  |  | 30 |

|  |  |  | kőben gomb | 1 |  |  |  |

|  |  |  | csap | 2 |  |  |  |

|  |  |  | tárcsa | 3 |  |  |  |

|  |  |  | gomb | 4 |  |  |  |

|  |  |  | egyéb5 | 5 |  |  |  |

|  |  |  |  |  | Balti | 1 |  |

|  |  |  |  |  | EOMA | 2 |  |

| Sor- szám | A pont | Az állandósítás | Határpont | DAT T_ KOZEP- HIBA kód |

| rendűsége | kódja | módja | kódja | jellege | kódja |

| karakterhelyek |

| 1–2. |  | 3. |  | 4. |

| 2. RÉSZLETPONTOK |

| 2.1. Vízszintes részletpontok |

| 2.1.1. Numerikus részletpontok |

| 1. | I. rendű |  |  |  |  |  |  |

| a) | újfelmérés | 31 |  |  |  |  | 6, 8 |

| b) | digitális átalakítás | 36 |  |  |  |  | 7, 9 |

| 2. | II. rendű |  |  |  |  |  |  |

| a) | újfelmérés | 32 |  |  |  |  | 10, 12 |

| b) | digitális átalakítás | 37 |  |  |  |  | 11, 13 |

| 3. | III. rendű |  |  |  |  |  |  |

| a) | újfelmérés | 33 |  |  |  |  | 14, 16 |

| b) | digitális átalakítás | 38 |  |  |  |  | 15, 17 |

| 4. | IV. rendű |  |  |  |  |  |  |

| a) | újfelmérés | 34 |  |  |  |  | 18, 20 |

| b) | digitális átalakítás | 39 |  |  |  |  | 19, 21 |

| 5. | V. rendű | 35 |  |  |  |  | 22 |

|  |  |  | terepen nem jelölt | 1 |  |  |  |

|  |  |  | ideiglenes jelölés | 2 |  |  |  |

|  |  |  | építm. domináns pontja | 3 |  |  |  |

|  |  |  | kő | 4 |  |  |  |

|  |  |  | csap | 5 |  |  |  |

|  |  |  | festés | 6 |  |  |  |

|  |  |  | szeg, Hilti | 7 |  |  |  |

|  |  |  | határdomb6 | 8 |  |  |  |

|  |  |  | egyéb azonosító jelölés | 9 |  |  |  |

|  |  |  |  |  | államhatár pont | 1 |  |

|  |  |  |  |  | megyehatár pont | 2 |  |

|  |  |  |  |  | községhatár pont | 3 |  |

|  |  |  |  |  | fekvéshatár pont | 4 |  |

|  |  |  |  |  | földrészlet határpont | 5 |  |

|  |  |  |  |  | egyéb részletpont | 6 |  |

| 2.1.2. Grafikus (digitalizált) részletpontok |

| 1. | I. rendű | 41 |  |  |  |  | 7, 9 |

| 2. | II. rendű | 42 |  |  |  |  | 11, 22 |

| 3. | III. rendű | 43 |  |  |  |  | 15, 17 |

| 4. | IV. rendű | 44 |  |  |  |  | 19, 21 |

|  |  |  | terepen nem jelölt | 1 |  |  |  |

|  |  |  | építm. domináns pontja | 3 |  |  |  |

|  |  |  | kő | 4 |  |  |  |

|  |  |  | csap | 5 |  |  |  |

|  |  |  | határdomb | 8 |  |  |  |

|  |  |  | egyéb azonosító jelölés | 9 |  |  |  |

|  |  |  |  |  | államhatár pont | 1 |  |

|  |  |  |  |  | megyehatár pont | 2 |  |

|  |  |  |  |  | községhatár pont | 3 |  |

|  |  |  |  |  | fekvéshatár pont | 4 |  |

|  |  |  |  |  | földrészlet határpont | 5 |  |

|  |  |  |  |  | egyéb részletpont | 6 |  |

| 5. | V. rendű | 45 | terepen nem jelölt | 1 |  | 6 | 22 |

| 2.1.3. Elméleti részletpontok |

| 1. | páros pontokból | 51 |  |  |  |  | rendűség- nek meg- felelő |

| 2. | egyéb elméleti | 52 |  |  |  |  |

|  |  |  | terepen nem jelölt | 1 |  |  |

|  |  |  |  |  | államhatár pont | 1 |

|  |  |  |  |  | megyehatár pont | 2 |

|  |  |  |  |  | községhatár pont | 3 |

|  |  |  |  |  | fekvéshatár pont | 4 |

|  |  |  |  |  | földrészlet határpont | 5 |

|  |  |  |  |  | egyéb részletpont | 6 |

| 3. | jelkulcs fogópontja7 | 52 | terepen nem jelölt | 1 |  | 6 |

| 2.2. Magassági részletpontok |

| 2.2.1. Mért részletpontok |

| 2.2.1.1. Balti alapszint |

| 1. | I. rendű |  |  |  |  |  |  |

| a) | belterületen M1 | 61 |  |  |  |  | 31 |

| b) | külterületen M1 | 66 |  |  |  |  | 32 |

| 2. | II. rendű |  |  |  |  |  |  |

| a) | belterületen M1 | 62 |  |  |  |  | 33 |

| b) | külterületen M1 | 67 |  |  |  |  | 34 |

| 3. | III. rendű |  |  |  |  |  |  |

| a) | belterületen M1 | 63 |  |  |  |  | 35 |

| b) | külterületen M1 | 68 |  |  |  |  | 36 |

|  |  |  | állandósított vízsz. ap. | 4 |  |  |  |

|  |  |  | egyéb azonosító jelölés | 9 |  |  |  |

|  |  |  |  |  | megyehatár pont | 2 |  |

|  |  |  |  |  | községhatár pont | 3 |  |

|  |  |  |  |  | fekvéshatár pont | 4 |  |

|  |  |  |  |  | földrészlet határpont | 5 |  |

|  |  |  |  |  | egyéb részletpont | 6 |  |

| 2.2.1.2. EOMA |

| 1. | I. rendű |  |  |  |  |  |  |

| a) | belterületen M1 | 71 |  |  |  |  | 31 |

| b) | külterületen M1 | 76 |  |  |  |  | 32 |

| 2. | II. rendű |  |  |  |  |  |  |

| a) | belterületen M1 | 72 |  |  |  |  | 33 |

| b) | külterületen M1 | 77 |  |  |  |  | 34 |

| 3. | III. rendű |  |  |  |  |  |  |

| a) | belterületen M1 | 73 |  |  |  |  | 35 |

| b) | külterületen M1 | 78 |  |  |  |  | 36 |

|  |  |  | állandósított vízsz. ap. | 4 |  |  |  |

|  |  |  | egyéb azonosító jelölés | 9 |  |  |  |

|  |  |  |  |  | megyehatár pont | 2 |  |

|  |  |  |  |  | községhatár pont | 3 |  |

|  |  |  |  |  | fekvéshatár pont | 4 |  |

|  |  |  |  |  | földrészlet határpont | 5 |  |

|  |  |  |  |  | egyéb részletpont | 6 |  |

| 2.2.2. Grafikus részletpontok |

| 2.2.2.1. Balti alapszint |

| 1. | fő- és alapszintvonal | 81 |  | 1 |  | 0 | 37 |

| 2. | mellékszintvonal (felező, negyedelő) | 82 |  | 1 |  | 0 | 37 |

| 3. | domborzati idom | 83 |  | 1 |  | 0 | 37 |

| 4. | kótált pont | 84 |  | 1 |  | 0 |  |

| 2.2.2.2. EOMA |

| 1. | fő- és alapszintvonal | 91 |  | 1 |  | 0 | 37 |

| 2. | mellékszintvonal (felező, negyedelő) | 92 |  | 1 |  | 0 | 37 |

| 3. | domborzati idom | 93 |  | 1 |  | 0 | 37 |

| 4. | kótált pont | 94 |  | 1 |  | 0 |  |

1 Az 1.1.1.− 1.1.3. sorszám alatti vízszintes alappontok adatait (állandósítási kód stb.) DAT átalakításakor a FÖMI alappont adatbázisából kell átvenni.

2 Kő betonoszloppal, pillér (nem magaspont), vasasztal, vasoszlop.

3 Az 1.2.1− 1.2.5. sorszám alatti magassági alappontok adatait (állandósítási kód stb.) DAT átalakításakor a FÖMI alappont adatbázisából kell átvenni.

4 A magassági főalappontot is az 1.2.2. pont alatti kóddal kell ellátni (középhiba kódja: 25).

5 Pl. furatos tábla, fali gomb, konzolos pontjelölés.

6 A határdomb, a határdomb kővel és a határdomb faoszloppal jelöléseket jelkulcsi jellel kell különböztetni.

7 Nem objektumot ábrázoló jelkulcsok (pl. kapcsolójel, a vízfolyás iránya), illetve lépcsőfokok, vasbeton- és acélhidak jelkulcsi ábrázolásához szükséges vonalak végpontjai.

A térképi elemek kódolási szabályai

1. Numerikus részletpontnak kell tekinteni minden számszerűen meghatározott pontot [Fttv. 9. § (4) bekezdés]. Ezen belül

a) újfelmérés alatt a helyszíni (terepi) adatgyűjtést,

b) digitális átalakításon pedig a korábban numerikusan meghatározott (pl. szabatos városmérés során mért és számított) részletpontok számítógépes feldolgozását

kell érteni.

2. Grafikus részletpontnak az 1. pont alá nem tartozókat (térképről mért koordinátákkal rendelkező, numerizált vagy digitalizált) részletpontokat kell tekinteni.

3. Ha különböző rendű pontok által meghatározott vonalak metszik egymást, a metszéspont az alacsonyabb rendű pont kódját kapja (pl. I. és II. rendű pontokból álló vonal metszi az I. rendű pontok által meghatározott vonalat, a metszéspont II. rendű lesz). A metszéspontok állandósítási kódja minden esetben 1.

4. A térbeli kitérő vonalak (pl. távvezeték és földrészlet határ) síkrajzi metszése esetében metszéspontot nem kell számítani.

5. Közigazgatási határok (melléklet 2.8 pont), a fekvéshatárok, továbbá a belterületi földrészletek közterülettel érintkező pontjai I. rendű részletpontoknak minősülnek.

6. A természetben meg nem jelölt földrészlet határpont állandósítási kódja 1. Ha a földrészlet határpont épület vagy burkolat pontjával azonos, állandósítási kódja 3.

7. A geokódot egységesen 5216 kóddal kell ellátni.

8. A termőföld privatizáció (kárpótlás–KP, részarány-tulajdon rendezés–RA) során kialakult termőföld minőségi osztályok határpontjainak kódja egységesen 3516. A későbbiekben digitalizálással meghatározott minőségi osztály határpontok kódja minden esetben 4516.

9. II. rendű részletpontnak kell tekinteni

a) az épületek,

b) az alaprajzukkal ábrázolt építmények és tereptárgyak,

c) a hidak és felüljárók,

d) a távvezetékek alaprajzzal ábrázolt műtárgyainak, tartóinak, továbbá

e) az alaprajzzal ábrázolt vízi közművek, a vízügyi műtárgyak

töréspontjait, kivéve, ha azok nem elégítik ki – a külön szabályzatban – az azonosításra előírt középhibát. Az állandósítási kód minden esetben 3.

10. III. rendű részletpontok közé kell sorolni

a) az épülettartozékok (tartópillér, terasz, lépcső, levetített sík stb.),

b) a töltések és földművek,

c) jelkulccsal megjelenített építmények, tereptárgyak, köztéri szobrok és emlékművek,

d) a burkolatok (út- és járdaburkolat), az áteresz,

e) a vasutak és a kötélpályák, a távvezetékek tengelyvonalának, illetve jelkulcsi ábrázolású műtárgyai, valamint

f) a vízi közművek és a vízügyi műtárgyak jelkulccsal ábrázolt

töréspontjait. Ezen pontok állandósítási kódja egységes 3.

11. A digitalizált kerítések és támfalak kódja minden esetben 4336.

12. Az árkok pontjai IV. rendűek. Az állandósítási kód egységesen 9.

13. Az alrészletek töréspontjai IV. rendű részletpontok, kódjuk 3416 vagy 4416. Ha épület vagy útburkolat töréspontjával azonos az alrészlet töréspontja, kódja 3436 vagy 4436 lesz.

14. A folyók (csatornák) és állóvizek partvonalának (medervonalának) töréspontjai IV. rendű részletpontnak minősülnek, állandósítási kódjuk 1.

15. A térképszelvények sarokpontjai egységesen 5216 kódot kapják (egyéb elméleti pont).

2. számú függelék[^10]

A DIGITÁLIS ÁLLAMI FÖLDMÉRÉSI ALAPTÉRKÉP ÉS A VÁLTOZÁSI VÁZRAJZ

RÉTEG-KIOSZTÁSA

2. függelék

A DIGITÁLIS ÁLLAMI FÖLDMÉRÉSI ALAPTÉRKÉP ÉS A VÁLTOZÁSI VÁZRAJZ

RÉTEG-KIOSZTÁSA

| Sor- szám | A térképi elem megnevezése | DAT objektumféleség | Réteg | A vonal (jelkulcs) | A DAT felirat | DAT jelkulcs | Alap- adat jelleg |

| kód | név | stílusa | vastag- sága | tartalma | típusa |

| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 |

| 1. GEODÉZIAI ALAPPONTOK |

| 1.1. Vízszintes és OGPSH alappontok |

| 1.1.1. | felső- és negyedrendű alappont | AA02–03 | 1 | V_ALAPPONT |  |  | pontazonosító | 2,5 Á | JKDATA02–09, 23 | 1 |

| 1.1.2. | ötödrendű alappont | AA04 |  |  | JKDATA09–15, 23 | 1 |

| 1.1.3. | felmérési alappont | AA05 |  | 1,8 Á | JKDATA16–22 | 1 |

| 1.1.4. | OGPSH alappont | AA01 | 76 | OGPSH_PONT |  |  |  | 2,5 Á | JKDATA01 | 1 |

| 1.2. Magassági és gravimetriai alappontok |

| 1.2.1. | 0. rendű kéregmozgási alappont | AB03 | 77 | KÉREG_MOZ |  |  |  | 2,5 Á | JKDATA25 | 1 |

| 1.2.2. | főalappont | AB02 | 2 | M_ALAPPONT |  |  |  |  | 1 |

| 1.2.3. | I–III. rendű alappont | AB04–07 | pontazonosító | 1,8 Á | JKDATA26–28 | 1 |

| 1.2.4. | IV. rendű alappont |  |  | 1 |

| 1.2.5. | geodéziai gravimetriai alappont | AB01 | 3 | GR_ALAPPONT |  |  | pontaz+Gr. | 2,5 Á | JKDATA24 | 1 |

| 2. HATÁRVONALAK, HATÁRPONTOK |

| 2.1. Közigazgatási határok |

| 2.1.1. | államhatár | BA01 | 4 | ÁLLAMHATÁR | 4–1–0,4–1–0,4–1–0,4–1 (jelkulcs) folytonos |  | országnév | 7,0 ND | JKDATB01 | 1 |

|  |  |  |  |  | pontazonosító | 1,8 Á | JKDATA10 | 1 |

| 2.1.2. | megyehatár | BA02 | 5 | MEGYEHATÁR | 0,4 | megyenév | 3,0 ND | JKDATB01 | 1 |

|  |  |  |  |  | pontazonosító | 1,8 Á | JKDATA16–17, 22, 30–34 | 1 |

| 2.1.3. | településhatár | BA04 | 6 | TELEPÜLÉSHAT | 0,18 | településnév | 7,0 ND | JKDATB01 | 1 |

|  |  |  |  |  | pontazonosító | 1,5 Á | JKDATA16–17, 22, 30–34 | 1 |

| 2.1.4. | fekvéshatár | BB01 | 7 | FEKVÉSHATÁR | 5–1–0,4–1–0,4–1 (jelkulcs) folytonos | 0,4 | fekvés neve | 3,0 ND | JKDATB02–03 | 1 |

| pontazonosító | 1,5 Á | JKDATA16–17, 22, 30–34 | 1 |

| 2.1.5. | kerülethatár | BB02 | 8 | KERÜLETHATÁR | kerületnév (-szám) | 5,0 ND |  | 1 |

| 0,18 | pontazonosító | 1,5 Á | JKDATA16–17, 22 | 1 |

| 2.1.6. | tömbhatár | BB05 | 9 | TÖMBHATÁR | folytonos | 0,3 | tömbszám (arab) | 3,0 D | JKDATA29–30 | 1 |

| 2.2. A földrészlet adatai és határvonalai |

| 2.2.1. | földrészlet határvonala | BC01–08; BD01–02 | 10 | FRL_HATÁR | folytonos | 0,18 |  |  | JKDATA29–30 | 1 |

| 2.2.2. | helyrajzi szám (jogerős) |  | 11 | HRSZ |  |  | helyrajzi szám | 2,0 D |  | 1 |

| 2.2.3. | alrészlet határvonala | BE01 | 12 | ALR_HATÁR | pontsor (0,5–0,5) | 0,18 |  |  |  | 1 |

| 2.2.4. | alrészlet betűjele |  | 13 | ALR_JEL |  |  | betűjel | 2,0 kD |  | 1 |

| 2.2.5. | alrészlet művelési ága | BE02 | 14 | ALR_MŰV_ÁG |  |  | művelési ág | 1,5 kD |  | 1 |

| 2.2.6. | minőségi osztály határvonala és megírása | BF01 | 15 | MIN_OSZT | szaggatott (3–1) | 0,18 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 2.2.7. | szabvány alatti kapcsolt alrészlet és megírása | BE03–04 | 16 | SZA_ALR | pontsor (0,5–0,5) | 0,18 | művelési ág | 1,5 kD |  | 1 |

| 2.2.8. | szabvány alatti minőségi osztály és megírása | BF02 | 17 | SZA_MIN_OSZT | szaggatott (3–1) | 0,18 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 2.3. A földrészlet előzetes változásai |

| 2.3.1. | földrészlet előzetes határa | BC01–08; BD01–02 | 18 | ELŐ_FRL_HAT | folytonos | 0,5 |  |  |  | 1 |

| 2.3.2. | előzetes helyrajzi szám |  | 19 | ELŐ_HRSZ |  |  | helyrajzi szám | 2,0 D |  | 1 |

| 2.3.3. | változott alrészlet határvonala | BE01 | 20 | VÁLT_ALR | pontsor (0,5–0,5) | 0,3 |  |  |  | 1 |

| 2.3.4. | változott alrészlet betűjele |  | 21 | VÁLT_ALR_JEL |  |  | betűjel | 2,0 kD |  | 1 |

| 2.3.5. | változott alrészlet művelési ága | BE02 | 22 | V_ALR_MŰVÁG |  |  | művelési ág | 1,5 kD |  | 1 |

| 2.3.6. | előzetes szabvány alatti kapcsolt alrészlet és megírása | BE03–04 | 23 | ELŐ_SZA_ALR | pontsor (0,5–0,5) | 0,3 | betűjel, műv. ág | 1,8 kD |  | 1 |

| 2.3.7. | előzetes minőségi osztály határa és megírása | BF02 | 24 | ELŐ_MIN_OSZT | szaggatott (3–1) | 0,3 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 2.3.8. | előzetes szabvány alatti minőségi osztály határa és megírása | BF02 | 25 | ELŐ_SZA_MINO | szaggatott (3–1) | 0,3 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 2.3.9. | záradékolás iktatószáma |  | 26 | ZÁRADÉK_ISZ |  |  | iktatószám | 2,5 Á |  | 1 |

| 2.4. Védett területek határai |

| 2.4.1. | természetvédelmi terület | HC04–05 | 27 | TERMÉSZETVÉD | szaggatott (6–3) | 0,18 | terület neve | 3,0 kÁ |  | 2 |

| 2.4.2. | bányaterület, geológiai feltárás területe | HC08, 11 | 28 | BÁNYATER | szaggatott (6–3) | 0,18 | terület neve | 3,0 kÁ |  | 2 |

| 2.4.3. | vízművek, források, fürdők védőterülete | HC12 | 29 | VÍZ_VÉDŐTER | szaggatott (6–3) | 0,18 | terület neve | 3,0 kÁ |  | 2 |

| 3. ÉPÜLETEK, ÉPÍTMÉNYEK |

| 3.1. Épületek |

| 3.1.1. | lakóépület | CA01 | 30 | LAKÓÉPÜLET | folytonos | 0,18 |  |  |  | 1 |

| 3.1.2. | gazdasági és melléképület >12 m 2 | CA05–06 | 31 | GAZD_ÉPÜLET | folytonos | 0,18 | funkció | 1,8 kD |  | 1 |

| 3.1.3. | középület, közintézmény | CA03 | 32 | KÖZÉPÜLET | folytonos | 0,18 | funkció | 1,8 kD |  | 1 |

| 3.1.4. | templom, kápolna, mauzóleum, imaház |  | 33 | TEMPLOM | folytonos | 0,18 | funkció | 1,8 kD |  | 1 |

| 3.1.5. | üzemi épület, építmény | CA04 | 34 | ÜZEMI_ÉPÜLET | folytonos | 0,18 | funkció | 1,8 kD |  | 1 |

| 3.1.6. | házszám |  | 35 | HÁZSZÁM |  |  | házszám | 2,0 kÁ |  | 1 |

| 3.1.7. | üdülőépület | CA02 | 87 | ÜDÜLŐÉPÜLET | folytonos | 0,18 |  |  |  | 1 |

| 3.1.8. | vegyes funkciójú épület | CA07 | 93 | VEGYES_ÉP | folytonos | 0,18 | funkció | 1,8 kD |  | 1 |

| 3.1.9. | rendezetlen funkciójú épület | CA08 | 94 | REND.LEN_ÉP | folytonos | 0,18 | funkció | 1,8 kD |  | 1 |

| 3.2. Épületek tartozékai |

| 3.2.1. | épület tartópillére (ábrázolandó) | CB02 | 84 | ÉP_PILLÉR | folytonos | 0,18 |  |  | JKDATC02–03 | 1 |

| 3.2.2. | épülethez tartozó lépcső, terasz, rámpa, lábazat | CB03, 05–06 | 36 | ÉPÜLET_TART | folytonos | 0,18 | ,,terasz”, ,,rámpa” | 1,5 kD |  | 1 |

| 3.2.3. | terepszintre levetített külső falsík, tető, föld feletti átjáró, épülethez csatlakozó lefedett terület | CB07 | 37 | VETÍTETT_SÍK | szaggatott (1,5–0,5) | 0,18 |  |  |  | 2(1) |

| 3.3. Toronyszerű építmények, emlékművek |

| 3.3.1. | kémény (épületen és épületen kívül) | CD01–02 | 38 | TORONY_ÉP | folytonos | 0,18 |  |  | JKDATC08–14 | 2(1) |

| 3.3.2. | kilátó | Kilátó (névvel) | 1,8 kD | JKDATC15 |

| 3.3.3. | torony (épületen és épületen kívül) | torony | 1,8 kD | JKDATC16–17 |

| 3.3.4. | szélmalom | CD04 | szélmalom | 1,8 kD |  |

| 3.3.5. | harangláb, kőkereszt, képoszlop | CD06–07 |  |  | JKDATC27–28 |

| 3.3.6. | szobor, emlékmű | ,,x” szobor, emlékmű | 1,8 kD | JKDATC06–07 |

| 3.4. Falak, támfalak, kerítések, földművek |

| 3.4.1. | szabadon álló fal, falazott kerítéslábazat a földrészlet határon | CC01–04 | 39 | FAL_KERÍTÉS | folytonos | 0,18 |  |  |  | 2(1) |

| 3.4.2. | támfal, támfal pillérrel | CC06 | 40 | TÁMFAL | folytonos | 0,18 |  |  |  | 2(1) |

| 3.4.3. | védtöltés koronavonala, töltésláb, földmunkával létesített egyéb tereptárgy | CC05 | 41 | TÖLTÉS | pontsor (0,5–0,5) | 0,18 | rendeltetés | 1,5 kD |  | 2(1) |

| 3.5. Romok |

| 3.5.1. | ábrázolandó műemlékrom | CE05–06 | 42 | ROM | pontsor (0,5–0,5) | 0,18 | ,,y” rom (neve) | 1,8 kD |  | 1 |

| 4. KÖZLEKEDÉS |

| 4.1. Utcák, közterek (belterületen) |

| 4.1.1. | út, utca, tér, közterület neve |  | 43 | UTCANÉV |  |  | ,,z” út, utca stb. | 3,0 kD |  | 1 |

| 4.1.2. | épületben vezető átjáró, passzázs, árkád | DB12–13 | 85 | PASSZ_ÁRKÁD | szaggatott (1,5–0,5) | 0,18 |  |  |  | 1 |

| 4.1.3. | lépcső közterületen | DB10 | 44 | LÉPCSŐ | folytonos | 0,18 | ,,v” lépcső | 1,5 kD |  | 2(1) |

| 4.1.4. | burkolat széle |  | 45 | BURKOLAT | folytonos | 0,18 | jb, burkolat | 1,8 kD |  | 2(1) |

| 4.1.5. | árok (nem alrészlet) | DB09 | 88 | ÁROK_BT | pontsor (0,5–0,5) | 0,18 | árok, á | 1,5 kD |  | 2(1) |

| 4.2. Közutak (külterületen) |

| 4.2.1. | I. rendű utak burkolat széle | DC01–03 | 46 | AUTÓÚT_SZÉLE | folytonos | 0,18 | útszám+közl. út | 2,0 kD | JKDATD01 | 2(1) |

| 4.2.2. | I. rendű út: padka, árok, töltéskorona széle | DC10, DG07–08 | 47 | AUTÓÚT_PADKA | pontsor (0,5–0,5) | 0,18 | árok, töltés | 1,8 kD |  | 2(1) |

| 4.2.3. | II. rendű utak burkolat széle | DC04 | 48 | MŰÚT_SZÉLE | folytonos | 0,18 | (útszám)+közl. út | 2,0 kD | JKDATD01 | 2(1) |

| 4.2.4. | II. rendű utak: padka, árok, töltéskorona széle |  | 49 | MŰÚT_PADKA | pontsor (0,5–0,5) | 0,18 | árok, töltés | 1,8 kD |  | 2(1) |

| 4.2.5. | mellékutak burkolat széle | DC05 | 50 | MELLÉKÚT | folytonos | 0,18 | közl. út | 2,0 kD |  | 2(1) |

| 4.2.6. | egyéb közlekedési utak (kerékpárút) | DC07–08 | 51 | EGYÉB_ÚT | folytonos | 0,18 | út, kerékpárút | 1,8 kD |  | 2(1) |

| 4.2.7. | talajút, dűlőút (nem alrészlet) | DC06 | 89 | DŰLŐÚT | pontsor (0,5–0,5) | 0,18 | út | 1,8 kD |  | 2(1) |

| 4.2.8. | árok (nem alrészlet) | DC11 | 90 | ÁROK_KT | pontsor (0,5–0,5) | 0,18 | árok, á | 1,5 kD |  | 2(1) |

| 4.3. Pontszerű tereptárgyak |

| 4.3.1. | autópályák (autóutak) segélykérő telefonja | DG02 | 47, 49 | rétegkód szerint |  |  | Ts. | 2,0 kD | JKDATD08 | 2(1) |

| 4.3.2. | kilométerkő, kilométertábla | DG07 | 47, 49, 52– 55, 58– 59 |  |  | ,,i” km | JKDATD09–10 |

| 4.3.3. | hektométerkő, hektométertábla | DG08 |  |  | ,,n” hm |  |

| 4.4. Vasutak, közúti villamospályák, HÉV |

| 4.4.1. | vasút (tengelyvonal) | DD01 | 52 | VASÚT | folytonos | 0,4 | vasút | 2,0 kD |  | 2(1) |

| 4.4.2. | villamosított vasút (tengelyvonal) | DD02 | vill. vasút |  | JKDATD02 |

| 4.4.3. | közúti villamos (tengelyvonal) | DD03 | 53 | VILLAMOS_HÉV | villamos | 1,8 kD |  | 2(1) |

| 4.4.4. | HÉV (tengelyvonal) | DD05 |  | HÉV |  |  |

| 4.4.5. | ipari, erdei vasút (tengelyvonal), kisnyomtávú | DD06 | 54 | IPARI_VASÚT | iparvasút, erdei vasút | 1,8 kD |  | 2(1) |

| 4.4.6. | sikló (tengelyvonal) | DD07 | 55 | EGYÉB_VASÚT | sikló | 1,5 kD |  | 2(1) |

| 4.4.7. | fogaskerekű (tengelyvonal) | DD08 | fogaskerekű |  |  |

| 4.5. Műtárgyak |

| 4.5.1. | híd | DF01 | 56 | HÍD | folytonos | 0,18 | a műtárgy neve | 3,0 kD |  | 1 |

| 4.5.2. | felüljáró (gyalogos, közúti) | DF02 | 57 | FELÜLJÁRÓ | szaggatott (1,5–0,5) | 0,18 | közl. út | 1,5 kD |  | 1 |

| 4.5.3. | alagút(torkolat) | DF05 | 91 | ALAGÚT | folytonos | 0,18 | a műtárgy neve | 1,5 kD |  | 1 |

| 5. VIZEK |

| 5.1. Medervonal |

| 5.1.1. | folyó, tó, csatorna stb. meder(part-)vonala | FA01–05 | 58 | MEDERVONAL | folytonos | 0,18 | ,,név” | 3,0 kD |  | 2(1) |

| 5.2. Műtárgyak |

| 5.2.1. | zsilip | FC03 | 59 | MŰTÁRGY_VÍZ | folytonos | 0,18 | zsilip, zs. | 1,8 kD | JKDATF02 | 2(1) |

| 5.2.2. | móló, partvédmű, sarkantyú | FC04 | móló, partv. |  | 2(1) |

| 5.2.3. | medence |  | medence |  | 2(1) |

| 5.2.4. | duzzasztógát | FC05 | duzzasztó (anyaga is) |  | 2(1) |

| 5.2.5. | víztorony | FC07 | 60 | VÍZTORONY | folytonos | 0,18 | víztorony | 1,8 kD | JKDATC15 | 2(1) |

| 5.2.6. | áteresz | DF03 | 80 | ÁTERESZ | pontsor (0,5–0,5) | 0,18 |  |  | JKDATD07 | 2(1) |

| 5.3. Pontszerű tereptárgyak |

| 5.3.1. | hidroglóbusz | FC07 | 60 | VÍZTORONY |  |  | hidroglóbusz | 1,8 kD | JKDATF10 | 2(1) |

| 5.3.2. | vízmérce | FC12 | 58 | MEDERVONAL |  |  |  |  | JKDATF03 | 2(1) |

| 5.3.3. | forrás, kút, szökőkút, tűzcsap stb. | FB05, FC09–10 | 61 | KÚT |  |  | forrás, kút, szökőkút | 1,8 kD | JKDATF01, 04–09 | 2(1) |

| 6. TÁVVEZETÉKEK, FÜGGŐPÁLYÁK |

| 6.1. Földfelszíni és felszín feletti távvezetékek |

| 6.1.1. | nagyfeszültségű elektromos vezeték | EA01 | 62 | ELEKT_TÁVVEZ | folytonos | 0,18 |  |  | JKDATE01–04 | 2 |

| 6.1.2. | drótkötélpálya | EA02 | 63 | DRÓTKÖTÉL | szaggatott (2–1) | 0,18 | drkp. | 1,8 kD | JKDATE05 | 2 |

| 6.1.3. | egyéb függőpálya | EA03 | 64 | EGYÉB_FÜGGŐP | szaggatott (2–1) | 0,18 | sífelvonó (stb.) | 2,0 kD |  | 2 |

| 6.1.4. | távhő, melegvíz | EA04 | 65 | TÁVHŐ | folytonos | 0,18 | Gő, M | 2,0 Fk kD |  | 2 |

| 6.1.5. | olajvezeték (tartóbakkal) | EA05 | 66 | OLAJ_FELSZÍN | folytonos | 0,18 | O | 2,0 Fk ND |  | 2 |

| 6.1.6. | gázvezeték (tartóbakkal) | EA06 | 67 | GÁZ_FELSZÍNI | folytonos | 0,18 | G | 2,0 Fk ND |  | 2 |

| 6.1.7. | egyéb felszíni és felszín feletti távvezeték |  | 68 | EGYÉB_FELSZ | folytonos | 0,18 | rendeltetés szerint | 1,8 kD |  | 2 |

| 6.2. Földfelszín alatti távvezetékek |

| 6.2.1. | olajvezeték, irányjelzővel, szaglócsővel |  | 69 | OLAJ_F_ALATT | szaggatott (10–2) | 0,18 | O | 2,0 Fk ND | JKDATE11 | 2 |

| 6.2.2. | gázvezeték, irányjelzővel, szaglócsővel |  | 70 | GÁZ_F_ALATTI | szaggatott (10–2) | 0,18 | G | 2,0 Fk ND | JKDATE11 | 2 |

| 6.2.3. | vízvezeték, irányjelző táblával | FB03 | 71 | VÍZVEZETÉK | szaggatott (10–2) | 0,18 | V | 2,0 Fk ND |  | 2 |

| 6.2.4. | egyéb vezeték, irányjelzővel, szaglócsővel |  | 72 | EGYÉB_F_ALA | szaggatott (10–2) | 0,18 | vezetékfajta | 2,0 Fk ND | JKDATE11 | 2 |

| 6.2.5. | távvezeték biztonsági övezete |  | 73 | BIZT_ÖV | szaggatott (6–3) | 0,18 | vezetékfajta | 1,5 kD |  | 2 |

| 7. EGYÉB TEREPTÁRGYAK |

| 7.1. Bányászat |

| 7.1.1. | függőleges akna | CD11 | 28 | BÁNYATER |  |  | akna (neve) | 1,8 kD | JKDATC23 | 2 |

| 7.1.2. | tárna, lejtős akna |  |  |  |  |  | tárna (neve) | 2,0 Fk ND | JKDATC24 | 2 |

| 7.1.3. | olajtermelő kút | EB02 | 66 | OLAJ_FELSZÍNI |  |  | O | JKDATE06 | 2 |

| 7.1.4. | gáztermelő kút | EB03 | 67 | GÁZ_FELSZÍNI |  |  | G | 2,0 Fk ND | 2 |

| 7.1.5. | olajtartály | EB04 | 66 | OLAJ_FELSZÍNI |  |  | O | 2,0 Fk ND |  | 2 |

| 7.1.6. | gáztartály | EB05 | 67 | GÁZ_FELSZÍNI |  |  | G | 2,0 Fk ND |  | 2 |

| 7.1.7. | egyéb üzemanyagtartály |  | 68 | EGYÉB_FELSZÍNI |  |  | Üa. | 2,0 Fk ND |  | 2 |

| 7.1.8. | üzemanyagtöltő állomás üzemi területe | DB21 | 74 | ÜA_KÚT | szaggatott (6–3) | 0,18 | Üa. állomás | 1,5 kD | JKDATD06 | 2 |

| 7.2. Pontszerű és egyéb tereptárgyak |

| 7.2.1. | szélmotor | CD03 | 75 | EGYEBEK |  |  | szélmotor | 1,8 kD | JKDATC22 | 2 |

| 7.2.2. | temetőn kívüli tömegsír, sír, kripta | CD09 |  |  | sír | 1,8 kD |  | 2 |

| 7.2.3. | dögkút | CD10 |  |  | dögkút, dögk. | 1,8 kD | JKDATC26 | 2 |

| 7.2.4. | egyedül álló fa (természetvédelmi emlék, határdombon lévő fa, képes fa stb.) | CD08 | 27 | TERMÉSZETVÉD |  |  |  |  | JKDATC20–21 | 2 |

| 7.2.5. | védett fasor | szaggatott (6–3) | 0,18 | védett fasor | 1,8 kD |  | 2 |

| 8. EGYÉB ADATOK |

| 8.1. | teljes helyrajzi szám a területszámításhoz |  | 78 | TELJES_HRSZ |  |  | teljes hrsz. | 1,5 D |  | 1 |

| 8.2. | töredék helyrajzi szám a kirajzoláshoz |  | 92 | TÖREDÉK_HRSZ |  |  | töredék hrsz. | 2,0 D |  | 1 |

| 8.3. | kapcsolójel |  | 79 | KAPCS_JEL |  |  |  |  | JKDATB04 | 1 |

| 8.4. | természetbeni határ, jogi állapottal nem egyező |  | 81 | TERM_HATÁR | szaggatott (2–1) | 0,18 |  |  |  | 1 |

| 8.5. | tervezett jogi határ, természetben nem található |  | 82 | TERV_HATÁR | szaggatott (4–1) | 0,18 |  |  |  | 1 |

| 8.6. | közterületről nyíló pince | CB01 | 83 | KT_PINCE | folytonos | 0,18 |  |  |  | 1 |

| 8.7. | dűlőnév, földrajzi név | BB04 | 86 | DŰLŐNÉV |  |  | dűlőnév, földrajzi név | 3,0 kD |  | 1 |

| 9. AZ EGYSÉGES ORSZÁGOS TÉRKÉPRENDSZER (EOTR) TÉRKÉPSZELVÉNYEINEK KERETVONALAI |

| 9.1. | 1:1000 méretarányú alaptérkép |  | 101 | 1000_MA | folytonos | 0,18 | szelvény- feliratok |  |  | 1 |

| 9.2. | 1:2000 méretarányú alaptérkép |  | 102 | 2000_MA | folytonos | 0,18 |  |  | 1 |

| 9.3. | 1:4000 méretarányú alaptérkép |  | 103 | 4000_MA | folytonos | 0,18 |  |  | 1 |

| 9.4. | 1:10000 méretarányú átnézeti térkép kirajzolásához |  | 104 | 10000_MA | folytonos | 0,18 |  |  | 1 |

| 10. VÁLTOZÁSI VÁZRAJZ KÉSZÍTÉSE SORÁN KEZELT MEGLÉVŐ, ÚJ ÉS MEGSZŰNŐ RÉGI ADATOK |

| 10.1. Változás előtti – hiteles – adatok |

| 10.1.1. | földrészlet határvonala | BC01–08; BD01–02 | 110 | VE_FRL_HAT | folytonos | 0,18 |  |  | JKDATA29–30 | 1 |

| 10.1.2. | helyrajzi szám (jogerős) |  | 111 | VE_HRSZ |  |  | helyrajzi szám | 2,0 D |  | 1 |

| 10.1.3. | alrészlet határvonala | BE01 | 112 | VE_ALR_HAT | pontsor (0,5–0,5) | 0,18 |  |  |  | 1 |

| 10.1.4. | alrészlet betűjele |  | 113 | VE_ALR_JEL |  |  | betűjel | 2,0 kD |  | 1 |

| 10.1.5. | alrészlet művelési ága | BE02 | 114 | VE_ALR_MŰVÁG |  |  | művelési ág | 1,5 kD |  | 1 |

| 10.1.6. | minőségi osztály határvonala és megírása | BF01 | 115 | VE_MIN_OSZT | szaggatott (3–1) | 0,18 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 10.1.7. | szabvány alatti kapcsolt alrészlet és megírása | BE03–04 | 116 | VE_SZA_ALR | pontsor (0,5–0,5) | 0,18 | művelési ág | 1,5 kD |  | 1 |

| 10.1.8. | szabvány alatti minőségi osztály és megírása | BF02 | 117 | VE_SZA_MINO | szaggatott (3–1) | 0,18 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 10.2. Változás utáni – előzetes – adatok |

| 10.2.1. | földrészlet előzetes határa | BC01–08; BD01–02 | 118 | VU_FRL_HAT | folytonos | 0,5 |  |  | JKDATA29–30 | 1 |

| 10.2.2. | előzetes helyrajzi szám |  | 119 | VU_HRSZ |  |  | helyrajzi szám | 2,0 D |  | 1 |

| 10.2.3. | változott alrészlet határvonala | BE01 | 120 | VU_ALR_HAT | pontsor (0,5–0,5) | 0,3 |  |  |  | 1 |

| 10.2.4. | változott alrészlet betűjel |  | 121 | VU_ALR_JEL |  |  | betűjel | 2,0 kD |  | 1 |

| 10.2.5. | változott alrészlet művelési ága | BE02 | 122 | VU_ALR_MŰVÁG |  |  | művelési ág | 1,5 kD |  | 1 |

| 10.2.6. | előzetes szabvány alatti kapcsolt alrészlet és megírása | BE03–04 | 123 | VU_SZA_ALR | pontsor (0,5–0,5) | 0,3 | betűjel, műv. ág | 1,8 kD |  | 1 |

| 10.2.7. | előzetes minőségi osztály határa és megírás | BF02 | 124 | VU_MIN_OSZT | szaggatott (3–1) | 0,3 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 10.2.8. | előzetes szabvány alatti minőségi osztály határa és megírása | BF02 | 125 | VU_SZA_MINO | szaggatott (3–1) | 0,3 | műv. ág, min. oszt. | 1,5 kD |  | 1 |

| 10.3. Új épületek, építmények |

| 10.3.1. | új lakóház | CA01 | 130 | ÚJ_LAKÓÉP | folytonos | 0,3 |  |  |  | 1 |

| 10.3.2. | új gazdasági és melléképület >12 m2 | CA05–06 | 131 | ÚJ_GAZD_ÉP | folytonos | 0,3 | funkció | 1,8 kD |  | 1 |

| 10.3.3. | új középület, közintézmény | CA03 | 132 | ÚJ_KÖZÉPÜLET | folytonos | 0,3 | funkció | 1,8 kD |  | 1 |

| 10.3.4. | új templom, kápolna, mauzóleum, imaház |  | 133 | ÚJ_TEMPLOM | folytonos | 0,3 | funkció | 1,8 kD |  | 1 |

| 10.3.5. | új üzemi épület, építmény | CA04 | 134 | ÚJ_ÜZEMI_ÉP | folytonos | 0,3 | funkció | 1,8 kD |  | 1 |

| 10.3.6. | új házszám |  | 135 | ÚJ_HÁZSZÁM |  |  | házszám | 2,0 kÁ |  | 1 |

| 10.3.7. | új üdülőépület | CA02 | 136 | ÚJ_ÜDÜLŐÉP | folytonos | 0,3 |  |  |  | 1 |

| 10.3.8. | új vegyes funkciójú épület | CA07 | 137 | ÚJ_VEGYES_É | folytonos | 0,3 | funkció | 1,8 kD |  | 1 |

| 10.3.9. | új rendezetlen fukciójú épület | CA08 | 138 | ÚJ_RLEN_ÉP | folytonos | 0,3 | funkció | 1,8 kD |  | 1 |

| 10.4. A változás során megszűnő határvonalak |

| 10.4.1. | megszűnő földrészlet határvonal | BC01–08; BD01–02 | 210 | MSZ_FRL_HAT | folytonos | 0,18 |  |  | megszüntető jel | 1 |

| 10.4.2. | megszűnő helyrajzi szám |  | 211 | MSZ_HRSZ |  |  | helyrajzi szám | 2,0 D | áthúzás | 1 |

| 10.4.3. | megszűnő alrészlet határ | BE01 | 212 | MSZ_ALR_HAT | pontsor (0,5–0,5) | 0,18 |  |  | megszüntető jel | 1 |

| 10.4.4. | megszűnő alrészlet betűjel |  | 213 | MSZ_ALR_JEL |  |  | betűjel | 2,0 kD | áthúzás | 1 |

| 10.4.5. | megszűnő alrészlet művelési ág | BE02 | 214 | MSZ_ALR_MŰÁ |  |  | művelési ág | 1,5 kD | megsz. jel és áthúz. | 1 |

| 10.4.6. | megszűnő sza. alatti kapcsolt alrészlet és megírása | BF01 | 215 | MSZ_SZA_ALR | szaggatott (3–1) | 0,18 | műv. ág, min. oszt. | 1,5 kD | megsz. jel és áthúz. | 1 |

| 10.4.7. | megszűnő minőségi osztály és megírása | BE03–04 | 216 | MSZ_MINO | pontsor (0,5–0,5) | 0,18 | művelési ág | 1,5 kD | megsz. jel és áthúz. | 1 |

| 10.4.8. | megszűnő sza. alatti minőségi osztály és megírása | BF02 | 217 | MSZ_SZA_MINO | szaggatott (3–1) | 0,18 | műv. ág, min. oszt. | 1,5 kD | megsz. jel és áthúz. | 1 |

| 10.5. A változás során megszűnő épületek, építmények |

| 10.5.1. | megszűnő lakóépület | CA01 | 230 | MSZ_LAKÓÉP | folytonos | 0,18 |  |  | megszüntető jel | 1 |

| 10.5.2. | megszűnő gazdasági- és melléképület >12 m2 | CA05–06 | 231 | MSZ_GAZD_ÉP | folytonos | 0,18 | funkció | 1,8 kD | megsz. jel és áthúz. | 1 |

| 10.5.3. | megszűnő középület, közintézmény | CA03 | 232 | MSZ_KÖZÉP | folytonos | 0,18 | funkció | 1,8 kD | megsz. jel és áthúz. | 1 |

| 10.5.4. | megszűnő templom, kápolna, mauzóleum, imaház |  | 233 | MSZ_TEMPL | folytonos | 0,18 | funkció | 1,8 kD | megsz. jel és áthúz. | 1 |

| 10.5.5. | megszűnő üzemi épület, építmény | CA04 | 234 | MSZ_ÜZ_ÉP | folytonos | 0,18 | funkció | 1,8 kD | megsz. jel és áthúz. | 1 |

| 10.5.6. | megszűnő házszám |  | 235 | MSZ_HÁZSZÁM |  |  | házszám | 2,0 kÁ | áthúzás | 1 |

| 10.5.7. | megszűnő üdülőépület | CA02 | 236 | MSZ_ÜDÜLŐÉP | folytonos | 0,18 |  |  | megszüntető jel | 1 |

| 10.5.8. | megszűnő vegyes funkciójú épület | CA07 | 237 | MSZ_VE_ÉP | folytonos | 0,18 | funkció | 1,8 kD | megsz. jel és áthúz. |  |

| 10.5.9. | megszűnő rendezetlen funkciójú épület | CA08 | 238 | MSZ_RL_ÉP | folytonos | 0,18 | funkció | 1,8 kD | megsz. jel és áthúz. |  |

| 10.5.10. | a változás során megszűnt adatok jelölése (áthúzás) |  | 239 | ÁTHÚZÁS | folytonos | 0,18 |  |  | áthúzás | 1 |

| 10.5.11. | megszüntető jel |  | 240 | MSZ_JEL | folyt. párh. vonalka | 0,18 |  |  |  |  |

| 11. A MÉRÉSI VÁZLAT ADATAI |

| 11.1. | a változási vázrajzon ábrázolt főbb méretek, a kitűzési adatok nélkül |  | 241 | VÁZR_MÉRET |  |  | méretek | 1,5 kD |  | 1 |

| 11.2. | az új részletpontok pontszámai |  | 242 | R_PONTSZÁM |  |  | pontszám | 1,5 kÁ |  | 1 |

| 11.3. | az ingatlan-nyilvántartási térkép méretei |  | 243 | TÉRK_MÉRET |  |  | méretek | 1,5 kD |  | 1 |

| 11.4. | az eredeti – korábbi – mérési vázlat adatai |  | 244 | ER_MÉRT_ADAT |  |  | méretek | 1,5 kD |  | 1 |

| 11.5. | a helyszíni mérés adatai |  | 245 | MÉRT_ADAT |  |  | méretek | 1,5 kD |  | 1 |

| 11.6. | kitűzési méretek |  | 246 | KIT_MÉRET |  |  | méretek | 1,5 kD |  | 1 |

| 11.7. | szolgalmi, kezelői, használati jog stb. határvonala |  | 247 | SZOLG_JOG_H | szaggatott (3–1) | 0,18 |  |  |  | 1 |

3. számú függelék

A MEGYEI ÉS KÖRZETI FÖLDHIVATALOK SZÁMJEL RENDSZERE

1. A számjel rendszer

1.1. Megyei, körzeti földhivatal és földhivatali kirendeltség

A megyék azonosító számát a KSH rendszere alapján kell meghatározni. A megyei azonosítóját ki kell egészíteni a körzeti földhivatal, valamint a földhivatali kirendeltség számjelével. A megyei földhivatal azonosítója mindig két karakterből áll (a KSH megye kódja), míg a körzeti földhivatal és a földhivatali kirendeltség számjele három karaktert tartalmaz, az alábbi értelmezés szerint:

xxxxx

1 2

1 Az első két karakter a megye kódja, amely mindig azonos a megyei földhivatal kódjával.

2 A körzeti földhivatal sorszámát a 3. és 4. karakter mutatja. Az ötödik karakter az adott körzeti földhivatal kirendeltségére utal.

2. A megyei és körzeti földhivatalok, valamint a földhivatali kirendeltségek számjelei

01 FŐVÁROSI Földhivatal

02 BARANYA Megyei Földhivatal

02010 KOMLÓ Körzeti Földhivatal

02020 MOHÁCS Körzeti Földhivatal

02030 PÉCS Körzeti Földhivatal

02031 Megyei jogú város PÉCS

02040 SIKLÓS Körzeti Földhivatal

02050 SZIGETVÁR Körzeti Földhivatal

03 BÁCS-KISKUN Megyei Földhivatal

03010 BAJA Körzeti Földhivatal

3011 BÁCSALMÁS Földhivatali Kirendeltség

03020 KALOCSA Körzeti Földhivatal

03030 KECSKEMÉT Körzeti Földhivatal

03040 KISKŐRÖS Körzeti Földhivatal

03050 KISKUNFÉLEGYHÁZA Körzeti Földhivatal

03060 KISKUNHALAS Körzeti Földhivatal

3061 KUNSZENTMIKLÓS Földhivatali Kirendeltség

04 BÉKÉS Megyei Földhivatal

04010 BÉKÉS Körzeti Földhivatal

04020 BÉKÉSCSABA Körzeti Földhivatal

4021 GYOMAENDRŐD Földhivatali Kirendeltség

04030 GYULA Körzeti Földhivatal

04040 MEZŐKOVÁCSHÁZA Körzeti Földhivatal

04050 OROSHÁZA Körzeti Földhivatal

04060 SZARVAS Körzeti Földhivatal

04070 SZEGHALOM Körzeti Földhivatal

05 BORSOD-ABAÚJ-ZEMPLÉN Megyei Földhivatal

05010 EDELÉNY Körzeti Földhivatal

05020 ENCS Körzeti Földhivatal

05030 MEZŐKÖVESD Körzeti Földhivatal

05040 MISKOLC Körzeti Földhivatal

5041 Megyei jogú város MISKOLC

05050 ÓZD Körzeti Földhivatal

05060 SÁTORALJAÚJHELY Körzeti Földhivatal

05070 SZERENCS Körzeti Földhivatal

05080 TISZAÚJVÁROS Körzeti Földhivatal

06 CSONGRÁD Megyei Földhivatal

06010 HÓDMEZŐVÁSÁRHELY Körzeti Földhivatal

06020 MAKÓ Körzeti Földhivatal

06030 SZEGED Körzeti Földhivatal

6031 Megyei jogú város SZEGED

06040 SZENTES Körzeti Földhivatal

07 FEJÉR Megyei Földhivatal

07010 BICSKE Körzeti Földhivatal

07020 DUNAÚJVÁROS Körzeti Földhivatal

07030 MÓR Körzeti Földhivatal

07040 SÁRBOGÁRD Körzeti Földhivatal

07050 SZÉKESFEHÉRVÁR Körzeti Földhivatal

08 GYŐR-MOSON-SOPRON Megyei Földhivatal

08010 CSORNA Körzeti Földhivatal

08020 GYŐR Körzeti Földhivatal

8021 Megyei jogú város GYŐR

08030 KAPUVÁR Körzeti Földhivatal

08040 MOSONMAGYARÓVÁR Körzeti Földhivatal

08050 SOPRON Körzeti Földhivatal

09 HAJDÚ-BIHAR Megyei Földhivatal

09010 BERETTYÓÚJFALU Körzeti Földhivatal

09020 DEBRECEN Körzeti Földhivatal

9021 Megyei jogú város DEBRECEN

9022 HAJDÚBÖSZÖRMÉNY Földhivatali Kirendeltség

09030 HAJDÚSZOBOSZLÓ Körzeti Földhivatal

09040 PÜSPÖKLADÁNY Körzeti Földhivatal

10 HEVES Megyei Földhivatal

10010 EGER Körzeti Földhivatal

10020 FÜZESABONY Körzeti Földhivatal

10030 GYÖNGYÖS Körzeti Földhivatal

10040 HATVAN Körzeti Földhivatal

10050 HEVES Körzeti Földhivatal

11 KOMÁROM-ESZTERGOM Megyei Földhivatal

11010 DOROG Körzeti Földhivatal

11011 ESZTERGOM Földhivatali Kirendeltség

11020 KOMÁROM Körzeti Földhivatal

11030 TATA Körzeti Földhivatal

11040 TATABÁNYA Körzeti Földhivatal

12 NÓGRÁD Megyei Földhivatal

12010 BALASSAGYARMAT Körzeti Földhivatal

12020 PÁSZTÓ Körzeti Földhivatal

12030 RÉTSÁG Körzeti Földhivatal

12040 SALGÓTARJÁN Körzeti Földhivatal

13 PEST Megyei Földhivatal

13010 BUDAKÖRNYÉKI Körzeti Földhivatal

13011 ÉRD Földhivatali Kirendeltség

13020 CEGLÉD Körzeti Földhivatal

13021 NAGYKŐRÖS Földhivatali Kirendeltség

13030 DABAS Körzeti Földhivatal

13040 GÖDÖLLŐ Körzeti Földhivatal

13050 MONOR Körzeti Földhivatal

13060 NAGYKÁTA Körzeti Földhivatal

13070 RÁCKEVE Körzeti Földhivatal

13080 SZENTENDRE Körzeti Földhivatal

13090 VÁC Körzeti Földhivatal

13091 DUNAKESZI Földhivatali Kirendeltség

14 SOMOGY Megyei Földhivatal

14010 BALATONBOGLÁR Körzeti Földhivatal

14020 BARCS Körzeti Földhivatal

14030 KAPOSVÁR Körzeti Földhivatal

14040 MARCALI Körzeti Földhivatal

14050 NAGYATÁD Körzeti Földhivatal

14060 SIÓFOK Körzeti Földhivatal

15 SZABOLCS-SZATMÁR-BEREG Megyei Földhivatal

15010 FEHÉRGYARMAT Körzeti Földhivatal

15020 KISVÁRDA Körzeti Földhivatal

15030 MÁTÉSZALKA Körzeti Földhivatal

15040 NYÍRBÁTOR Körzeti Földhivatal

15050 NYÍREGYHÁZA Körzeti Földhivatal

15060 VÁSÁROSNAMÉNY Körzeti Földhivatal

16 JÁSZ-NAGYKUN-SZOLNOK Megyei Földhivatal

16010 JÁSZBERÉNY Körzeti Földhivatal

16020 KUNSZENTMÁRTON Körzeti Földhivatal

16030 SZOLNOK Körzeti Földhivatal

16031 MEZŐTÚR Földhivatali Kirendeltség

16040 TÖRÖKSZENTMIKLÓS Körzeti Földhivatal

16041 KARCAG Földhivatali Kirendeltség

16050 TISZAFÜRED Körzeti Földhivatal

17 TOLNA Megyei Földhivatal

17010 BONYHÁD Körzeti Földhivatal

17020 DOMBÓVÁR Körzeti Földhivatal

17030 PAKS Körzeti Földhivatal

17040 SZEKSZÁRD Körzeti Földhivatal

17050 TAMÁSI Körzeti Földhivatal

18 VAS Megyei Földhivatal

18010 CELLDÖMÖLK Körzeti Földhivatal

18020 KÖRMEND Körzeti Földhivatal

18030 SÁRVÁR Körzeti Földhivatal

18040 SZOMBATHELY Körzeti Földhivatal

19 VESZPRÉM Megyei Földhivatal

19010 AJKA Körzeti Földhivatal

19020 BALATONFÜRED Körzeti Földhivatal

19030 PÁPA Körzeti Földhivatal

19040 TAPOLCA Körzeti Földhivatal

19050 VESZPRÉM Körzeti Földhivatal

19051 ZIRC Földhivatali Kirendeltség

20 ZALA Megyei Földhivatal

20010 KESZTHELY Körzeti Földhivatal

20011 ZALASZENTGRÓT Földhivatali Kirendeltség

20020 LENTI Körzeti Földhivatal

20030 LETENYE Körzeti Földhivatal

20040 NAGYKANIZSA Körzeti Földhivatal

20050 ZALAEGERSZEG Körzeti Földhivatal

[^3]: A melléklet 1.3. pontja a 98/2002. (X. 17.) FVM rendelet 2. § (1) bekezdésével megállapított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
[^4]: Lásd az 1998: XXXVI. törvény 2. §-a (1) bekezdésének d) pontját.
[^5]: A melléklet 1.6. pontja a 98/2002. (X. 17.) FVM rendelet 2. § (2) bekezdése szerint módosított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
[^6]: A melléklet 2.3. pontja a 98/2002. (X. 17.) FVM rendelet 2. § (3) és (4) bekezdése szerint módosított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
[^7]: A melléklet 3.1. pontja a 98/2002. (X. 17.) FVM rendelet 2. § (5) bekezdése szerint módosított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
[^8]: A melléklet 6.4. pontjának (5) bekezdése a 98/2002. (X. 17.) FVM rendelet 2. § (6) bekezdése szerint módosított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
[^9]: A melléklet 1. függeléke a 98/2002. (X. 17.) FVM rendelet 2. § (7) bekezdésével megállapított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
[^10]: A melléklet 2. függeléke a 98/2002. (X. 17.) FVM rendelet 2. § (7) bekezdésével megállapított szöveg, e módosító rendelet 3. §-a alapján a rendelkezéseit a folyamatban lévő földmérési munkáknál is alkalmazni kell.
