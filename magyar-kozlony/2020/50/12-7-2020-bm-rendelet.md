# A belügyminiszter 7/2020. (III. 20.) BM rendelete

Magyar Közlöny 2020. évi 50. szám, 2020. március 20. · [hiteles PDF](https://magyarkozlony.hu/hivatalos-lapok/5EaGg5VyQbxnPJbnmsnz5e6fd6d3336c2/dokumentumok/ab5e8de541d3a18f38001ca64b3234909e1a60a8/letoltes)

---

A belügyminiszter 7/2020. (III. 20.) BM rendelete
az egységes elektronikuskártya-kibocsátási keretrendszerről szóló 2014. évi LXXXIII. törvény
végrehajtásához szükséges kapcsolódási, műszaki, technológiai, biztonsági előírásokról, követelményekről
és a hitelesítési rendről szóló 53/2015. (IX. 24.) BM rendelet módosításáról
Az egységes elektronikuskártya-kibocsátási keretrendszerről szóló 2014. évi LXXXIII. törvény 21. § (2) bekezdés b) pontjában
kapott felhatalmazás alapján, a Kormány tagjainak feladat- és hatásköréről szóló 94/2018. (V. 22.) Korm. rendelet 40. §
(1) bekezdés 3. pontjában meghatározott feladatkörömben eljárva a következőket rendelem el:
1. §
Az egységes elektronikuskártya-kibocsátási keretrendszerről szóló 2014. évi LXXXIII. törvény végrehajtásához
szükséges kapcsolódási, műszaki, technológiai, biztonsági előírásokról, követelményekről és a hitelesítési rendről
szóló 53/2015. (IX. 24.) BM rendelet [a továbbiakban: 53/2015. (IX. 24.) BM rendelet] 11. alcíme a következő 53. §-sal
egészül ki:
„53. § (1) A kártya elektronikus olvasásának műszaki és biztonsági követelményeit a 6. melléklet határozza meg.
(2) A kártya elektronikus olvasására jogosult a 6. mellékletben meghatározott követelmények szerint köteles eljárni.”
2. §
Az 53/2015. (IX. 24.) BM rendelet az 1. melléklet szerinti 6. melléklettel egészül ki.
3. §
Ez a rendelet a kihirdetését követő napon lép hatályba.
4. §
E rendelet tervezetének a műszaki szabályokkal és az információs társadalom szolgáltatásaira vonatkozó
szabályokkal kapcsolatos információszolgáltatási eljárás megállapításáról szóló, 2015. szeptember 9-i (EU)
2015/1535 európai parlamenti és tanácsi irányelv 5–7. cikke szerinti előzetes bejelentése megtörtént.
 Dr. Pintér Sándor s. k.,
 belügyminiszter
1. melléklet a 7/2020. (III. 20.) BM rendelethez
„6. melléklet az 53/2015. (IX. 24.) BM rendelethez
A kártya elektronikus olvasásának műszaki és biztonsági követelményei
1. A kártyaelfogadó terminállal szembeni követelmények
1.1. A kártyaelfogadó terminál összetevői:
1.1.1. RFID kártyaolvasó,
1.1.2. kulcsok tárolását és a kriptográfiai műveleteket végző biztonsági hardver elem (a továbbiakban:
SAM),
1.1.3. kártyaolvasót és az SAM-et vezérlő szoftver vagy hardver modul, és
1.1.4. opcionálisan hálózati kommunikációt megvalósító komponens.
1.2. A kártyaelfogadó terminál kötelező jellemzői:
1.2.1. Az RFID kártyaolvasó proximity kártyák kezelésére alkalmas kártyaolvasó egység, illetve
mobileszköz, amely alkalmas – a 3. mellékletben foglaltaknak megfelelően – az adat elektronikus
hordozására képes eszközzel való biztonságos együttműködésre.
1.2.2. Az SAM
1.2.2.1. tárolja és kezeli a 128 bites AES kulcsokat,
1.2.2.2. garantálja, hogy a tárolt kulcs ne legyen megismerhető,
1.2.2.3. képes a 3. mellékletben meghatározott követelményeknek megfelelő kártyákkal történő
autentikációra, kulcsdiverzifikációra és az adatok olvasására az általa kezelt kulcsok
segítségével,
1.2.2.4. beépített védelemmel rendelkezik az illetéktelen felhasználás megakadályozására, és
1.2.2.5. támogatja a tárolt kulcsok utólagos biztonságos frissítését.

1.2.3. A vezérlő modul
1.2.3.1. vezérli a kártyaelfogadás teljes folyamatát, amelynek során párhuzamos kapcsolatot tart
fenn a kártyaolvasóval és az SAM-mel, valamint opcionálisan a hálózati komponenssel,
1.2.3.2. a sértetlenség és hitelesség igazolására opcionálisan képes az SHA256, valamint az ECC
algoritmusok használatára.
1.2.4. A hálózati kommunikációs komponens – ha a működtető vagy a kártyakibocsátó nyilvántartása
felé kommunikációt kezdeményez – alkalmas a távoli szerverek közötti biztonságos, hitelesített és
rejtjelezett kommunikációra.
2. A biztonsági hardver elem igénylésének, nyilvántartásának és kezelésének szabályai
2.1. A kártyaelfogadó az SAM-re vonatkozó igényt a működtetőhöz nyújtja be a működtető által biztosított
igénylőlap használatával.
2.2. A működtető az üzemeltető útján gondoskodik a terminálnak az SAM kártyaelfogadó által kezelhető
kulcsokkal történő felprogramozásáról, egyedi azonosítóval való ellátásáról és opcionálisan elfogadó-
specifikus speciális kulcsok átadásáról. A működtető nyilvántartja a felprogramozott SAM-eket, azok
nyilvántartási állapotát, az azokon tárolt kulcsokat és a rajtuk végzett műveleteket, biztosítja a kezelt
kártyatípus frissített kulcskészletének elérését. Az SAM igénylés állapota lehet nyitott, ellenőrzés alatt,
jóváhagyott, gyártásra átadott, lezárt és törölt.
2.3. A működtető a honlapján teszi közzé az SAM-re vonatkozó tájékoztató listaárat. Az SAM rendelkezésre
bocsátása és megszemélyesítése térítés ellenében történik, amelynek végleges díját az üzemeltetővel kötött
szerződés határozza meg.
2.4. A működtető az SAM-eket a kártyaelfogadónak a hiánytalan és hibátlan igénylés beérkezésétől számított
90 napon belül adja át, amely határidőbe az üzemeltető által lefolytatott közbeszerzési eljárás időtartama
nem számít be.
2.5. Tesztelési célból szervezetenként legfeljebb 10 db SAM igényelhető, aminek szükségességét az igénylőlapon
indokolva kell igazolni.
2.6. A felprogramozott SAM a kártyaelfogadó tulajdonába kerül, azonban azt sem használatba, sem tulajdonba
nem adhatja át harmadik félnek a működtető előzetes, írásbeli hozzájárulása nélkül.
2.7. A kártyaelfogadó köteles az általa kezelt SAM biztonságos kezeléséről gondoskodni. A kártyaelfogadónak
a biztonsági elem beépített védelmének feloldásához használt kulcsok kezelése során az alábbi elvárásoknak
kell megfelelnie:
2.7.1. a kártyaelfogadó nyilvántartja, hogy mely SAM-hez, mely kulcs használandó, a működtető által
biztosított egyedi kulcs alapján;
2.7.2. a kártyaelfogadó szabályzatában rögzíti a biztonsági elemek és a kulcs kezelésére vonatkozó
eljárásrendeket, a szabályzat lefedi a biztonsági elemek és a kulcsok teljes életciklusát;
2.7.3. kártyaelfogadónak szabályzatban meg kell határoznia azon személyek körét, akik a kulcshoz
hozzáférnek.
2.8. A kártyaelfogadó a kulcsot a biztonsági elemtől a szerver oldalon folyamatosan elkülönítve tárolja.
A kártyaelfogadónak ellenőriznie kell a felhasználás előtt, hogy a biztonsági elem továbbra is
a kártyaelfogadó birtokában van, annak használata jogszerű és megfelel az igénylés céljának.
A kártyaelfogadó nyilvántartja a biztonsági elem aktív, inaktív, működőképes, működésképtelen vagy letiltott
állapotát és a biztonsági elemen végzett műveleteket, valamint köteles ezen adatokban bekövetkezett
változásokat a működtetőnek haladéktalanul jelezni. A működtető a kártyaelfogadó által jelzett változásokat
nyilvántartja.
2.9. A korábbi igénylésben rögzített céltól eltérő felhasználás esetén a kártyaelfogadó köteles új igénylést
benyújtani a működtetőhöz az általa biztosított igénylőlap útján.
2.10. A kártyaelfogadó köteles az illetéktelen hozzáférést és felhasználást haladéktalanul jelenteni
a működtetőnek.
2.11. A kártyaelfogadó köteles a működtető által biztosított utólagos kulcsfrissítési metódus valamelyikét saját
környezetébe illeszteni, és ennek megfelelően a publikált kulcsfrissítést elvégezni.”

VIII. A Kúria határozatai
A Kúria közleménye
a Nemzeti Választási Bizottság határozatának helybenhagyásáról
A népszavazás kezdeményezéséről, az európai polgári kezdeményezésről, valamint a népszavazási eljárásról szóló
2013. évi CCXXXVIII. törvény 30. § (4) bekezdése alapján a Kúria az alábbi közleményt teszi közzé:
A Kúria 2020. március 11. napján kelt Knk.VI.37.014/2020/2. számú végzésében a Nemzeti Választási Bizottság
– országos népszavazási kérdés hitelesítését megtagadó – 495/2019. számú határozatát az indokolás
megváltoztatásával helybenhagyta.
A határozat megtekinthető a Kúria hivatalos honlapján, a w ww.kuria-birosag.hu oldalon.
Budapest, 2020. március 11.

Dr. Kalas Tibor s. k.,

a tanács elnöke

IX. Határozatok Tára
