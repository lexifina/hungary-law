# A belügyminiszter 24/2004. (VI. 11.) BM rendelete

Magyar Közlöny 2004. évi 80. szám, 2004. június 11. · [hiteles PDF](https://magyarkozlony.hu/hivatalos-lapok/d0da2ead5fa230811313974a24bb8aaa2ffd3c94/dokumentumok/48a9f7523f9258435c23aee2300e53eeaf585cd4/letoltes)

---

A belügyminiszter
24/2004. (VI. 11.) BM
rendelete
a közszolgálati nyilvántartás egyes kérdéseiről szóló
7/2004. (III. 2.) BM rendelet módosításáról
A közszolgálati jogviszonnyal összefüggő adatkezelés-
re és a közszolgálati nyilvántartásra vonatkozó szabályok-
ról szóló 233/2001. (XII. 1.) Korm. rendelet 27. § b) pont-
jában foglalt felhatalmazás alapján a következőket rende-
lem el:
1. §
A közszolgálati nyilvántartás egyes kérdéseiről szóló
7/2004. (III. 2.) BM rendelet 2. számú melléklete e ren-
delet melléklete szerinti függelékkel egészül ki.
2. §
Ez a rendelet a kihirdetése napján lép hatályba.
Dr. Lamperth Mónika s. k.,
belügyminiszter
Melléklet
a 24/2004. (VI. 11.) BM rendelethez
[7/2004. (III. 2.) BM rendelet
2. számú függelék a 2. számú melléklethez]
Állományformátum a központi
közszolgálati nyilvántartás részére történő
adat és adatváltozás jelentésére
Az állományformátum célja
Az állományformátum meghatározása azt a célt szolgál-
ja, hogy a számítástechnikai eszközökkel vezetett közszol-
gálati alapnyilvántartásokból elektronikus adathordozón
keresztül, adatlap közbeiktatása nélkül lehessen adatokat
szolgáltatni a központi közszolgálati nyilvántartás részére.
1. Az állomány általános leírása
Az állomány adattartalmára, valamint a kódszótárakra
vonatkozóan az Adatlap kitöltési útmutatója az irányadó.
Az állomány szöveg formátumú (txt file), azaz bármely
egyszerű szövegszerkesztő program segítségével olvas-
ható.
Az állományok feltöltésére az MSZ 7795–3 szabvány
szerinti ASCII (szabványos ASCII 0–127-ig), illetve
ASCII/PC (852-es) vagy pedig a CWI karakterkód készle-
tek használhatók.
Az állomány rekordokból tevődik össze, az egyes rekor-
dok hézag, elválasztó jel nélkül követik egymást.
Az első rekord az állományra vonatkozó kísérő in-
formációkat tartalmazza (azonosító rekord), további re-
kordjai az Adatlap egyes lapjainak felelnek meg (adatre-
kordok), s a KÖZIGTAD-ba jelentett adatokat tartal-
mazzák.
Az adatváltozásokat tartalmazó rekordok (adatrekor-
dok) első hat mezője (adatrekord fejrésze) azonos szerke-
zetű minden rekord esetében, és az adott adatrekordot egy-
értelműen azonosító információkat tartalmazza.
A rekordok mezőkből épülnek fel. A mezők – és ezen
keresztül a rekordok – mérete az aktuális kitöltöttségtől
függetlenül, de a lap típusától függően állandó (fix rekord-
szerkezet). Az üres mezőket a szóközzel kell feltölteni. A
mezőkben szereplő számokat balról nullákkal kell feltölte-
ni. A mezőkben szereplő szövegek elhelyezése balra iga-
zítva, a végén szóközzel (jelölése: ~) feltöltve történik.
Minden rekord háromjegyű sorszámmal kezdődik,
amely az állomány első, kísérő információkat tartalmazó
rekordja (azonosító rekord) esetén 000, majd egyesével fo-
lyamatosan növekszik. A rekordsorszám három jegyen tá-
rolódik. A rekordsorszámok a rekordoknak csak az adott
állományon belüli sorrendjét határozzák meg, egyéb jelen-
téssel nem bírnak.
Egy adatállományban tetszőleges darabszámú adatre-
kord szerepelhet. A 999. sorszámú adatrekord után a 000.
sorszámmal egy új adatrekord következik.
Egy technikai azonosítóhoz tartozó lapoknak (adatre-
kordoknak) egy adatállományon belül kell szerepelniük.
Az adatváltozásokat hordozó rekordok tartalmuktól
függetlenül, tetszőleges sorrendben követhetik egymást
(de a feldolgozás hatékonyságának növelése érdekében az
egyes technikai azonosítóhoz tartozó rekordok egymás
után szerepeltetése célszerű).
Az egyes rekordokat a „kocsivissza” (hex0D) és a
„soremelés” (hex0A), az állományt pedig a „file vége”
(hex1A) kódok zárják le.
Az adatváltozásokat tartalmazó rekordok első hat adat-
csoportja azonos szerkezetű és a rekordot egyértelműen
azonosító információkat tartalmazza.
Az első adatcsoport egyetlen mezőből áll, mely a már
említett állományon belüli sorszámot tartalmazza.
A második adatcsoport egyetlen ún. rekord állapot jelző
számból áll, mely 0 vagy 1 vagy 8 lehet. A 0 azt jelzi; hogy
a rekordban található adatokat az első alkalommal jelentik
a központi közszolgálati nyilvántartás számára, azaz az

adott technikai azonosítót és lapsorszámot tartalmazó re-
kordot eddig még nem küldtek.
Ha a jelző értéke 1, az arra utal, hogy a rekordban talál-
ható adatokat egy előzőleg küldött adatváltozás-jelentő re-
kord javításaként küldik a központi közszolgálati nyilván-
tartás részére. Ebben az esetben a technikai azonosító és a
lapsorszám kötelezően megegyezik a javítandó rekord
technikai azonosítójával és lapsorszámával.
Ha egy korábban elküldött rekord törlése válik szüksé-
gessé, a jelző értékét 8-ra kell állítani. Ebben az esetben a
technikai azonosítón a kitöltés időpontján és a lap sorszá-
mán kívül egyéb adatot nem tartalmazhat a rekord.
A harmadik adatcsoportot szintén egy mező alkotja,
amely annak a személynek a technikai azonosítóját tartal-
mazza, akinek az adatai a rekordban találhatók.
A negyedik adatcsoport azt a kitöltési időpontot tartal-
mazza, amikor a rekordban található adatokat a közszolgá-
lati alapnyilvántartásba felvették. Ez az időpont az Adatla-
pon vezetett közszolgálati alapnyilvántartás „a kitöltés
időpontja” adatának megfelelője. Az adatcsoport az év,
hónap és nap mezőkből áll.
Az ötödik adatcsoport a rekordban közölt információk
jellegére utal, a hatodik mező pedig egy sorszámot tartal-
maz, mely megmondja, hogy az adott személyről ilyen jel-
legű adatváltozást hányadik alkalommal vettek fel a köz-
szolgálati alapnyilvántartásba. Ez az adatcsoport az adat-
lapon a lap sorszámának felel meg.
2. Az állomány neve
Az állomány azonosító neve nyolc, a név kiterjesztése
pedig három karakterből áll.
A név első hat karaktere az adatokat küldő szerv azono-
sító száma, mely megegyezik az Adatlapon a technikai
azonosító első hat jegyével.
Az utolsó két karakter annak az évszámnak az utolsó két
jegyével egyezik meg, amely évben az állományt létrehoz-
ták.
A kiterjesztés az adott évben az adott szerv által elkészí-
tett adatjelentő állományok sorszámát tartalmazza. Az első
állomány sorszáma 001, a következőké pedig folyamato-
san egyesével növekszik.
3. Az adatállományban szereplő rekordok leírása
A következő táblázatok az alábbi oszlopokból épülnek
fel:
ID: az adott rekordon belül a mező azonosítására szol-
gáló mező
A mező rövid megnevezése: az adott rekord mezőjének
rövid megnevezése
Típus: az adatmező típusát jelzi az alábbiak szerint:
– ’N’ – numerikus
– ’AN’ – alfanumerikus
– ’D’ – dátum típusú
Mezőméret: az adatmezőt alkotó karakterek száma.
Leírás: az adatmező tartalma.

3.1. Kísérő információk rekordleírása (azonosító rekord)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord sorszáma.
A mező tartalma kizárólag ’000’ lehet.
2. Karakter-kódkészlet AN 8 byte,
fix
Az alkalmazott karakter-kódkészlet neve.
Lehetséges értékei:
g ’ASCII ~~~’
g ’ASCII/PC ~~~~~’
g ’CWI ~~~~~’
3. Előállító program neve AN* 26 byte,
fix
Az állományt előállító program neve.
4. Előállító személy neve AN* 26 byte,
fix
Az állományt előállító személy neve.
5. Technikai mező AN* 48 byte,
fix
Az állományt előállító rendszer tetszés szerint használhatja.
6. Adatszolgáltatási időszak N 6 byte,
fix
Az adatszolgáltatás időszaka.
Formátuma: ’ééééhh’
7. Változott rekordok száma N 5 byte,
fix
A küldött adatváltozást tartalmazó rekordok összes száma az állományban.
8. Először küldött rekordok száma N 5 byte,
fix
Az összes változott rekordból az először küldött rekordok száma.
9. Javító rekordok száma N 5 byte,
fix
Az összes változott rekordból a javító rekordok száma.
10. Megjegyzés AN* 252 byte,
fix
Szabadon felhasználható mező.
A *-gal jelölt mezők tetszőleges tartalmúak lehetnek, a balra igazítás ezekben a mezőkben nem kötelező.

3.2. Legmagasabb iskolai végzettség, továbbá szakirányú továbbképzésben szerzett végzettség adatai („I” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ’ééééhhnn’
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’I~~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Bizonyítvány kelte AN 4 byte,
fix
A végzettséget igazoló oklevél, bizonyítvány kelte.
Formátuma: ’éééé’
8. Végzettség kódja AN 5 byte,
fix
A végzettség kódja.
Az első 2 karakter a végzettség szintjét, a 3–5. karakter a végzettség szakirányát
jelöli.
3.3. Iskolarendszeren kívüli oktatás keretében szerzett szakképesítés, meghatározott munkakör betöltésére jogosító ok-
irat adatai („S” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’S~~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Szakképesítés kódja N 3 byte,
fix
A szakképesítés megnevezésének kódja. A mező 1–2. karakterei a szakképesítés
szintjét és jellegét, a 3. karaktere a szakképesítés szakirányát, illetve e szakirány
jellegét jelzik.
8. Okirat kelte N 4 byte,
fix
Az okirat kelte.
Formátuma: ’éééé’

3.4. Tudományos fokozat adatai („T” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám
N
3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző
N
1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító
N
11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja
D
8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel
AN
4 byte,
fix
A lap jele. Tartalma: ’T~~~’
6. Sorszám
N
2 byte,
fix
A lap sorszáma.
7. Tudományos fokozat kódja
N
1 byte,
fix
A tudományos fokozat szintjének kódja.
8. Okirat kelte
N
4 byte,
fix
Az igazoló okirat kelte.
Formátuma: ’éééé’.
3.5. Idegennyelv-ismeret adatai („N” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’N’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Idegen nyelv kódja AN 2 byte,
fix
Az idegen nyelv kódja.
8. Nyelvvizsga-fokozat kódja AN 2 byte,
fix
Az állami nyelvvizsga fokozatának kódja. A kód első karaktere a nyelvvizsga fo-
kozatának kódja, a második karaktere a nyelvvizsga típusának kódja.
9. Okirat kelte AN 4 byte,
fix
Az igazoló okirat kelte.
Formátuma: ’éééé’
10. Pótlék-jogosultság AN 1 byte,
fix
Idegennyelv-tudási pótlékra jogosult-e.

3.6. Közigazgatási vizsga adatai („V” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’V~~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Vizsgakötelezettség kódja N 1 byte,
fix
A vizsgakötelezettség megnevezésének kódja.
8. Vizsga határideje D 8 byte,
fix
A vizsga letételének határideje.
Formátuma: ééééhhnn
9. Vizsga időpontja N 4 byte,
fix
A vizsga tervezett időpontja.
Formátuma: ’éééé’
10. Vizsgaidőszak kódja N 2 byte,
fix
A vizsga tervezett időpontjának (hónap) kódja.
11. Vizsgáztató szerv kódja N 2 byte,
fix
A vizsgáztatásra jogosult szerv kódja.
3.7. Közigazgatási vizsga letételének adatai („VL” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’VL~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Vizsga típusa N 1 byte,
fix
A vizsga típusa.
8. Bizonyítvány kelte D 8 byte,
fix
A bizonyítvány kelte dátum.
Formátuma: ’ééééhhnn’

3.8. Közszolgálati jogviszony tartalmára vonatkozó adatok („J” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’J~~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Közszolgálati jogviszony kez-
dete
D 8 byte,
fix
A közszolgálati jogviszonyban töltött idő számítása alapján a közszolgálati jogvi-
szony kezdete.
Formátuma: ’ééééhhnn’
8. Közszolgálati jogviszony idő-
tartama
N 6 byte,
fix
A közszolgálati jogviszonyban töltött idő számítása alapján a közszolgálati jogvi-
szony időtartama.
Formátuma: ’ééhhnn’
9. Kinevezés időpontja D 8 byte,
fix
Határozatlan időre szóló kinevezés esetén a kinevezés időpontja.
Formátuma: ’ééééhhnn’
10. Kinevezés kódja N 3 byte,
fix
Határozatlan időre szóló kinevezés esetén a kinevezés kódja.
11. Kinevezéshez kapcsolódó mun-
kaidő heti óraszáma
N 2 byte,
fix
Határozatlan időre szóló kinevezés esetén a heti munkaidő óraszáma.
12. Kinevezéshez kapcsolódó mun-
kaidő kódja
N 1 byte,
fix
Határozatlan időre szóló kinevezés esetén a heti munkaidő kódja.
13. Jogviszony kezdetének idő-
pontja
D 8 byte,
fix
Határozott időre szóló kinevezés esetén a közszolgálati jogviszony időtartamának
kezdete.
Formátuma: ’ééééhhnn’.
14. Jogviszony végének időpontja D 8 byte,
fix
Határozott időre szóló kinevezés esetén a közszolgálati jogviszony időtartamának
vége.
Formátuma: ’ééééhhnn’
15. Jogviszony kódja N 3 byte,
fix
Határozott időre szóló kinevezés esetén a közszolgálati jogviszony kódja.
16. Jogviszonyhoz kapcsolódó
munkaidő heti óraszáma
N 2 byte,
fix
Határozott időre szóló kinevezés esetén a heti munkaidő óraszáma.
17. Jogviszonyhoz kapcsolódó
munkaidő kódja
N 1 byte,
fix
Határozott időre szóló kinevezés esetén a heti munkaidő kódja.
18. Módosítás időpontja D 8 byte,
fix
Határozott időre szóló kinevezés határozatlan időre történő módosításának idő-
pontja.
Formátuma: ’ééééhhnn’
19. Módosítás kódja N 3 byte,
fix
Határozott időre szóló kinevezés határozatlan időre történő módosításának kódja.
20. Módosításhoz kapcsolódó mun-
kaidő heti óraszáma
N 2 byte,
fix
Határozott időre szóló kinevezés határozatlan időre történő módosítása esetén a
heti munkaidő óraszáma.
21. Módosításhoz kapcsolódó mun-
kaidő kódja
N 1 byte,
fix
Határozott időre szóló kinevezés határozatlan időre történő módosítása esetén a
heti munkaidő kódja.
22. Helyettes jegyzői kinevezés tar-
tama -tól
D 8 byte,
fix
Határozott időre szóló jegyzői kinevezés tartamának kezdete helyettesítés céljá-
ból.
Formátuma: ’ééééhhnn’
23. Helyettes jegyzői kinevezés tar-
tama -ig
D 8 byte,
fix
Határozott időre szóló jegyzői kinevezés tartamának vége helyettesítés céljából.
Formátuma: ’ééééhhnn’.
24. Helyettes jegyzői kinevezés
kódja
N 3 byte,
fix
Határozott időre szóló jegyzői kinevezés kódja helyettesítés céljából.

ID A mező rövid megnevezése Típus Mezőméret Leírás
25. Helyettes jegyzői kinevezéshez
kapcsolódó munkaidő heti óra-
száma
N 2 byte,
fix
Határozott időre szóló jegyzői kinevezés esetén a heti munkaidő óraszáma.
26. Helyettes jegyzői kinevezéshez
kapcsolódó munkaidő kódja
N 1 byte,
fix
Határozott időre szóló jegyzői kinevezés esetén a heti munkaidő kódja.
27. Határozott idejű áthelyezés idő-
tartama -tól
D 8 byte,
fix
Közigazgatási szervtől határozott időre történő áthelyezés kezdete.
Formátuma: ’ééééhhnn’
28. Határozott idejű áthelyezés idő-
tartama -ig
D 8 byte,
fix
Közigazgatási szervtől határozott időre történő áthelyezés vége.
Formátuma: ’ééééhhnn’
29. Határozott idejű áthelyezés
kódja
N 3 byte,
fix
Közigazgatási szervtől határozott időre történő áthelyezés kódja.
30. Határozott idejű áthelyezéshez
kapcsolódó munkaidő heti óra-
száma
N 2 byte,
fix
Közigazgatási szervtől határozott időre történő áthelyezés esetén a heti munkaidő
óraszáma.
31. Határozott idejű áthelyezéshez
kapcsolódó munkaidő kódja
N 1 byte,
fix
Közigazgatási szervtől határozott időre történő áthelyezés esetén a heti munkaidő
kódja.
32. Végleges áthelyezés időpontja D 8 byte,
fix
Végleges közigazgatási áthelyezés időpontja.
Formátuma: ’ééééhhnn’
33. Végleges áthelyezés kódja N 3 byte,
fix
Végleges közigazgatási áthelyezés kódja.
34. Végleges áthelyezéshez kapcso-
lódó munkaidő heti óraszáma
N 2 byte,
fix
Végleges közigazgatási áthelyezés esetén a heti munkaidő óraszáma.
35. Végleges áthelyezéshez kapcso-
lódó munkaidő kódja
N 1 byte,
fix
Végleges közigazgatási áthelyezés esetén a heti munkaidő kódja.
36. Áthelyezés időpontja D 8 byte,
fix
Más foglalkoztatási jogviszonyból történő áthelyezés időpontja.
Formátuma: ’ééééhhnn’
37. Áthelyezés kódja N 3 byte,
fix
Más foglalkoztatási jogviszonyból történő áthelyezés kódja.
38. Áthelyezéshez kapcsolódó
munkaidő heti óraszáma
N 2 byte,
fix
Más foglalkoztatási jogviszonyból történő áthelyezés esetén a heti munkaidő óra-
száma.
39. Áthelyezéshez kapcsolódó
munkaidő kódja
N 1 byte,
fix
Más foglalkoztatási jogviszonyból történő áthelyezés esetén a heti munkaidő
kódja.
40. Adományozás kódja N 3 byte,
fix
Az adományozott cím kódja.
41. Adományozás időpontja D 8 byte,
fix
Az adományozott cím adományozásának időpontja.
Formátuma: ’ééééhhnn’
42. Adományozás visszavonásának
dátuma
D 8 byte,
fix
Az adományozott cím visszavonásának időpontja.
Formátuma: ééééhhnn
43. Születési dátum D 8 byte,
fix
A közszolgálati jogviszonyban álló személy születésének időpontja.
Formátuma: ’ééééhhnn’
44. Nemkód N 1 byte,
fix
A közszolgálati jogviszonyban álló személy nemének kódja.
45. Jutalmak éve (25 éves) N 4 byte,
fix
A jubileumi jutalmak esedékességének éve (25 éves).
Formátuma: ’éééé’
46. Jutalmak éve (30 éves) N 4 byte,
fix
A jubileumi jutalmak esedékességének éve (30 éves).
Formátuma: ’éééé’
47. Jutalmak éve (35 éves) N 4 byte,
fix
A jubileumi jutalmak esedékességének éve (35 éves).
Formátuma: ’éééé’
48. Jutalmak éve (40 éves) N 4 byte,
fix
A jubileumi jutalmak esedékességének éve (40 éves).
Formátuma: ’éééé’

3.9. Besorolás adatai („B” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’B~~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Besorolási osztály N 1 byte,
fix
Besorolási osztály kódja.
8. Besorolási fokozat N 2 byte,
fix
Besorolási fokozat.
9. Pályaszakasz kezdete D 8 byte,
fix
Pályaszakasz kezdete.
Formátuma: ’ééééhhnn’
10. Besorolási alap kódja N 2 byte,
fix
A besorolási fokozatba kerülés alapjának kódja.
11. Következő fokozatba lépés
dátuma
D 8 byte,
fix
A következő besorolási fokozatba előírt várakozási idő lejárta.
Formátuma: ééééhhnn
3.10. A képzés, továbbképzés, vezetőképzés, átképzés (együtt: továbbképzés) adatai („TK” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’TK~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Továbbképzés kezdete D 8 byte,
fix
A továbbképzés kezdetének dátuma.
Formátuma: ’ééééhhnn’
8. Továbbképzés vége D 8 byte,
fix
A továbbképzés befejezésének dátuma.
Formátuma: ’ééééhhnn’
9. Továbbképzés időtartama N 4 byte,
fix
A továbbképzés időtartama órákban.
10. Továbbképzés jellege N 4 byte,
fix
A továbbképzés jellege.
11. Szervező intézmény N 4 byte,
fix
A továbbképzést szervező intézmény neve.
12. Továbbképzés típusa N 4 byte,
fix
A továbbképzés típusa.

ID A mező rövid megnevezése Típus Mezőméret Leírás
13. Továbbképzés témája N 4 byte,
fix
A továbbképzés tartalma és témája.
14. Továbbképzés költségtérítésé-
nek összege
N 7 byte,
fix
A továbbképzéshez biztosított költségtérítés összege.
15. Tanulmányi támogatás összege N 7 byte,
fix
Tanulmányi szerződés alapján nyújtott támogatás.
16. Költségtérítés forrása N 4 byte,
fix
A költségtérítés forrása.
3.11. Vezetőre vonatkozó adatok („VEZ” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’VEZ~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Vezető megnevezésének kódja N 3 byte,
fix
A kód két részből áll. Az első 2 karakter a vezetői kinevezés, illetve vezetői meg-
bízás megnevezésének kódja. A 3. karakter kizárólag jegyzők esetében töltendő,
a település lakosságszámát mutatják.
8. Vezető kinevezésének ideje D 8 byte,
fix
A vezetői kinevezés, illetve vezetői megbízás kezdetének dátuma.
Formátuma: ééééhhnn
3.12. A vezetői kinevezés, illetve vezetői megbízás megszűnésének adatai („VEZM” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’VEZM’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Megszűnés időpontja D 8 byte,
fix
A vezetői kinevezés, illetve vezetői megbízás megszűnésének dátuma.
Formátuma: ’ééééhhnn’
8. Megszűnés módja N 2 byte,
fix
A vezetői kinevezés, illetve vezetői megbízás megszűnésének módja.

3.13. Tartós távollét adatai („TAR” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’TAR~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Tartós távollét kódja N 2 byte,
fix
A tartós távollét jogcímének kódja.
8. Tartós távollét kezdete D 8 byte,
fix
A tartós távollét időtartamának kezdete.
Formátuma: ’ééééhhnn’
9. Tartós távollét vége D 8 byte,
fix
A tartós távollét megszűnésének várható időpontja.
Formátuma: ’ééééhhnn’
3.14. Tartós távollét megszűnésének adatai („TARM” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’TARM’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Tartós távollét megszűnésének
dátuma
D 8 byte,
fix
A tartós távollét megszűnésének időpontja.
Formátuma: ééééhhnn
3.15. Áthelyezés, illetve a közszolgálati jogviszony megszűnésének adatai („JV” adatlap)
ID A mező rövid megnevezése Típus Mezőméret Leírás
1. Rekordsorszám N 3 byte,
fix
A rekord állományon belüli sorszáma.
2. Állapotjelző N 1 byte,
fix
A rekord állapotát jelző szám. Lehetséges értékei:
g ’0’– új bejegyzés
g ’1’– módosítás
g ’8’– törlés

ID A mező rövid megnevezése Típus Mezőméret Leírás
3. Technikai azonosító N 11 byte,
fix
Személy technikai azonosítója.
4. Kitöltés időpontja D 8 byte,
fix
A lap kitöltésének dátuma.
Formátuma: ééééhhnn
5. Lapjel AN 4 byte,
fix
A lap jele. Tartalma: ’JV~~’
6. Sorszám N 2 byte,
fix
A lap sorszáma.
7. Visszahelyezés dátuma D 8 byte,
fix
A visszahelyezés időpontja határozott idejű áthelyezésből.
Formátuma: ’ééééhhnn’
8. Visszahelyezés kódja N 3 byte,
fix
A visszahelyezés kódja határozott idejű áthelyezésből.
9. Határozott idejű áthelyezés kez-
dete
D 8 byte,
fix
Közigazgatási szervhez határozott időre történő áthelyezés kezdete.
Formátuma: ’ééééhhnn’
10. Határozott idejű áthelyezés
vége
D 8 byte,
fix
Közigazgatási szervhez határozott időre történő áthelyezés vége.
Formátuma: ’ééééhhnn’
11. Határozott idejű áthelyezés
kódja
N 3 byte,
fix
Közigazgatási szervhez határozott időre történő áthelyezés kódja.
12. Fogadó szerv kódja N 3 byte,
fix
Közigazgatási szervhez határozott időre történő áthelyezés esetén a fogadó köz-
igazgatási szerv kódja.
13. Végleges áthelyezés időpontja D 8 byte,
fix
A végleges közigazgatási áthelyezés időpontja.
Formátuma: ’ééééhhnn’
14. Végleges áthelyezés kódja N 3 byte,
fix
A végleges közigazgatási áthelyezés kódja.
15. Végleges fogadó szerv kódja N 3 byte,
fix
Végleges közigazgatási áthelyezés esetén a fogadó szerv kódja.
16. Más jogszabály alá tartozó
szervhez történő áthelyezés idő-
pontja
D 8 byte,
fix
Más foglalkoztatási jogviszonyra vonatkozó jogszabály hatálya alá tartozó szerv-
hez történő áthelyezés időpontja.
Formátuma: ’ééééhhnn’
17. Más jogszabály alá tartozó
szervhez történő áthelyezés
kódja
N 3 byte,
fix
Más foglalkoztatási jogviszonyra vonatkozó jogszabály hatálya alá tartozó szerv-
hez történő áthelyezés kódja.
18. Más jogszabály alá tartozó
szerv kódja
N 3 byte,
fix
Más foglalkoztatási jogviszonyra vonatkozó jogszabály hatálya alá tartozó szerv-
hez történő áthelyezés esetén a fogadó költségvetési intézmény kódja.
19. Megszűnés időpontja D 8 byte,
fix
A közszolgálati jogviszony vagy főtisztviselői kinevezés megszűnésének idő-
pontja.
Formátuma: ’ééééhhnn’
20. Megszűnés módja N 3 byte,
fix
A közszolgálati jogviszony vagy főtisztviselői kinevezés megszűnésének módja.
21. Jogviszony időtartama végki-
elégítéshez
N 6 byte,
fix
A végkielégítés mértékének meghatározásához figyelembe vehető közszolgálati
jogviszony időtartama.
Formátuma: ’ééhhnn’
22. Végkielégítés időpontja D 8 byte,
fix
A végkielégítés kifizetésének időpontja.
Formátuma: ’ééééhhnn’
23. Végkielégítés mértéke N 2 byte,
fix
A végkielégítés kifizetésének mértéke.
24. Végkielégítés összege N 8 byte,
fix
A végkielégítés kifizetésének összege Ft-ban.
’’
