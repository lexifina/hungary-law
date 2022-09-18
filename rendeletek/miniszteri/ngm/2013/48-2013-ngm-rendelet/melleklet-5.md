## 6K04021_17

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | max 5 hosszú numerikus |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat nyitásának kiadásának pontos ideje az AEE órája szerint | szabványos dátum és iőő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 db számjegy sztring formátumban |

| 5. | EIT | Egyéb dokumentum típusa | 20 hosszú szöveg |

| 6. | EIL | Egyéb dokumentum típus leírás | 20 hosszú szöveg |

| 7. | EDA | Egyéb dokumentumon szereplő adatok | lista, max 100 |

| 7.1 | > ENM | Egyéb dokumentumon szereplő adat megnevezése | 20 karakteres szöveges |

| 7.2 | > EVL | Egyéb dokumentumon szereplő adat értéke | 200 karakteres szöveges |

| 8. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 9. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 10. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 11. | HSH | Ellenőrző kód | 64 HEXA karakter |

## Bizonylat-összesítő nyomtatása esetén a naplóállományban a dokumentum kivonatát kell az Egyéb dokumentum (EDN) típusú naplósorban rögzíteni, melynek tartalma a dokumentum megnevezése, valamint a dokumentumon szereplő bizonylatok összesített darabszáma bizonylattípusonként, a mező megnevezésében a bizonylattípus nevét, az adattartalmában a darabszámot feltüntetve. Csak azokat a bizonylattípusokat kell feltüntetni, melyek szerepeltek a bizonylat-összesítő dokumentumon.

5. melléklet a 48/2013. (XI. 15.) NGM rendelethez[^192]

Az Adóügyi Ellenőrző Egység (AEE) és a NAV szerverei közötti kommunikáció protokolljára vonatkozó előírások

1. Az AEE és a NAV szerver (ezen mellékletben a továbbiakban: NAV) üzenetei az UTF-8-as kódlap szerint kódolt karaktersorozatok. Jelen melléklet tekintetében XXXXXXXXX az adatszolgáltatással érintett pénztárgép AP számát, HHHHHHHHHH a szerver által előállított, 10 hexadecimális számjegyből álló munkamenet azonosító kódot jelöli. Amennyiben az AEE válaszüzeneteiben a HHHHHHHHHH igazoló kód szerepel, úgy minden esetben a megelőző NAV üzenetben szereplő kódot kell alkalmazni.

2. Az SMS üzenetek küldésére, vagy a közvetlen IP kommunikáció biztosítására a mobil szolgáltatóknak HTTPS alapú webszolgáltatást kell biztosítaniuk a NAV számára. A szolgáltató kizárólag a NAV szerverétől fogadhat el üzenetküldési parancsot. Az üzenetek címzése az IMSI szám vagy IP cím alapján történik, az illesztőfelület jellege szerint.

3. Az AEE-nek képesnek kell lennie tárolni a NAV SSL tanúsítványának publikus kulcsát, kapcsolatot csak ezzel a tanúsítvánnyal ellenőrzötten építhet ki. A mobilhálózatra az üzenetek HTTPS/POST metódussal küldi a NAV.

4. Az AEE-nek képesnek kell lennie a NAV-val való kapcsolat felvételre, üzenetküldésre, üzenet fogadására, illetve a NAV-tól érkező utasítások végrehajtására az e mellékletben foglaltak szerint.

5. Az ebben a mellékletben jelzett AEE által elküldött fájl nevének formátuma „fájlnév~HHHHHHHHHH”, ahol fájlnév az éppen küldött naplófájl neve a 4. mellékletben előírt felépítés szerinti. A beküldés POST metódussal és multipart/form-data adatkódolással, minden küldött fájl esetében a továbbítás binary kódolással történik. A naplófájlokat elektronikusan aláírva, PKCS#7 formátumban, az elektronikus tanúsítvány csatolása nélkül, bináris adatként kell küldeni a NAV részére.

6. Az AEE-nek be kell jegyeznie a legutóbb megnyitott szöveges állományba a fogadott és a küldött üzenetek tartalmát. Ez alól kivétel az elküldött naplófájlok, illetve fogadott tanúsítványok, firmware szeletek tartalma, ami helyett a naplófájl nevét, illetve a (cert) vagy (frw)megjelölést kell naplózni.

7. Az AEE-nek bontania kell az SSL kapcsolatot, amennyiben legalább 1 percig semmiféle kommunikáció sem történik a NAV-val.

8. Az AEE által kezdeményezett kapcsolatfelvétel sikertelensége esetén az AEE a kommunikációt legkorábban az előző kommunikációt követő egy perc múlva ismételheti meg maximálisan két alkalommal. Amennyiben ezen kísérletek sikertelenek maradnak, akkor csak a korábbi CONSET üzenet DTNEXT paraméterében meghatározott időtartam elteltét követően, CONSET üzenet hiányában 30 perc múlva kísérelheti meg újra az AEE a kapcsolatfelvételt a NAV szerverrel.

9. Folyamatban lévő kommunikáció esetén, ha az külön szabályozásra nem kerül, a kommunikáció sikertelensége vagy az AEE által a NAV szerver felé küldött üzenetre vonatkozó jelen mellékletben meghatározott NAV válasz hiányában az AEE minden üzenetet legfeljebb három alkalommal küldhet el a NAV-nak. A NAV szerver maximális válaszideje elküldéstől számítva 60 másodperc, az AEE ennek leteltét követően tekintheti úgy, hogy a NAV szerver nem válaszolt. Az AEE a kommunikációt legkorábban az előző kommunikációt követő három perc múlva ismételheti meg. Sikertelen kommunikáció esetén 10 és 30 perc közötti véletlenszerűen megválasztott szünet megtartása után az AEE újabb egy kísérletet tehet az üzenet elküldésére. Amennyiben az is sikertelen, úgy az adott hexadecimális kóddal azonosított kommunikációt sikertelennek kell tekinteni és az AEE csak a korábbi CONSET üzenet DTNEXT paraméterében meghatározott időtartam elteltét követően, CONSET üzenet hiányában 30 perc múlva kísérelheti meg újra a kapcsolatfelvételt a NAV szerverrel.

I. Az AEE által küldött üzenetek

## I/1. Normál bejelentkezés

## Az AEE a pénztárgép üzembe helyezett állapotában rendszeresen normál bejelentkezést hajt végre a NAV szerveréhez. A normál bejelentkezést haladéktalanul végre kell hajtani, ha a következő események közül legalább egy bekövetkezik:

a) A pénztárgépet bekapcsolják.

b) A pénztárgépen adóügyi napot nyitnak, az adott naptári napon elsőként.

c) A legutóbbi normál bejelentkezés óta eltelik a NAV legutóbbi CONSET üzenetében megjelölt időtartam, ilyen üzenet hiányában 30 perc.

Az AEE normál bejelentkezéskor titkosított (SSL) csatornát épít fel a NAV szerverrel való kommunikációra és azon a

„TRMRDY~XXXXXXXXX~S~N~T” üzenetet küldi el, ahol

S – az AEE éppen nyitott szöveges állomány sorszáma,

N – az AEE éppen nyitott szöveges állományában aktuálisan levő bejegyzések száma,

T – az AEE által utoljára nyitott szöveges fájl megnyitása óta eltelt üzemidő percben.

I/2. Elsőbbségi bejelentkezés

Az AEE a normál bejelentkezések ciklusától függetlenül, annak ütemezését nem módosítva elsőbbségi bejelentkezést hajt végre, ha az e pontban felsorolt események vagy állapot bármelyike bekövetkezik vagy előáll. Az AEE elsőbbségi bejelentkezéskor titkosított (SSL) csatornát épít fel a NAV szerverrel való kommunikációra és azon a

„PRIOR~YY~XXXXXXXXX~S~N~T” üzenetet küldi el, ahol

YY – az elsőbbségi adatszolgáltatás jelzését kiváltó ok kódja,

S – az AEE éppen nyitott szöveges állomány sorszáma,

N – az AEE éppen nyitott szöveges állományában aktuálisan levő bejegyzések száma,

T – az AEE által utoljára nyitott szöveges fájl megnyitása óta eltelt üzemidő percben.

Az elsőbbségi adatszolgáltatás jelzését kiváltó ok kódja:

a) YY=02 – abban az esetben, ha az AEE külső áramellátása megszűnik

b) YY=03 – a pénztárgép blokkolt állapotba hozza magát, ide nem értve a NAV üzenete által történő blokkolást

c) YY=04 – a naplófájlba bejegyzésre került az alábbi események egyike:

– pénztárgép szüneteltetésének kezdete

– pénztárgép szüneteltetésének vége

– pénztárgép átadása szerviznek

– pénztárgép visszavétele szerviztől

– éves felülvizsgálat elvégzése

d) YY=05 – a pénztárgép jelzi, hogy mivel nincs külső áramellátása, nincs a pénztárgépen nyitott adóügyi nap, a legutóbbi napzárásra vonatkozó bejegyzést tartalmazó naplóállomány sikeres fogadását a NAV visszaigazolta, ezért az AEE ezen állapot fennállásáig mellőzni fogja a rendszeres bejelentkezést,

e) YY=06 – a hordozható pénztárgép jelzi, hogy mivel nincs külső áramellátása, a legutóbbi lezárt naplóállomány sikeres fogadását a NAV visszaigazolta, ezért az AEE ezen állapot fennállásáig mellőzni fogja a rendszeres bejelentkezést

f) YY=07 – a pénztárgép azonnali bejelentkezésre vonatkozó felszólítást kapott.

g) YY=08 – az AEE saját áramforrásról üzemel, és annak töltöttsége a kritikus szint (10%) alá csökkent.

I/3. A NAV szerver által kijelölt feladat elvégzéséről szóló visszaigazolás

## A NAV szerver e mellékletben részletezett utasításainak végrehajtásáról az e mellékletben részletezett forgatókönyvek szerint az AEE az

## „ANS~XXXXXXXXX~YY~HHHHHHHHHH” üzenetet küldi, ahol

## YY – a NAV legutóbbi üzenetében foglaltakra vonatkozó visszajelzés kódja

## Az YY lehetséges értékei:

1. YY=01 – blokkolás utasítás végrehajtva,

2. YY=02 – blokkolás feloldás utasítás végrehajtva,

3. YY=03 – Áfa gyűjtő átállítás utasítás fogadva,

4. YY=04 – Áfa gyűjtő átállítás utasítás végrehajtva,

5. YY=05 – szoftverfrissítésre kész,

6. YY=06 – szoftverfrissítés letöltve,

7. YY=07 – szoftverfrissítés végrehajtva,

8. YY=08 – adózói adat frissítési utasítás fogadva,

9. YY=09 – SSL tanúsítvány letöltve

10. YY=10 – kapcsolat felvételi gyakoriság beállítva

11. YY=11 – az euró átálláshoz kapcsolódó dátumok fogadása sikeres

12. YY=12 – az átszemélyesítés sikeres

13. YY=14 – maximális naplóállomány méret beállítva

14. YY=15 – átszemélyesítés adózói adatok igénylése

15. YY=17 – nem küldhető több lezárt naplóállomány

16. YY=18 – adózói adatok frissítése megtörtént

17. YY=20 – Euró átállás megtörtént

18. YY=22 – Üzemeltetés szünetel

19. YY=31 – Blokkolás végrehajtása sikertelen

20. YY=32 – Blokkolás feloldása sikertelen

21. YY=33 – adózói adatok frissítése sikertelen

22. YY=34 – adózói adatok fogadása sikertelen

23. YY=35 – ÁFA tábla frissítése sikertelen

24. YY=36 – az üzenet értelmezhetetlen

25. YY=37 – naplófájl küldése ötszöri próbálkozás után is sikertelen

26. YY=38 – kapcsolat felvételi gyakoriság beállítás végrehajtása sikertelen

27. YY=39 – euró átálláshoz kapcsolódó dátumok fogadása sikertelen

28. YY=40 – az átszemélyesítés sikertelen

29. YY=41 – UPDCLR utasítás végrehajtva

30. YY=42 – UPDCLR utasítás végrehajtása sikertelen

31. YY=43 – tanúsítvány fogadása sikertelen

32. YY=44 – maximális naplóállomány méret beállítása sikertelen

33. YY=45 – nyomtatandó üzenet vétele sikeres

34. YY=46 – nyomtatandó üzenet vétele sikertelen

35. YY=47 – korábbi üzemeltető naplóállományainak törlése megtörtént

36. YY=48 – korábbi üzemeltető naplóállományainak törlése sikertelen

37. YY=49 – euró átállás végrehajtása sikertelen

38. YY=50 – Szoftverszelet CRC hiba másodszor

39. YY=51 – Szoftver SHA256 hiba másodszor

40. YY=52 – Sikertelen szoftver frissítés, az AEE visszaáll az előző verzióra

41. YY=53 – UPDCLR utasításban megjelölt folyamat nem létezik

I/4. A következő szoftver szelet igénylése a NAV szervertől

## A működtető szoftver frissítése során az e mellékletben részletezett forgatókönyv szerint az AEE az

## „UPDREQ~NNN~XXXXXXXXX~HHHHHHHHHH” üzenetet küldi, ahol

## NNN – a következő szoftver szelet sorszáma három számjegyen

I/5. A működtető szoftver adott verziójának elkérése

## Az AEE a pénztárgép rendszerbe állítását követően a

## „REQFW~V~XXXXXXXXX” üzenet elküldésével kezdeményezheti a NAV-nál a működtető szoftver adott verziójának telepítését, ahol

## V – az igényelt szoftver verziószáma.

## Ennek hatására az e mellékletben leírt forgatókönyv szerint megtörténik a szoftverfrissítés, amennyiben az lehetséges. A „V” helyén álló „L” az üzenetben a szoftver legfrissebb verzióját jelenti.

I/6. Első hitelesített bejelentkezés az AEE üzembe helyezésének folyamatában

## Az AEE az üzembe helyezési folyamat részeként, az e mellékletben részletezett forgalmazás során a

## „HELO~XXXXXXXXX~HHHHHHHHHH” üzenetet küldi.

I/7. Üzembe helyezési folyamat megindítása

## Az AEE a rendszerbe állítását követően a

## „DEFFST~XXXXXXXXX~UHK~HHHHHHHHHH” üzenettel, az üzemeltetés befejezését követően a

## „DEFMOD~XXXXXXXXX~UHK~S~HHHHHHHHHH” üzenet elküldésével kezdeményezheti a NAV-nál az új üzembe helyezési folyamat megindítását, ahol

## UHK – az üzembe helyezéshez előzőleg beszerzett 16 számjegyből álló üzembe helyezési kód

## S – a legutóbbi napzárásra vonatkozó bejegyzést tartalmazó naplóállomány sorszáma.

## Az új üzembe helyezési folyamat kizárólag a pénztárgép szervizmenüjéből indítható akkor, ha a pénztárgép hálózati áramforrásról üzemel, nincs nyitott adóügyi nap és a legutóbbi adóügyi nap zárását tartalmazó naplóállomány, valamint minden korábbi naplóállomány külső adathordozón az üzemeltető birtokában van. Az első vagy az új üzembe helyezés az e mellékletben részletezett forgalmazás eredményeként történhet meg.

I/8. Üzemeltetés befejezése

## Az AEE a pénztárgép üzembe helyezett állapotában a

## „SUSPEND~XXXXXXXXX” üzenettel kezdeményezi az üzemeltetés befejezését.

## Az üzemeltetés befejezésének folyamata kizárólag akkor indítható, ha a pénztárgép hálózati áramforrásról üzemel. Az üzemeltetés befejezése az e mellékletben részletezett forgalmazás eredményeként valósulhat meg.

I/9. Üzemeltetés folytatása

## Az AEE az üzemeltetés befejezését követően a

## „SUSPUNDO~XXXXXXXXX” üzenettel kezdeményezi az üzemeltetés folytatását a meglévő üzemeltető vonatkozásában.

## Az üzemeltetés folytatása az e mellékletben részletezett forgalmazás eredményeként valósulhat meg.

I/10. Az AEE-NAV kommunikáció tesztelése

## Az AEE a pénztárgép rendszerbe állítását követően a

## „PING~XXXXXXXXX” üzenet elküldésével tesztelheti az AEE-NAV kommunikációt.

## Ezt az üzenetet kizárólag erre irányuló kezelői beavatkozás válthatja ki. A pénztárgépen lehetővé kell tenni olyan kezelői beavatkozást, ami ezen üzenet küldését váltja ki. A kommunikáció tesztelését az AEE egy percen belül legfeljebb kettő, egy napon belül legfeljebb száz alkalommal kezdeményezheti.

I/11. A NAV szerver által kért állapotjelentés üzenet

## Az AEE a NAV szerver e mellékletben megjelölt utasítására az e mellékletben részletezett forgatókönyv szerint a

## „STATUS~XXXXXXXXX~UZE=Q1~BLO=Q2~DEF=Q3~VAT=Q4~FRW=Q5~EUR=Q6~CON=Q7~UDC=Q8~PRN=Q9~STS=Q10~HHHHHHHHHH” üzenetet elküldésével jelenti az itt megjelölt folyamatok mindegyikének aktuális állapotát a pénztárgépen.

| Folyamatjelölő | Q lehetséges értékei és jelentésük |

| UZE | Rendszerbe állítás és üzembe helyezés állapota: 0 – Nincs rendszerbe állítva 1 – Rendszerbe állítva, első üzembe helyezés nem történt meg 2 – Üzembe helyezve 3 – Üzemeltetés befejezve |

| BLO | Blokkolás állapota: 0 – normál állapot (nincs blokkolva és nincs sikertelen blokkolás) 1 – NAV által blokkolva 2 – NAV általi blokkolás sikertelen 3 – NAV általi blokkolás feloldása sikertelen 4 – A pénztárgép önmagát blokkolta |

| DEF | Adózói és telephely adatok (fejléc) állapota: 0 – Fejléc nincs 1 – Fejléc rendben 2 – Fejléc frissítése végrehajtásra vár 3 – Fejléc frissítés sikertelen |

| VAT | ÁFA tábla frissítés állapota: 0 – ÁFA tábla nincs 1 – ÁFA tábla beállítva 2 – ÁFA tábla frissítése végrehajtásra vár 3 – ÁFA tábla frissítése sikertelen |

| FRW | Szoftver frissítés állapota: 0 – nincs szoftver frissítési folyamat 1 – felszólítás megérkezett 2 – fejléc megérkezett 3 – szeletek letöltése folyamatban 4 – szoftver sikeresen letöltve az AEE-be 5 – szoftver frissítésre átadva 6 – szoftver frissítés végrehajtásra vár 7 – szoftver frissítés sikertelen |

| EUR | Euró átállás állapota: 0 – nincs ilyen folyamat 1 – dátumok fogadva 2 – felkészülési időszak megkezdődött 3 – euró átállás megtörtént 4 – kivezetési időszak vége |

| CON | Bejelentkezési gyakoriság beállítási folyamat állapota: Q értéke a bejelentkezési gyakoriság, percben |

| UDC | Folyamat törlés folyamat állapota: 0 – nincs folyamat törlés folyamat VAT/FRW/DEF/EUR/CON/FIL/PRN/ALL – felszólítás érkezett 1 – folyamat sikeresen zárult |

| PRN | Üzenet nyomtatási folyamat állapota: 0 – nincs üzenet nyomtatási folyamat 1 – üzenet nyomtatási folyamat ütemezve 2 – üzenet nyomtatási folyamat sikeres 3 – üzenet nyomtatási folyamat sikertelen |

| STS | A gyártó által meghatározott, legfeljebb 20 karakter hosszú állapotjelzés |

I/12. AEE állapotjelentés üzenet

## Az AEE az üzenetben szereplő folyamatok állapotának változásakor az e mellékletben leírt forgatókönyv szerint a

## „STATUS~XXXXXXXXX~UZE=Q1~BLO=Q2~DEF=Q3~VAT=Q4~FRW=Q5~EUR=Q6~CON=Q7~UDC=Q8~PRN=Q9~STS=Q10” üzenetet elküldésével jelenti az itt megjelölt folyamatok mindegyikének aktuális állapotát a pénztárgépen. A Q1-Q10 lehetséges értékei és jelentésük azonos az I/11. üzenetnél leírtakkal.

II. Az AEE által fogadott üzenetek

II/1. Felszólítás azonnali bejelentkezésre

## Az AEE részére küldött „CMSSL~XXXXXXXXX” üzenet szólítja fel a pénztárgépet azonnali elsőbbségi bejelentkezés végrehajtására.

## Az üzenetet a bekapcsolt pénztárgépben működő AEE-nek nek mindenkor fogadnia kell, az üzenet fogadását követően haladéktalanul elsőbbségi bejelentkezést kell végrehajtania az e mellékletben részletezett forgatókönyv szerint.

## II/2. Utasítás adatszolgáltatásra

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul a NAV a

## „TRMNOW~F~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t azonnali adatszolgáltatásra, ahol

## F – az a naplófájl sorszám, aminél nagyobb sorszámú naplóállományok küldésére vonatkozik az utasítás.

## Erre az AEE haladéktalanul:

a) lezárja minden adózó aktuálisan nyitott naplóállományát

b) egyesével, növekvő sorszám szerint, az e mellékletben részletezett forgatókönyv alapján elküldi a NAV részére az összes olyan naplóállományt, aminek sorszáma nagyobb, mint F.

II/3. Az AEE legutóbbi üzenetéről szóló visszaigazolás

A NAV az AEE egyes üzeneteire válaszul az „ACK~YY~HHHHHHHHHH” üzenetet küldi az e mellékletben részletezett forgatókönyvek szerint, ahol

YY – a visszaigazolás jellegét jelölő kód,

Az YY lehetséges értékei:

a) YY=00 – Általános hiba az üzenetben, kommunikációban, naplófájl fogadásban. Az így nyugtázott események nem voltak sikeresek, a munkamenet sikertelenül zárult. Utasítás az SSL kapcsolat bontására.

b) YY=02 – sikeresen fogadott naplófájl nyugta és következő naplófájl küldési utasítás,

c) YY=03 – sikeresen fogadott naplófájl nyugta további adási utasítás nélkül, melynek fogadását követően az AEE-nek azonnal bontania kell az SSL kapcsolatot,

d) YY=04 – sikeresen fogadott üzenet nyugta, melynek fogadását követően az AEE-nek azonnal bontania kell az SSL kapcsolatot

e) YY=05 – A REQFW kérés jelenleg nem hajtható végre, az AEE-nek azonnal bontania kell az SSL kapcsolatot

f) YY=06 – Az üzembe helyezési folyamat adott lépése sikeres volt.

g) YY=07 – Az üzembe helyezési, megszemélyesítési, átszemélyesítési folyamat egésze sikeres volt, az AEE-nek azonnal bontania kell az SSL kapcsolatot.

h) YY=08 – üzemeltetés befejezése lefolytatható

i) YY=09 – sikeresen fogadott üzenetről szóló nyugta, melynek fogadását követően az AEE-nek azonnal egy normál bejelentkező üzenetet (TRMRDY) kell küldenie

j) YY=10 – Utasítás a DEFMOD üzenet S paraméterében megadott sorszámú, valamint minden kisebb sorszámú naplóállomány olvashatatlanná tételére (a 0. sorszámú regisztrációs állománytól eltekintve), továbbá az SSL kapcsolat bontására.

k) YY=50 – Nem érvényes üzembe helyezési kód

l) YY=51 – Az üzembe helyezési kódot már felhasználták

m) YY=52 – Nem nyilvántartott AEE

n) YY=53 – Az AP szám már regisztrálva van másik AEE-hez

o) YY=54 – Ez az AEE már regisztrált másik AP számmal

p) YY=55 – Ez az AEE már regisztrált másik üzembe helyezési kóddal

q) YY=56 – Az IMEI nincs párban az IMSI-vel

r) YY=57 – Az AEE már megszemélyesítve.

s) YY=58 – Érvénytelen engedélyszám vagy szoftver verzió

t) YY=60 – Az üzemeltetés befejezése nem hajtható végre

u) YY=61 – Üzemeltetés befejezése folyamat sikertelen, utasítás az SSL kapcsolat bontására.

v) YY=64 – Az üzemeltetés befejezése nyugtázva

w) YY=65 – A művelet nem hajtható végre, utasítás az SSL kapcsolat bontására

II/4. Utasítás a pénztárgép blokkolt állapotba hozására

## A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul a „PTGBLCK~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t a pénztárgép blokkolt állapotba hozására.

## Ennek hatására az AEE blokkolja a pénztárgépet és az e mellékletben részletezett forgatókönyv szerinti választ küldi.

II/5. Utasítás a pénztárgép blokkolásának feloldására

## A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul az „UNBLCK~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t a pénztárgép blokkolt állapotának feloldására.

## Ennek hatására az AEE feloldja a pénztárgép blokkolt állapotát és az e mellékletben részletezett forgatókönyv szerinti választ küldi.

II/6. A pénztárgép működtető szoftver frissítése (firmware update)

## A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul, vagy az AEE ezirányú igényére a „FRWUPD~ééééhhnnóóppmm~HHHHHHHHHH” üzenettel ad utasítást a működtető szoftver frissítésére, ahol

## ééééhhnnóóppmm – a működtető szoftver telepítésére kijelölt végső időpont.

## A működtető szoftver akkor telepítendő, ha nincs nyitott adóügyi nap a pénztárgépen. A pénztárgép nem teheti lehetővé adóügyi nap megnyitását a működtető szoftver sikeres telepítése nélkül az üzenetben megjelölt időpont után.

## Az e mellékletben részletezett forgatókönyv szerint a NAV az egyes szoftver szeletek tulajdonságait az

## „UPDDTL~NNN~CCCC~KKKKK~HHHHHHHHHH” üzenettel jelzi, ahol

## NNN – a szoftver szeletek száma

## CCCC – az adott szoftver szelet 32 bites CRC ellenőrző kódja 8 karakteren

## KKKKK – a szoftver egészének SHA256 algoritmussal képzett ellenőrző kódja 64 karakteren

## Az üzenetben a ~CCCC szakasz értelemszerűen ismétlődik annyiszor, ahány szeletből áll a szoftver.

II/7. Utasítás az egyes forgalmi gyűjtőkhöz kapcsolódó ÁFA kulcsok és jelölő címkék módosítására

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a NAV az egyes forgalmi gyűjtőkhöz tartozó ÁFA kulcsok módosítására a

## „VATUPD~XXXXXXXXX~ééééhhnnóóppmm~A-AAAA-BBBB-CCCC~B-AAAA-BBBB-CCCC~C-AAAA-BBBB-CCCC~D-AAAA-BBBB-CCCC ~E-AAAA-BBBB-CCCC~HHHHHHHHHH” üzenet elküldésével ad utasítást az AEE részére, ahol

## ééééhhnnóóppmm – Azon időpont éve, hónapja, napja, órája, perce, másodperce, amit követően az üzenetben megadott kulcsokat és kategória címkéket alkalmazni kell a pénztárgépen.

## A, B ,C ,D ,E – a változással érintett forgalmi gyűjtők első karaktere

## AAAA – a megadott időponttól az adott karakterrel kezdődő jelű forgalmi gyűjtőkre érvényes ÁFA-kulcs, százalékban kifejezve, százalékjel nélkül, szükség esetén tizedesvesszőt alkalmazva

## BBBB – az adott ÁFA kulcshoz tartozó ÁFA tartalom, százalékban kifejezve, százalékjel nélkül, szükség esetén tizedesvesszőt alkalmazva

## CCCC – az érintett forgalmi gyűjtőkre érvényes címke, aminek hossza maximálisan 8 karakter.

## Egy gyűjtőhöz minden esetben egy „AAAA”, egy „BBBB” és egy „CCCC” érték tartozik.

## A VATUPD üzenet minden esetben a gyűjtők teljes készletét tartalmazza függetlenül attól, hogy egy-egy gyűjtő adatai módosultak-e.

## Az ÁFA kulcsok és kategória címkék módosítása a NAV üzenet alapján történik, azt a pénztárgépen más módon csak az egyedi mentesítéssel rendelkező gépeken lehet beállíthatóvá tenni.

## Az ÁFA tábla frissítését a pénztárgépnek zárt adóügyi napnál kell végrehajtania úgy, hogy az üzenetben megjelölt időpontot követően nem végezheti el a pénztárgép új adóügyi nap megnyitását, ha nem került sor a frissítés érvényesítésére.

II/8. Utasítás üzemeltetői vagy telephely adatok frissítésére a pénztárgépen

## A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a

## „DEFUPD~XXXXXXXXX~P1a~P2bbb~P3ccc~P4ddd~P5eee~P6fff~P7ggg~P8hhh~HHHHHHHHHH” üzenettel ad utasítást a pénztárgép üzemeltetői vagy telephely adatainak módosítására. Az egyes paraméterek lehetséges értékeit és jelentését az alábbi táblázat foglalja össze:

## Az üzenetben szereplő P1 paraméter értékétől függően a P2-P8 paraméterek jelentése az alábbi:

| P1-nél szereplő ’a’ értéke | Változás tárgya | bbb jelentése (P2) | ccc jelentése (P3) | ddd jelentése (P4) | eee jelentése (P5) | fff jelentése (P6) | ggg jelentése (P7) | hhh jelentése (P8) |

| 1 | Pénztárgép üzemeltető adatai, üzemanyagkúton használt kétvállalkozós pénztárgép esetén az üzemanyag tulajdonos adózó adatai változnak | Adózó adószáma 12345678- 1-12 formátumban | Adózó neve | Adózó székhelyének új irányító-száma | Adózó székhely település | Adózó székhely közterület neve | Adózó székhely közterület jellege | Adózó székhely házszám |

| 2 | Üzemanyagkúton használt kétvállalkozós pénztárgépen az üzemeltető adózó adatai változnak | Adózó adószáma 12345678- 1-12 formátumban | Adózó neve | Adózó székhelyének új irányító-száma | Adózó székhely település | Adózó székhely közterület neve | Adózó székhely közterület jellege | Adózó székhely házszám |

| 3 | a pénztárgép üzemeltetési helye változik | (üres) | Üzlet neve | Üzlet irányítószáma | Üzlet település | Üzlet közterület neve | Üzlet közterület jellege | Üzlet házszáma |

## A pénztárgépnek az egyes paraméterek vonatkozásában az alábbi maximális hosszúságú értékeket kell kezelnie, figyelemmel az adatokban szerepeltethető karakterek tárigényére:

| Paraméter | Maximális hossz (karakter) |

| P1 | 1 |

| P2 | 20 |

| P3 | 100 |

| P4 | 6 |

| P5 | 50 |

| P6 | 50 |

| P7 | 20 |

| P8 | 50 |

## Az érkezett fejlécadatok nyomtatásakor a pénztárgép nyomtatója egy-egy sortörés, illetve sorvégi kötőjel karaktert szúrhat be a megfelelő megjelenítés érdekében. A bizonylat fejlécére nyomtatott adatoknak meg kell egyezni az üzenetben elküldött adatokkal, az így beszúrt karakterektől eltekintve.

## Az üzenet fogadását követően az AEE-nek gondoskodnia kell a jelzett módosítások érvényesítéséről a pénztárgépen úgy, hogy a módosítás végrehajtására zárt adóügyi nap mellett, az üzenet fogadását követő első napnyitás előtt kerüljön sor. A pénztárgépnek a módosítás végrehajtásáról az e mellékletben részletezett forgatókönyv szerinti választ kell küldenie a NAV-nak.

II/9. Utasítás az euró átálláshoz kapcsolódó dátumok beállítására

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a NAV az

## EURD~XXXXXXXXX~D1~D2~D3~aaa~HHHHHHHHHH" üzenet megküldésével ad utasítást az euró átálláshoz kapcsolódó dátumok módosítására, ahol

## D1 – a felkészülési időszak kezdete ééééhhnnóóppmm formátumban

## D2 – az átállás időpontja ééééhhnnóóppmm formátumban

## D3 – a kivezetési időszak vége ééééhhnnóóppmm formátumban

## aaa – a rögzítésre kerülő HUF/EUR árfolyam hat értékes jegy pontossággal, tizedesvesszőt alkalmazva, legfeljebb 12 karakteren

## Az üzenet fogadását követően az AEE-nek gondoskodnia kell a jelzett módosítások átvezetéséről a pénztárgépen és az e mellékletben részletezett forgatókönyv szerinti választ kell küldenie a NAV-nak.

II/10. Utasítás az AEE normál bejelentkezési gyakoriságának módosítására

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a NAV a

## „CONSET~XXXXXXXXX~DTNEXT~DTCONT~HHHHHHHHHH” üzenettel határozza meg az AEE következő normál bejelentkezésének időpontját és az azt követő bejelentkezési gyakoriságot, ahol

## DTNEXT – Az AEE következő normál bejelentkezésének elvárt időpontja az üzenet fogadásától számítva, percben. Lehetséges értékei 1 és 9999 közötti egész számok.

## DTCONT – Az AEE normál bejelentkezési gyakorisága az üzenet fogadását követő első normál bejelentkezést követően, percben. Lehetséges értékei 1 és 9999 közötti egész számok.

## Az üzenet fogadását követően az AEE-nek gondoskodnia kell a jelzett módosítások átvezetéséről a pénztárgépen és az e mellékletben részletezett forgatókönyv szerinti választ kell küldenie a NAV-nak.

II/11. Utasítás az AEE alaphelyzetbe állítására

## Az AEE normál vagy elsőbbségi bejelentkezésére, illetve egyéb üzeneteire válaszul az e mellékletben részletezett forgatókönyvek szerint a NAV az

## „UPDCLR~XXXXXXXXX~R~HHHHHHHHHH” üzenettel ad utasítást az AEE-ben futó frissítési folyamatok egyikének vagy mindegyikének lezárására, illetve a jelzett paraméterek alapértelmezésre állítására, az alábbiak szerint:

| R értéke | Elvárt művelet |

| VAT | Lezárja és sikertelennek tekinti a futó ÁFA tábla frissítési folyamatot |

| FRW | Lezárja és sikertelennek tekinti a futó szoftverfrissítési folyamatot |

| DEF | Lezárja és sikertelennek tekinti a futó adózói adat frissítési folyamatot |

| EUR | Lezárja és sikertelennek tekinti a futó euró átállási dátum frissítési folyamatot a jövőbeni dátumokra vonatkozóan |

| PRN | Lezárja és sikertelennek tekinti a futó technikai tájékoztatás bizonylat nyomtatás folyamatot |

| CON | Az alapértelmezett 30 percre állítja a normál bejelentkezések időközét |

| FIL | Az alapértelmezett 1024 kilobájtra állítja a naplóállomány méretkorlátot |

| ALL | A fenti műveletek mindegyikét elvégzi. |

## Az üzenet fogadását követően az AEE-nek végre kell hajtania az elvárt műveleteket.

II/12. Utasítás a naplófájl méretkorlát megváltoztatására

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyvek szerint a NAV a

## FILESIZE~XXXXXXXXX~N~HHHHHHHHHH, üzenettel ad utasítást az AEE-ben vezetett naplóállomány méretkorlátjának beállítására, ahol

## N – az új méretkorlát, kilobájtban megadva.

## Amennyiben az AEE-ben vezetett naplófájl mérete eléri a megadott méretkorlátot, azt az AEE-nek le kell zárnia és a naplózást egy újonnan nyitott naplófájlban kell folytatnia. Az első FILESIZE üzenet fogadását megelőzően ez a méretkorlát 1024 kilobájt.

## Az AEE működési sajátosságainak megfelelően alkalmazhat a FILESIZE utasításban megadottnál alacsonyabb méretkorlátot is.

II/13. Utasítás technikai tájékoztatás bizonylat nyomtatására

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyvek szerint a NAV a

## PRNT~XXXXXXXXX~SZOVEG~HHHHHHHHHH, üzenettel ad utasítást az adott üzenet kinyomtatására a pénztárgép nyugtanyomtatóján, ahol

## SZOVEG – az üzenet legfeljebb 1024 karakter hosszúságú szövege, ami kizárólag betűket, számokat, valamint a szóköz, kérdőjel, felkiáltójel, pont, vessző, kötőjel, zárójel, alulvonás(_), csillag (*), százalék (%), egyenlő (=), plusz (+), bekezdésjel (§), törtvonal (/), visszaperjel (\) és kukac (@) karaktereket tartalmazhat.

## Az üzenet fogadását követő első napzárást követően a pénztárgépnek ki kell nyomtatnia a kapott üzenetet a pénztárgép nyomtatóján. Az üzenetben szereplő „\n” karaktersorozatot „új sor” karakterként kell értelmezni a nyomtatáskor.

II/14. Utasítás állapotjelentésre

## Az AEE normál vagy elsőbbségi bejelentkezésére válaszul a NAV a

## „STSREQ~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t állapotjelentés küldésére.

## Erre az AEE haladéktalanul elküldi a teljes körű állapotjelentést az e mellékletben részletezett forgatókönyv szerint.

III. Az AEE-NAV forgalmazások forgatókönyvei

## A forgalmazási forgatókönyvek irányának oszlopában alkalmazott rövidítések és az egyes szerverekkel folytatott kommunikáció

## MSG: A NAV üzenet szervere (https://opg.nav.gov.hu/msg)

## NFL: A NAV naplófájl szervere (https://opg.nav.gov.hu/nfl)

## SWU: A NAV szoftverfrissítés szerver (https://opg.nav.gov.hu/swu)

## RMS: A NAV regisztrációs folyamathoz kapcsolódó üzenetszervere (https://opgreg.nav.gov.hu/msg)

## REG: A NAV regisztrációs eljárás szervere (https://opgreg.nav.gov.hu/reg)

## SSG: A NAV üzembe helyezési szervere (https://opgreg.nav.gov.hu/ssg)

## Az egyes szerverekkel váltott üzenetek belső felépítése:

## Az AEE→MSG, AEE→RMS, AEE→SWU, AEE→SSG irányú üzenetnél a tartalom típusa „urlencoded”, az üzenet karaktersorozatot tartalmazó form paraméter neve: „MSG”.

## AEE→REG irányban a tartalom típusa „content type= multipart/form-data”, a fájlt azonosító elem neve: „REG”. Ekkor egy pkcs#7 formátumú fájl kerül továbbításra mely tartalmazza a regisztrációs fájlt, annak aláírását és a tanúsítványt.

## AEE→NFL irányban a tartalomtípus „content type= multipart/form-data”, a fájlt azonosító elem neve: „NFL”. Ekkor egy pkcs#7 formátumú fájl kerül továbbításra mely tartalmazza a naplófájlt és annak aláírását. Ikervállalkozós pénztárgép esetén a második fájlt „NFL2” néven kell azonosítani és egy másik boundary-ba kell elhelyezni.

## REG→AEE irányában, a pénztárgép rendszerbe állításakor leküldésre kerül az autentikációs tanúsítvány. A tartalom típusa „content type=application/octet-stream”, a leküldendő fájl tartalma közvetlen beleírásra kerül.

## SWU→AEE irányban, szoftver frissítésekor leküldésre kerül(nek) a szoftver bináris fájl(ok). A tartalom típusa „content type=application/octet-stream”, a leküldendő szoftver fájl tartalma közvetlen beleírásra kerül.

## MSG→AEE, NFL→AEE, SSG→AEE illetve RMS→AEE irányú kommunikáció során, a küldött üzenetre kapott válasz esetén, a tartalom típusa text/plain, az érkezett üzenet paraméternevet nem tartalmaz.

## Az egyes forgatókönyvek közötti átmenet lehetősége

## Az e mellékletben megadott forgatókönyvekben szereplő „ACK~03~HHHHHHHHHH” vagy „ACK~04~HHHHHHHHHH” visszaigazolás helyett a NAV szervernek lehetősége van az „ACK~09~HHHHHHHHHH” üzenetet küldeni. Ezt az üzenetet az addig lezajlott forgalmazásra vonatkozóan az AEE-nek úgy kell értelmezni, mint az „ACK~03~HHHHHHHHHH” vagy „ACK~04~HHHHHHHHHH” üzenetet, de az SSL kapcsolat bontása helyett haladéktalanul egy normál bejelentkezés üzenetet (TRMRDY) kell küldenie az MSG-nek.

## Kommunikációs hiba kezelése a NAV szerver oldalon.

## Ha az alább ismertetett forgatókönyvek szerinti forgalmazások során a NAV által küldött üzenetre az üzenet elküldését követő 30 percen belül az AEE nem küldi el a lehetséges válaszok egyikét, vagy a lehetséges válaszok helyett normál vagy elsőbbségi bejelentkező üzenetet küld, akkor a NAV szerver az adott üzenetet elveszettnek tekinti. A NAV szerver az elveszettnek tekintett üzenetet újra megkísérli elküldeni. Kétszeri sikertelen ismétlést követően az adott folyamatot a NAV szerver meghiúsultnak tekinti, a NAV szerver az AEE következő bejelentkezésekor UPDCLR utasítást küld.

1. eset: AEE bejelentkezik, a NAV nem kér adatszolgáltatást

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | NAV elutasító válasz | ACK~04~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE bontja az SSL kapcsolatot |

2. eset: AEE bejelentkezik, a NAV kér adatszolgáltatást

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás adatszolgáltatásra | TRMNOW~F~HHHHHHHHHH | MSG→AEE |

| Az AEE lezárja az aktuálisan vezetett naplóállományt és az „F” értéknél nagyobb sorszámú naplófájlokat elküldi egyesével, sorszám szerint növekvő sorrendben. |

| 4. | Naplófájl küldése | (fájlnév~HHHHHHHHHH) és tartalom | AEE→NFL |

| 5. | A naplófájl fogadását a NAV az 5a., az 5b., vagy az 5c. üzenettel nyugtázza. |

| 5a. | NAV visszaigazolás és utasítás a következő fájl küldésére | ACK~02~HHHHHHHHHH | NFL→AEE |

| 5b. | NAV visszaigazolás | ACK~03~HHHHHHHHHH | NFL→AEE |

| 5c. | NAV hibajelzés | ACK~00~HHHHHHHHHH | NFL→AEE |

| 6. | Az AEE az 5a. üzenet fogadása esetén a 4. lépéssel folytatja. Amennyiben nincs újabb lezárt naplófájl, akkor a 6b. üzenetet küldi el az AEE és a folyamat a 7. lépéssel folytatódik. Az 5b. üzenet fogadása esetén az AEE a folyamatot a 7. lépéssel folytatja. Az 5c. üzenet fogadása esetén az AEE újraküldi a 4. lépésben legutóbb küldött naplófájlt. Ha az AEE egy fájl küldése kapcsán ötödször is az 5c. üzenetet kapja, akkor az AEE elküldi a 6a. üzenetet és a folyamat a 7. lépéssel folytatódik. |

| 6a. | Sikertelen fájlküldés | ANS~XXXXXXXXX~37~HHHHHHHHHH | AEE→MSG |

| 6b. | Nincs több lezárt naplóállomány | ANS~XXXXXXXXX~17~HHHHHHHHHH | AEE→MSG |

| 7. | Az AEE bontja az SSL kapcsolatot |

3. eset: A NAV blokkolja a pénztárgépet

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Blokkoló üzenet | PTGBLCK~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE megkísérli blokkolt állapotba hozni a pénztárgépet. Sikeres végrehajtás esetén az 5a. üzenetet, sikertelen végrehajtás esetén az 5b. üzenetet küldi. |

| 5a. | Blokkolás végrehajtva | ANS~XXXXXXXXX~01~HHHHHHHHHH | AEE→MSG |

| 5b. | Blokkolás végrehajtása sikertelen | ANS~XXXXXXXXX~31~HHHHHHHHHH | AEE→MSG |

| 6. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 7. | Az AEE bontja az SSL kapcsolatot |

4. eset: A NAV feloldja a pénztárgép blokkolását

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Blokkolást feloldó üzenet | UNBLCK~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE megkísérli feloldani a pénztárgép blokkolt állapotát. Sikeres végrehajtás esetén az 5a. üzenetet, sikertelen végrehajtás esetén az 5b. üzenetet küldi. |

| 5a. | Blokkolás feloldása végrehajtva | ANS~XXXXXXXXX~02~HHHHHHHHHH | AEE→MSG |

| 5b. | Blokkolás feloldás végrehajtása sikertelen | ANS~XXXXXXXXX~32~HHHHHHHHHH | AEE→MSG |

| 6. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 7. | Az AEE bontja az SSL kapcsolatot |

5. eset: ÁFA-tábla módosítása

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás az ÁFA-kulcsok módosítására | VATUPD~XXXXXXXXX~ééééhhnnóóppmm~A-AAAA-BBBB-CCCC~B-AAAA-BBBB-CCCC~C-AAAA-BBBB-CCCC~D-AAAA-BBBB-CCCC~E-AAAA-BBBB-CCCC~HHHHHHHHHH | MSG→AEE |

| 4. | Ha az AEE fogadta és értelmezni képes az üzenetet, a 4a. üzenetet küldi, egyébként a 4b. üzenetet küldi. |

| 4a. | Visszaigazolás az utasítás fogadásáról | ANS~XXXXXXXXX~03~HHHHHHHHHH | AEE→MSG |

| 4b. | Üzenet nem értelmezhető | ANS~XXXXXXXXX~36~HHHHHHHHHH | AEE→MSG |

| 5. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 6. | Az AEE bontja az SSL kapcsolatot |

| Ha a 4. lépésben a 4a. üzenet került elküldésre, akkor későbbi időpontban, amikor a módosítás beállítása a pénztárgépen megtörténik, az AEE a 7. lépéssel folytatja. |

| 7. | Az AEE gondoskodik a megfelelő módosítások végrehajtásáról. |

| 8. | Az AEE felépíti az SSL kapcsolatot |

| Sikeres módosítás esetén az AEE a 9a. üzenetet, sikertelenség esetén a 9b. üzenetet küldi el. |

| 9a. | Visszaigazolás a módosítás elvégzéséről | ANS~XXXXXXXXX~04~HHHHHHHHHH | AEE→MSG |

| 9b. | ÁFA tábla frissítése sikertelen | ANS~XXXXXXXXX~35~HHHHHHHHHH | AEE→MSG |

| 10. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 11. | Az AEE bontja az SSL kapcsolatot |

6. eset: Pénztárgép adózói vagy telephely adatainak frissítése

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás az adózói vagy telephelyadatok módosítására | DEFUPD~XXXXXXXXX~P1a~P2bbb~P3ccc~P4ddd ~P5eee~P6fff~P7ggg~P8hhh~HHHHHHHHHH | MSG→AEE |

| 4. | Az adózói adatok módosítására vonatkozó üzenet fogadásáról az AEE visszaigazolást küld. Sikeres fogadás esetén az AEE a 4a. üzenetet küldi. Sikertelenség esetén az AEE a 4b. üzenetet küldi, bontja az SSL kapcsolatot és a folyamat sikertelenül zárul. |

| 4a. | Adózói adatok fogadása sikeres | ANS~XXXXXXXXX~08~HHHHHHHHHH | AEE→MSG |

| 4b. | Adózói adatok fogadása sikertelen | ANS~XXXXXXXXX~34~HHHHHHHHHH | AEE→MSG |

| 5. | A folyamat a 3. vagy a 6. lépéssel folytatódik. |

| 6. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 7. | Az AEE bontja az SSL kapcsolatot |

| Ha a 4. lépésben a 4a. üzenet került elküldésre, akkor későbbi időpontban, amikor a módosítás beállítása a pénztárgépen megtörténik, az AEE a 8. lépéssel folytatja. |

| 8. | Az AEE gondoskodik a tárolt adózói adatok módosításáról. |

| 9. | Az AEE felépíti az SSL kapcsolatot |

| 10. Sikeres módosítás esetén az AEE a 10a. üzenetet, sikertelenség esetén a 10b. üzenetet küldi el. |

| 10a. | Adózói adatok frissítése megtörtént | ANS~XXXXXXXXX~18~HHHHHHHHHH | AEE→MSG |

| 10b. | Adózói adatok frissítése sikertelen | ANS~XXXXXXXXX~33~HHHHHHHHHH | AEE→MSG |

| 11. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 12. | Az AEE bontja az SSL kapcsolatot |

## Egy adózói vagy telephely adat frissítési folyamaton belül a NAV legfeljebb kettő, kétvállalkozós pénztárgépen legfeljebb három DEFUPD üzenetet küld úgy, hogy az üzenetek P1 paraméterének értéke különbözik. A pénztárgép adózói vagy telephely adatainak frissítésére irányuló üzenet fogadását a pénztárgép akkor és csak akkor tekintheti sikeresnek, ha a 6. lépésben jelölt visszaigazolás megtörtént, egyébként teljes egészében sikertelennek kell tekintenie.

7. eset: Euró átállás dátum módosítása

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás az euró átállás dátumának módosítására | EURD~XXXXXXXXX~D1~D2~D3~aaa~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE megkísérli a módosítás végrehajtását. Siker esetén az AEE a 4a. üzenetet küldi. Sikertelenség esetén az AEE a 4b. üzenetet küldi. |

| 4a. | Visszaigazolás a módosítás végrehajtásáról | ANS~XXXXXXXXX~11~HHHHHHHHHH | AEE→MSG |

| 4b. | Sikertelen fogadás jelzése | ANS~XXXXXXXXX~39~HHHHHHHHHH | AEE→MSG |

| 6. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 7. | Az AEE bontja az SSL kapcsolatot |

| Ha a 4. lépésben a 4a. üzenet került elküldésre, akkor későbbi időpontban, amikor az euró átállás a pénztárgépen megtörténik, az AEE a 8. lépéssel folytatja. |

| 8. | Az AEE az üzenetben küldött időszak életbe lépésekor gondoskodik a szükséges módosítások elvégzéséről. |

| 9. | Az AEE felépíti az SSL kapcsolatot |

| 10. Időszak sikeres aktiválása esetén az AEE a 10a. üzenetet, sikertelenség esetén a 10b. üzenetet küldi el. |

| 10a. | Euró átállás megtörtént | ANS~XXXXXXXXX~20~HHHHHHHHHH | AEE→MSG |

| 10b. | Euró átálláshoz kapcsolódó időszak beállítása sikertelen | ANS~XXXXXXXXX~49~HHHHHHHHHH | AEE→MSG |

| 11. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 12. | Az AEE bontja az SSL kapcsolatot |

8. eset: Utasítás a következő bejelentkezési időpont és a bejelentkezési gyakoriság módosítására

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás a bejelentkezési gyakoriság módosítására | CONSET~XXXXXXXXX~DTNEXT~DTCONT~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE megkísérli a következő normál bejelentkezési időpont és a bejelentkezési gyakoriság megfelelő beállítását. Siker esetén az 4a. üzenetet, sikertelenség esetén az 4b. üzenetet küldi. |

| 4a. | Visszaigazolás a módosítás végrehajtásáról | ANS~XXXXXXXXX~10~HHHHHHHHHH | AEE→MSG |

| 4b. | Sikertelen végrehajtás jelzése | ANS~XXXXXXXXX~38~HHHHHHHHHH | AEE→MSG |

| 5. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 6. | Az AEE bontja az SSL kapcsolatot |

9. eset: Az AEE működtető szoftverének frissítése

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás a működtető szoftver frissítésére | FRWUPD~ééééhhnnóóppmm~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE az új szoftver fogadására kész | ANS~XXXXXXXXX~05 ~HHHHHHHHHH | AEE→SWU |

| 5. | A szeletek adatai | UPDDTL~NNN~CCCC~KKKKK~HHHHHHHHHH | SWU→AEE |

| 6. Az egyes szeletek letöltése. A 7-8. lépések ismétlődnek mindaddig, amíg az az AEE a 9. pontban felsorolt üzenetek egyikét nem küldi. Átviteli hiba esetén az AEE ugyanazt a szoftverszeletet legfeljebb kétszer kérheti el. |

| 7. | Az AEE az NNN sorszámú szelet küldését kéri | UPDREQ~NNN~XXXXXXXXX~HHHHHHHHHH | AEE→SWU |

| 8. | Szoftverszelet küldése | (Szoftver szelet) | SWU→AEE |

| 9. Amennyiben a szoftverszelet fogadása sikeres volt, az AEE újabb szeletet kér a 7. pontban szereplő üzenet elküldésével, ha még van hiányzó szelet. Ha a teljes szoftver sikeresen letöltésre került, az AEE a 9a. üzenetet küldi. Amennyiben egy adott szoftver szelet CRC ellenőrző kódjának ellenőrzése az adott szelet második letöltésekor is hibát jelez, az AEE a 9b. üzenetet küldi, a folyamat a 10. lépéssel folytatódik és sikertelenül zárul. Ebben az esetben az AEE-nek a hiányzó szeletek letöltését 4 órán belül meg kell kísérelnie. Amennyiben az adott szoftver összes szeletének letöltése után a teljes szoftver SHA256 ellenőrző kódjának ellenőrzése másodszor is hibát jelez, az AEE a 9c. üzenetet küldi, a folyamat a 10. lépéssel folytatódik és sikertelenül zárul. Ebben az esetben az AEE-nek a teljes letöltési folyamatot 4 órán belül meg kell kísérelnie. |

| 9a. | A szoftver fogadása sikeres | ANS~XXXXXXXXX~06~HHHHHHHHHH | AEE→SWU |

| 9b. | Szoftverszelet CRC hiba másodszor | ANS~XXXXXXXXX~50~HHHHHHHHHH | AEE→SWU |

| 9c. | Szoftver SHA256 hiba másodszor | ANS~XXXXXXXXX~51~HHHHHHHHHH | AEE→SWU |

| 10. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | SWU→AEE |

| 11. | Az AEE bontja az SSL kapcsolatot |

| Legkésőbb a 3. lépés üzenetében szereplő „ééééhhnnóóppmm”’ karaktersorozatban megjelölt napon, zárt adóügyi napnál az AEE telepíti a letöltött szoftvert. A működtető szoftver új verziójának telepítésének sikerességéről vagy sikertelenségéről az AEE jelentést küld a NAV-nak. |

| 12. | Az AEE felépíti az SSL kapcsolatot |

| 13. Ha a szoftver frissítése sikeres volt, akkor az AEE a 13a. üzenetet küldi el, egyébként a 9b. üzenetet. |

| 13a. | AEE visszaigazolja a szoftver telepítését | ANS~XXXXXXXXX~07~HHHHHHHHHH | AEE→SWU |

| 13b. | Sikertelen szoftverfrissítés jelzése | ANS~XXXXXXXXX~52~HHHHHHHHHH | AEE→SWU |

| 14. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | SWU→AEE |

| 15. | Az AEE bontja az SSL kapcsolatot |

## A folyamat során a NAV elküldi a kért szoftver adatszeletet; a szeleteket a sikeres CRC-ellenőrzés után az AEE-nek össze kell raknia, majd ellenőriznie kell az adatállomány SHA256 algoritmussal képzett ellenőrző kódjának megfelelőségét.

## Amennyiben a működtető szoftver letöltése nem kezdődött meg az FRWUPD üzenet fogadását követően 60 percen belül, az AEE-nek meg kell ismételnie a folyamatot az SSL csatorna kiépítése után a 4. lépéstől kezdve a FRWUPD üzenet fogadását követő 4 órán belül.

## Szoftver frissítés elakadása esetén a már letöltött szeleteket nem kell újra letölteni, hacsak a NAV erre vonatkozóan az UPDCLR parancs kiadásával utasítást nem ad.

10. eset: Pénztárgép rendszerbe állítása

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE elküldi a regisztrációs fájlt a NAV-nak | (regisztrációs állomány) | AEE→REG |

| Ha a NAV szerver hibát észlel az AEE által küldött regisztrációs fájlban, akkor a 2. számú lépéssel folytatja, majd lezárja a folyamatot. Megfelelő regisztrációs fájl esetén a NAV szerver a 3. számú lépéssel folytatja. |

| 2. | NAV hibajelzés, az üzembe helyezés meghiúsult | ACK~YY~HHHHHHHHHH YY=52 – „Nem nyilvántartott AEE” YY=53 – „Az AP szám már regisztrálva másik AEE-hez.” YY=54 – „Ez az AEE már regisztrált másik AP YY=56 – Az IMEI nincs parban az IMSI-vel. YY=57 – Az AEE már megszemélyesítve. YY=58 – Érvénytelen engedélyszám vagy firmware verzió.” | REG→AEE |

| 3. | Autentikációs tanúsítvány elküldése az AEE-nek (prv) | (prv fájl) | REG→AEE |

| 4. | Amennyiben a prv fájl fogadása sikeres volt, az AEE a 4a. üzenetet küldi és a folyamat az 5. lépéssel folytatódik. Egyébként az AEE a 4b. üzenetet küldi és bontja a kapcsolatot. A 4a. és 4b. lépésben HHHHHHHHHH értéke „0000000000”. |

| 4a. | Autentikációs tanúsítvány fogadva | ANS~XXXXXXXXX~09~HHHHHHHHHH | AEE→RMS |

| 4b. | Autentikációs tanúsítvány fogadása sikertelen | ANS~XXXXXXXXX~43~HHHHHHHHHH | AEE→RMS |

| 5. | Autentikációs tanúsítvány elküldése az AEE-nek (cer) | (cer fájl) | RMS→AEE |

| 6. | Amennyiben a cer fájl fogadása sikeres volt, az AEE a 6a. üzenetet küldi és a folyamat a 7. lépéssel folytatódik. Egyébként az AEE a 6b. üzenetet küldi és bontja a kapcsolatot. |

| 6a. | Autentikációs tanúsítvány fogadva | ANS~XXXXXXXXX~09~HHHHHHHHHH | AEE→RMS |

| 6b. | Autentikációs tanúsítvány fogadása sikertelen | ANS~XXXXXXXXX~43~HHHHHHHHHH | AEE→RMS |

| 7. | NAV nyugtázás | ACK~06~HHHHHHHHHH | RMS→AEE |

| 8. | Az AEE bontja a (nem titkosított) kapcsolatot |

| 9. | Az AEE felépíti az SSL kapcsolatot |

| 10. | Az AEE normál bejelentkezése (autentikáltan) | HELO~XXXXXXXXX~HHHHHHHHHH | AEE→MSG |

| 11. Sikeres bejelentkezésre válaszul a NAV a 11a. üzenetet, sikertelen bejelentkezés esetén a 11b. üzenetet küldi. |

| 11a. | Visszaigazolás sikeres bejelentkezésről | ACK~07~HHHHHHHHHH | MSG→AEE |

| 11b. | Visszaigazolás sikertelen bejelentkezésről | ACK~00~HHHHHHHHHH | MSG→AEE |

| 12. | Az AEE bontja az SSL kapcsolatot |

## A regisztrációs fájlt az AEE tárolójára „0” sorszámmal, a naplóállományok elnevezésére vonatkozó előírás szerint elnevezve kell eltárolni. A regisztrációs állomány adatmezőinek feltöltésekor a rendelkezésre nem álló adózói adatokat megfelelő számú „0” karakterrel kell kitölteni. Az üzembe helyezési kód mezőjében 16 db „0” szerepeltetendő.

## Amennyiben a 4a. lépésben szereplő üzenet elküldése már megtörtént, a sikertelenül zárult rendszerbe állítási folyamatot csak ugyanazokkal az adatokkal kísérelheti meg újra az AEE, amelyeket a sikertelenül zárult folyamatban küldte el. Ha a 11a. lépésben szereplő üzenet küldését követően az AEE újabb rendszerbe állítási folyamatot nem indíthat.

11/a. eset: Pénztárgép első üzembe helyezése

| Lépés | Leírás | Üzenet | Irány |

| A folyamat elindítására akkor kerülhet sor, ha a pénztárgép rendszerbe van állítva, de még nem történt üzembe helyezés. |

| 1. | Az AEE lezárja az aktuálisan vezetett naplóállományt és új naplóállományt nyit, majd felépíti az SSL kapcsolatot |

| 2. | Az AEE elindítja az üzembe helyezési folyamatot | DEFFST~XXXXXXXXX~UHK~HHHHHHHHHH | AEE→SSG |

| Ha a NAV szerver hibát észlel az AEE által küldött regisztrációs fájlban, akkor a 3. számú lépéssel folytatja, majd lezárja a folyamatot. Megfelelő üzembe helyezési kód esetén a NAV szerver a 4. számú lépéssel folytatja. |

| 3. | NAV hibajelzés, az üzembe helyezés meghiúsult | ACK~YY~HHHHHHHHHH YY=50 – „Nem érvényes üzembe helyezési kód.” YY=51 – „Az üzembe helyezési kódot már felhasználták.” YY=52 – „Nem nyilvántartott AEE.” YY=53 – Az AP szám már regisztrálva van másik AEE-hez YY=54 – „Ez az AEE már regisztrált másik AP számmal” YY=55 – „Ez az AEE már regisztrált másik üzembe helyezési kóddal.” | SSG→AEE |

| 4. | A NAV elküldi az AEE részére az üzemeltetői és működési hely adatokat az 5-6 lépések megfelelő számú ismétlésével |

| 5. | Üzemeltetői és működési hely adatok | DEFUPD~XXXXXXXXX~P1a~P2bbb~P3ccc~P4ddd ~P5eee~P6fff~P7ggg~P8hhh~HHHHHHHHHH | SSG→AEE |

| 6. | Az AEE megkísérli azonnal átvezetni az érkezett adatokat. Amennyiben ez sikeres, a 6a üzenetet küldi, és a folyamat a 7. lépéssel folytatódik. Sikertelen átvezetés esetén az AEE a 6b. üzenetet küldi, a folyamat az 12. lépéssel folytatódik és sikertelenül zárul. |

| 6a. | Adatok eltárolásának visszaigazolása | ANS~XXXXXXXXX~08~HHHHHHHHHH | AEE→SSG |

| 6b. | Adatok eltárolása sikertelen | ANS~XXXXXXXXX~33~HHHHHHHHHH | AEE→SSG |

| 7. | Utasítás az ÁFA-kulcsok módosítására | VATUPD~XXXXXXXXX~ééééhhnnóóppmm~A-AAAA-BBBB-CCCC~B-AAAA-BBBB-CCCC~C-AAAA-BBBB-CCCC~D-AAAA-BBBB-CCCC~E-AAAA-BBBB-CCCC~HHHHHHHHHH | SSG→AEE |

| 8. | Ha az AEE fogadta az üzenetet, és végrehajtotta az abban foglaltakat, akkor a 8a. üzenetet küldi és a forgalmazás a 9. lépéssel folytatódik. Egyébként az AEE a 8b. üzenetet küldi, a majd a folyamat a 11. lépéssel folytatódik és sikertelenül zárul. |

| 8a. | Visszaigazolás az utasítás fogadásáról | ANS~XXXXXXXXX~03~HHHHHHHHHH | AEE→SSG |

| 8b. | Üzenet fogadása sikertelen vagy az üzenet értelmezhetetlen | ANS~XXXXXXXXX~35~HHHHHHHHHH | AEE→SSG |

| 9. | Utasítás az euró átállás dátumának módosítására | EURD~XXXXXXXXX~D1~D2~D3~aaa~HHHHHHHHHH | SSG→AEE |

| 10. | Ha az AEE sikeresen fogadta az üzenetet és végrehajtotta a benne foglalt utasítást, akkor az AEE a 10a. üzenetet küldi és a forgalmazás a 11. lépéssel folytatódik. Egyébként a 10b. üzenetet küldi, a majd a folyamat a 12. lépéssel folytatódik és sikertelenül zárul. |

| 10a. | Visszaigazolás a módosítás végrehajtásáról | ANS~XXXXXXXXX~11~HHHHHHHHHH | AEE→SSG |

| 10b. | Sikertelen végrehajtás jelzése | ANS~XXXXXXXXX~39~HHHHHHHHHH | AEE→SSG |

| 11. | A folyamat sikeres lezárásáról a NAV a 11a. üzenetet küldi, sikertelen lezárásáról a 11b. üzenetet küldi. |

| 11a. | Visszaigazolás a folyamat sikerességéről | ACK~07~HHHHHHHHHH | SSG→AEE |

| 11b. | Visszaigazolás a folyamat sikertelenségéről | ACK~00~HHHHHHHHHH | SSG→AEE |

| 12. | Az AEE bontja az SSL kapcsolatot |

## Az üzembe helyezési folyamat kizárólag akkor tekinthető sikeresen befejezettnek, ha sikeresen megtörtént minden olyan módosítás, amire a NAV utasítást adott, majd az AEE fogadta a 12a. lépésben szereplő visszaigazoló üzenetet. A pénztárgép adóügyi nap nyitását kizárólag a sikeresen lezárult üzembe helyezési folyamatot követően teheti lehetővé.

11/b. eset: Pénztárgép befejezett üzemeltetést követő új üzembe helyezése (átszemélyesítés)

| Lépés | Leírás | Üzenet | Irány |

| A folyamat elindítására akkor kerülhet sor, ha a pénztárgép üzemeltetésének befejezése sikeresen lezajlott. (12. eset) |

| 1. | Az AEE lezárja az aktuálisan vezetett naplóállományt és új naplóállományt nyit. Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE elindítja az átszemélyesítési folyamatot | DEFMOD~XXXXXXXXX~UHK~S~HHHHHHHHHH | AEE→SSG |

| Ha a NAV szerver hibát észlel az AEE által küldött regisztrációs fájlban, akkor a 3. számú lépéssel folytatja, majd lezárja a folyamatot. Megfelelő üzembe helyezési kód esetén a NAV szerver a 4. számú lépéssel folytatja. |

| 3. | NAV hibajelzés, az üzembe helyezés meghiúsult | ACK~YY~HHHHHHHHHH YY=50 – „Nem érvényes üzembe helyezési kód.” YY=51 – „Az üzembe helyezési kódot már felhasználták.” YY=52 – „Nem nyilvántartott AEE.” YY=53 – Az AP szám már regisztrálva van másik AEE-hez YY=54 – „Ez az AEE már regisztrált másik AP számmal” YY=55 – „Ez az AEE már regisztrált másik üzembe helyezési kóddal.” | SSG→AEE |

| 4. | A NAV elküldi az AEE részére az üzemeltetői és működési hely adatokat az 5-6 lépések megfelelő számú ismétlésével |

| 5. | Üzemeltetői és működési hely adatok | DEFUPD~XXXXXXXXX~P1a~P2bbb~P3ccc~P4ddd ~P5eee~P6fff~P7ggg~P8hhh~HHHHHHHHHH | SSG→AEE |

| 6. | Az AEE megkísérli átvezetni az érkezett adatokat. Amennyiben ez sikeres, az AEE 6a. üzenetet küldi, majd a folyamat a 7. lépéssel folytatódik. Sikertelen frissítés esetén az AEE a 6b. üzenetet küldi, a folyamat a 13. lépéssel folytatódik és sikertelenül zárul. |

| 6a. | Adatok eltárolásának visszaigazolása | ANS~XXXXXXXXX~08~HHHHHHHHHH | AEE→SSG |

| 6b. | Adatok eltárolása sikertelen | ANS~XXXXXXXXX~33~HHHHHHHHHH | AEE→SSG |

| 7. | Utasítás az S-nél nem nagyobb sorszámú naplóállományok törlésére | ACK~10~HHHHHHHHHH | SSG→AEE |

| 8. | Az AEE bontja az SSL kapcsolatot |

| 9. | Az AEE törli a legutóbbi napzárást tartalmazó és az annál korábbi naplóállományokat. Ha ez sikeresen lezajlott, akkor az AEE a 9a. üzenetet küldi. Egyébként az AEE a 9b. üzenetet küldi, bontja a kapcsolatot és a folyamat sikertelenül zárul le. |

| 9a. | Az átszemélyesítés sikeres | ANS~XXXXXXXXX~12~HHHHHHHHHH | AEE→SSG |

| 9b. | Az átszemélyesítés sikertelen | ANS~XXXXXXXXX~40~HHHHHHHHHH | AEE→SSG |

| 10. | Blokkolást feloldó üzenet | UNBLCK~HHHHHHHHHH | SSG→AEE |

| 11. | Az AEE megkísérli feloldani a pénztárgép blokkolt állapotát. Sikeres végrehajtás esetén a 11a. üzenetet, sikertelen végrehajtás esetén az 11b. üzenetet küldi. |

| 11a. | Blokkolás feloldása végrehajtva | ANS~XXXXXXXXX~02~HHHHHHHHHH | AEE→SSG |

| 11b. | Blokkolás feloldás végrehajtása sikertelen | ANS~XXXXXXXXX~32~HHHHHHHHHH | AEE→SSG |

| 12. | A folyamat sikeres lezárásáról a NAV a 12a. üzenetet küldi, sikertelen lezárásáról a 12b. üzenetet küldi. |

| 12a. | Az átszemélyesítési folyamat sikeresen lezárult | ACK~07~HHHHHHHHHH | SSG→AEE |

| 12b. | Visszaigazolás a folyamat sikertelenségéről | ACK~00~HHHHHHHHHH | SSG→AEE |

| 13. | Az AEE bontja az SSL kapcsolatot |

## Az átszemélyesítés kizárólag akkor tekinthető sikeresen befejezettnek, ha sikeresen megtörtént minden olyan módosítás, amire a NAV utasítást adott, majd az AEE fogadta a 10a. lépésben szereplő visszaigazoló üzenetet. A pénztárgép adóügyi nap nyitását kizárólag a sikeresen lezárult üzembe helyezési folyamatot követően teheti lehetővé. Átszemélyesítés után a naplóállományok sorszámozása ismétlés és kihagyás nélkül folytatódik.

## Sikertelenül zárult átszemélyesítés újra megkísérelhető.

12. eset: Pénztárgép üzemeltetésének befejezése

A pénztárgép üzemeltetésének befejezése során az AEE-ben tárolt naplóállományok feltöltésre kerülnek a NAV szerverére és a NAV blokkolja a pénztárgép működését. Ebből az állapotból a pénztárgép üzemeltetésének folytatásával (16. eset) vagy új üzembe helyezéssel (11/b. eset) kerülhet ki a pénztárgép.

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE jelzi a kezelői szándékot a az üzemeltetés befejezési folyamat megindítására | SUSPEND~XXXXXXXXX | AEE→SSG |

| 3. | Amennyiben az üzemeltetés befejezése megvalósítható, a NAV a 3a. üzenetet küldi és a folyamat a 4. lépéssel folytatódik. Egyéb esetben a NAV az 5b. üzenetet küldi, ennek fogadását követően az AEE bontja a kapcsolatot és a folyamat sikertelenül zárul. |

| 3a. | Üzemeltetés befejezése lefolytatható | ACK~08~HHHHHHHHHH | SSG→AEE |

| 3b. | Üzemeltetés befejezése nem hajtható végre | ACK~60~HHHHHHHHHH | SSG→AEE |

| 4. | Normál bejelentkezés | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 5. | Blokkoló üzenet | PTGBLCK~HHHHHHHHHH | MSG→AEE |

| 6. | Az AEE megkísérli blokkolt állapotba hozni a pénztárgépet. Sikeres végrehajtás esetén a 6a. üzenetet küldi és a folyamat a 7. lépéssel folytatódik. Sikertelen végrehajtás esetén az AEE a 6b. üzenetet küldi, bontja az SSL kapcsolatot és a folyamat sikertelenül zárul. |

| 6a. | Blokkolás végrehajtva | ANS~XXXXXXXXX~01~HHHHHHHHHH | AEE→MSG |

| 6b. | Blokkolás végrehajtása sikertelen | ANS~XXXXXXXXX~31~HHHHHHHHHH | AEE→MSG |

| 7. | Utasítás adatszolgáltatásra | TRMNOW~F~HHHHHHHHHH | MSG→AEE |

| 8. | Az AEE lezárja az éppen nyitott naplóállományt és az „F” értéknél nagyobb sorszámú naplóállományokat egyesével, sorszám szerint növekvő sorrendben elküldi a 9-10. lépések megfelelő számú ismétlésével. |

| 9. | Naplófájl küldése | (fájlnév~HHHHHHHHHH) és tartalom | AEE→NFL |

| 10. | A naplófájl fogadását a NAV a 10a., a 10b. vagy a 10c. üzenettel nyugtázza. |

| 10a. | NAV visszaigazolás és utasítás a következő fájl küldésére | ACK~02~HHHHHHHHHH | NFL→AEE |

| 10b. | Az üzemeltetés befejezése nyugtázva | ACK~64~HHHHHHHHHH | NFL→AEE |

| 10c. | NAV hibajelzés | ACK~00~HHHHHHHHHH | NFL→AEE |

| 11. | A 10a. üzenet fogadása esetén az AEE a folyamatot a 9. lépéssel folytatja. A 10b. üzenet fogadása esetén az AEE bontja az SSL kapcsolatot és a folyamat sikeresen lezárult. A 10c. üzenet fogadása esetén az AEE újraküldi a 9. lépésben legutóbb küldött naplófájlt. Ha az AEE egy fájl küldése kapcsán ötödször is a 10c. üzenetet kapja, akkor a folyamat a 12. lépéssel folytatódik és sikertelenül zárul. |

| 12. | Sikertelen fájlküldés | ANS~XXXXXXXXX~37~HHHHHHHHHH | AEE→MSG |

| 13. | Üzemeltetés befejezési folyamat sikertelen | ACK~61~HHHHHHHHHH | MSG→AEE |

| 13. | Az AEE bontja az SSL kapcsolatot |

## Ha az üzemeltetés befejezése folyamat sikeresen lezárul, akkor újabb üzembe helyezésig, illetve az üzemeltetés folytatása folyamat lezárultáig a pénztárgép nem lehet alkalmas adóügyi nap megnyitására.

13. eset: Utasítás azonnali elsőbbségi bejelentkezésre

| Lépés | Leírás | Üzenet | Irány |

| 1. | A NAV azonnali elsőbbségi bejelentkezésre utasítja az AEE-t (nem SSL csatornán) | CMSSL~XXXXXXXXX | Mobilszolgáltató→AEE |

| 2. | Az AEE felépíti az SSL kapcsolatot |

| 3. | Az AEE bejelentkezése | PRIOR~07~XXXXXXXXX~S~N~T | AEE→MSG |

| A forgalmazás az e mellékletben részletezett forgatókönyvek egyike szerint folytatódik az egyik olyan üzenettel, amit az MSG szerver adhat az AEE elsőbbségi bejelentkezésére válaszul. |

14. eset: Működtető szoftver frissítése az AEE kezdeményezésére

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE szoftverfrissítést igényel | REQFW~V~XXXXXXXXX | AEE→SSG |

| 3. | Amennyiben a NAV a szoftver frissítésére kész, a 3a. üzenetet küldi és a folyamat az e mellékletben foglalt 9. eset 4. lépésével folytatódik. Ha a szoftver frissítése aktuálisan nem lehetséges, a NAV a 3b. üzenetet küldi. Ilyenkor a folyamat a 4. lépéssel folytatódik és sikertelenül zárul le. |

| 3a. | Utasítás a működtető szoftver frissítésére | FRWUPD~ééééhhnnóóppmm~HHHHHHHHHH | SSG→AEE |

| 3b. | Szoftver frissítése most nem lehetséges | ACK~05~HHHHHHHHHH | SSG→AEE |

| 4. | A 3a. üzenet fogadása esetén az AEE a forgalmazást az e melléklet 9. esetében foglaltak szerint folytatja. A 3b. üzenet fogadása esetén az AEE bontja az SSL kapcsolatot és 4 órán belül nem ismétli meg a REQFW kérést. |

15. eset: A NAV folyamatot töröl az AEE-n

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás egy vagy több folyamat törlésére | UPDCLR~XXXXXXXXX~R~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE végrehajtja az utasításban foglaltakat. Sikeres végrehajtás esetén a 4a. üzenetet, sikertelen végrehajtás esetén a 4b. üzenetet küldi. Ha a 3. lépésben szereplő üzenetben R=”ALL”, akkor a sikeres végrehajtást az összes utasítás sikeres végrehajtása jelenti. Ha a megjelölt folyamat nem létezik, akkor az AEE a 4c. üzenetet küldi. |

| 4a. | Alaphelyzetbe állítás végrehajtva | ANS~XXXXXXXXX~41~HHHHHHHHHH | AEE→MSG |

| 4b. | Alaphelyzetbe állítás sikertelen | ANS~XXXXXXXXX~42~HHHHHHHHHH | AEE→MSG |

| 4c. | Megjelölt folyamat nem létezik | ANS~XXXXXXXXX~53~HHHHHHHHHH | AEE→MSG |

| 5. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 6. | Az AEE bontja az SSL kapcsolatot. |

16. eset: Üzemeltetés folytatása

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Üzemeltetés folytatásának kezdeményezése | SUSPUNDO~XXXXXXXXX | AEE→SSG |

| 3. | Amennyiben az üzemeltetés folytatása megvalósítható, a NAV a 3a. üzenetet, egyébként a 3b. üzenetet küldi. A 3b. üzenet fogadása esetén az AEE bontja az SSL kapcsolatot és a folyamat sikertelenül zárul. |

| 3a. | Blokkolást feloldó üzenet | UNBLCK~HHHHHHHHHH | SSG→AEE |

| 3b. | Üzemeltetés folytatása nem lehetséges | ACK~65~HHHHHHHHHH | SSG→AEE |

| 4. | Az AEE megkísérli feloldani a pénztárgép blokkolt állapotát. Sikeres végrehajtás esetén a 4a. üzenetet, sikertelen végrehajtás esetén a 4b. üzenetet küldi. |

| 4a. | Blokkolás feloldása végrehajtva | ANS~XXXXXXXXX~02~HHHHHHHHHH | AEE→SSG |

| 4b. | Blokkolás feloldás végrehajtása sikertelen | ANS~XXXXXXXXX~32~HHHHHHHHHH | AEE→SSG |

| 5. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | SSG→AEE |

## A sikertelenül zárult folyamat megismételhető.

17. eset: Utasítás a naplófájl maximális méretének beállítására

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás a maximális méret beállítására | FILESIZE~XXXXXXXXX~N~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE megkísérli a méretkorlát beállítását. Sikeres végrehajtás esetén az 5a. üzenetet, sikertelen végrehajtás esetén az 5b. üzenetet küldi. |

| 5a. | Méretkorlát beállítás végrehajtva | ANS~XXXXXXXXX~14~HHHHHHHHHH | AEE→MSG |

| 5b. | Méretkorlát beállítás sikertelen | ANS~XXXXXXXXX~44~HHHHHHHHHH | AEE→MSG |

| 6. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 7. | Az AEE bontja az SSL kapcsolatot |

18. eset: Utasítás technikai tájékoztatás bizonylat nyomtatására

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás üzenet nyomtatására | PRNT~XXXXXXXXX~SZOVEG~HHHHHHHHHH | MSG→AEE |

| 4. | Az AEE az üzenet szövegét eltárolja későbbi kinyomtatáshoz. Sikeres eltárolás esetén az 5a. üzenetet, sikertelen eltárolás esetén az 5b. üzenetet küldi. |

| 5a. | Nyomtatás végrehajtva | ANS~XXXXXXXXX~45~HHHHHHHHHH | AEE→MSG |

| 5b. | Nyomtatás végrehajtása sikertelen | ANS~XXXXXXXXX~46~HHHHHHHHH | AEE→MSG |

| 6. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 7. | Az AEE bontja az SSL kapcsolatot |

## A technikai tájékoztatás bizonylat nem adóügyi bizonylat.

19. eset: Az AEE-NAV kommunikáció tesztelése

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PING~XXXXXXXXXX | AEE→MSG |

| 3. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 4. | A pénztárgép operátori kijelzőjén megjelenik a „Kommunikációs csatorna él” felirat, majd 60 másodperc múlva az AEE bontja az SSL kapcsolatot. |

[^192]: Az 5. melléklet a 9/2016. (III. 25.) NGM rendelet 36. § f) pontjával megállapított szöveg.
