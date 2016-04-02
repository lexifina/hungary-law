## „4. melléklet a 48/2013. (XI. 15.) NGM rendelethez

## Az Adóügyi Ellenőrző Egységben (AEE) tárolt bizonylati adatok tartalmára és szerkezetére vonatkozó előírások

## 1. Az AEE-nek a pénztárgépben keletkezett adatokat UTF-8-as kódlap szerinti karakterkódolású, digitálisan aláírt XML típusú naplóállományokban (p7b) kell tárolnia. Az állomány struktúrájának leírását és a séma ellenőrző állományt (XSD állomány) a NAV közleményben teszi közzé.

## 2. Az AEE-nek a NAV szerverétől kapott, 5. melléklet szerinti utasítás alapján történő adattovábbításkor az AEE-n lévő összes adózó nyitott naplóállományát le kell zárnia, azt digitálisan aláírással kell ellátnia, és azt a NAV szervere felé el kell küldenie. Az AEE-nek minden állomány lezárását követően új naplóállományt kell nyitnia, és az adott adózóhoz rendelt naplóállományban kell folytatnia a bejegyzések rögzítését. Az AEE-nek a naplóállományt – a pénztárgép első üzembehelyezését megelőzően keletkezett állományok kivételével – annak megnyitását követő 24 óra elteltével akkor is le kell zárnia és újat kell nyitnia, ha ezen idő alatt nem történt adattovábbítás a NAV szervere felé.

## 3. Az AEE-nek a naplóállományt a naplófájl megnyitásának időpontja szerinti AAAAAAAAA_BBBBBBBB_ééééhhnnóóppmm_s.p7b néven kell eltárolnia, ahol

## a) AAAAAAAAA: A pénztárgép AP száma 9 karakteren,

## b) BBBBBBBB: Az adózó törzsszáma 8 karakteren, kétvállalkozós pénztárgép esetén az üzemanyag forgalmazó vállalkozás adó törzsszáma

## c) éééé: az év száma négy számjegyen,

## d) hh: a hónap sorszáma két számjegyen,

## e) nn: a nap sorszáma két számjegyen,

## f) óó: az óra száma két számjegyen,

## g) pp: a perc száma két számjegyen,

## h) mm: a másodperc száma két számjegyen,

## i) s: az állomány 1-től kezdődően, kihagyás és ismétlés nélkül képzett sorszáma az AEE élettartama során.

## 4. A jelen mellékletben meghatározott bejegyzések (továbbiakban bejegyzés típusok) tartalmára vonatkozó egységes szabályok a következők:

## 4.1. A bejegyzéseket a digitálisan aláírt XML állományban a NAV által közleményben közzétett XSD állományleíró struktúrának megfelelően kell megvalósítani.

## 4.2. Az AEE által létrehozott állományokban 32-nél kisebb kódú karakterek a CHR(10) sorvégjel kivételével nem szerepelhetnek.

## 4.3. Minden bejegyzést az adott naplóállományban 1-től kezdődő folyamatos sorszámmal kell ellátni.

## 4.4. A naplóállományban a numerikus értékeket a szükséges számú számjegyen, vezető nullák nélkül kell ábrázolni, kivéve, ha ezzel ellentétes előírás szerepel adott adatnál. A pénznem adatok bejegyzésének formátuma forint esetében tagolás nélkül egészre kerekített értékek tizedes nélkül, kivéve, ha ezzel ellentétes előírás szerepel adott adatnál. Az euróra történő átállást követően tagolás nélkül két tizedesre kerekítve, tizedesvesszővel elválasztva.

## 4.5. A jelen mellékletben szereplő ellenőrző kódok képzésére az SHA256 algoritmust kell alkalmazni. Az algoritmus eredményeképpen előálló 64 karakteres kódban szereplő A-F hexadecimális számjegyeket minden esetben nagybetűkként kell értelmezni és feltüntetni. Az SHA256 algoritmus bemenő adata az a karaktersorozat, amely az alábbi részekből tevődik össze az alábbi felsorolás sorrendjében:

## a) A bemenő karaktersorozat első hatvannégy karaktere az AEE által legutóbb lezárt szöveges állomány utolsóként bejegyzett (LCL) bejegyzésének 64 karakteres ellenőrző kódja. Amennyiben még nem létezik legutóbb lezárt szöveges állomány, akkor a bemenő karaktersorozat első 64 karaktere 64 db „F”.

## b) A bemenő karaktersorozat 65-128. karaktere az adott bejegyzést megelőzően rögzített bejegyzésének 64 karakteres ellenőrző kódja. Ha nem létezik az adott szöveges állományban előző bejegyzés, akkor a bemenő karaktersorozat 65-128. karaktere 64 db „F”.

## c) A bemenő karaktersorozat további karakterei az adott bejegyzés azonosítója, valamint minden mezőjének értéke a jelen mellékletben feltüntetett sorrendben, a mezőazonosító kódok nélkül.

## 4.6. Egy adott bejegyzésben minden mezőben fel kell tüntetni az abban szerepeltetendő adatot, ha az az adott konkrét esemény vagy bizonylat tekintetében releváns.

## 4.7. A naplófájlokban minden dátum/idő adatot az XML 1.0 szerinti „éééé-hh-nnTóó:pp:mm+óó:pp” formátumban kell feltüntetni, ahol az év, hónap, nap, óra, perc, másodperc minden esetben a helyi (magyar) idő szerint értendő. Téli időszámítás esetén az időzóna jelölésére a „+01:00”, nyári időszámítás esetén a „+02:00” jelölés használandó.

## 4.8. Az e mellékletben leírt szerkezetű naplóállomány verziószáma „X0006”. Jelen rendelet 2013. XI. 16-án hatályos szövegének megfelelő szerkezetű naplóállomány verziószáma „X0005”. Az AEE által létrehozott naplóállományok mindegyikének meg kell felelnie az egyik verzió követelményeinek. Az e rendeletben megkövetelt átállást követően kizárólag az „X0006” verziónak megfelelő naplóállományok képezhetők.

## 4.9. Ha a vonatkozó sémadefinícióban kötelezőként szereplő mező értéke nem áll rendelkezésre vagy a mező az adott kontextusban nem értelmezhető, a naplóállományban az adott mezőt üres értékkel kell szerepeltetni.

## 5. Az AEE naplóállományaiban az egyes, itt felsorolt események bekövetkezését az alábbi bejegyzések naplózzák.

## 5.1. Az AEE naplóállomány nyitása

## A pénztárgépben működő AEE a naplóállományok megnyitását – minden esetben a naplóállományok első bejegyzéseként – az alábbi bejegyzésekkel naplózza:

## Naplóállomány nyitása esetén a bejegyzés azonosító: LON

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | APN | Pénztárgép AP száma | 9 karakteres szöveg |

| 4. | TSZ | Üzemeltető törzsszáma (kétvállalkozós pénztárgép esetén az üzemanyag tulajdonos törzsszáma) | 8 karakteres szöveg |

| 5. | LFN | Naplófájl sorszáma | 8 karakteres szám |

| 6. | THT | Kétvállalkozós pénztárgép esetén az üzemeltető törzsszáma | 8 karakteres szöveg |

| 7. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 5.2. További eseményekre vonatkozó bejegyzések

## Bejegyzés azonosító: EVT

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Rekordsorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | EVC | Esemény kódja | 3 karakteres szöveg |

| 4. | EVD | Esemény leíró adata | üres / 400 karakteres szöveg |

| 5. | HSH | Ellenőrző kód | 64 HEXA karakter |

## A naplózott esemény jellegét az EVC mező kódolja az alábbiak szerint. Egyes eseményeknél az eseményt jellemző adatot is szerepeltetni kell az EVD mezőben az alábbiak szerint. Ha az esemény jellegéből következően nincs ilyen, az eseményt jellemző adat, akkor az EVD mező üres.

| Esemény | EVC mező értéke | EVD mezőben szereplő adat |

| Naplóállomány zárása (a naplóállomány utolsó bejegyzése) | LCL | (üres) |

| Pénztárgép bekapcsolása | CRI | (üres) |

| Pénztárgép kikapcsolása | CRO | (üres) |

| Az AEE a saját akkumulátoráról kezd működni (áramszünet kezdete) | POF | (üres) |

| Az AEE külső áramforrásról folytatja a működését (áramszünet vége) | PIN | (üres) |

| Az AEE saját áramforrása lemerül | BDN | (üres) |

| Az AEE a saját áramforrás lemerülése után újra működni kezd vagy működés közben újraindul | RST | „B”, ha az újraindulás az áramforrás lemerülése után megy végbe, „O” egyébként |

| A pénztárgépen észlelt hiba miatt a pénztárgép blokkolt állapotba került | BLS | „N”, ha a blokkolásra a NAV adott utasítást, „E” egyébként. |

| A pénztárgép hiba miatt történt blokkolt állapotának vége | BLF | „N”, ha a blokkolásra a NAV adott utasítást, „E” egyébként. |

| Pénztárgép gyakorló üzemmód kezdete | TRI | (üres) |

| Pénztárgép gyakorló üzemmód vége | TRF | (üres) |

| Üzenet küldése a NAV részére | MGO | Az üzenet szövege |

| Üzenet fogadása a NAV-tól | MGI | Az üzenet szövege |

| Euró üzemmód beállítása | EUR | (üres) |

| Pénztárgép szüneteltetés megkezdése | STB | A szüneteltetés végének várható dátuma |

| Pénztárgép szüneteltetés vége | STF | (üres) |

| Pénztárgép átadása a szerviznek | SCB | A javítási folyamat végének várható dátuma (ha ez bejegyezhető) |

| Pénztárgép visszavétele a szerviztől | SCF | (üres) |

| Felülvizsgálat elvégzése | YCH | A felülvizsgálatot végző műszerész igazolványának száma |

| Fogyasztásösszesítő bizonylat megnyitása éttermi pénztárgépen | WDO | Fogyasztásösszesítő egyedi azonosítója |

| Fogyasztásösszesítő bizonylat lezárása éttermi pénztárgépen | WDC | Fogyasztásösszesítő egyedi azonosítója |

| NAV szerverről érkezett üzenet sikeres kinyomtatása | PRN | Az üzenet szövege |

## A NAV-tól érkező szoftver szeletek naplófájlba történő bejegyzése során a bejegyzés EVD mezőjében a „FW” karaktersorozatot és az érkező szoftver szelet sorszámát három karakteren kell szerepeltetni. A NAV szerverről érkező tanúsítványok és kulcsok fogadására vonatkozó bejegyzések esetén az EVD mező tartalma a „CERT”, illetve a „KEY” karaktersorozat.

## A NAV szerver részére küldött naplófájl esetén a bejegyzés EVD mezőjének tartalma a küldött állomány teljes neve.

## 5.3. Pénztárgép működési információi, rendszerállapota és forgalmazási statisztikái és földrajzi helye

## A pénztárgépnek működése során minden naplóállományban legalább egyszer rögzíteni kell a pénztárgép működésére vonatkozó alábbi adatokat az alább leírt bejegyzésekben.

## 5.3.1. Pénztárgép működési információi bejegyzés azonosítója: INF

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | DTY | AEE gyártói típusnév | 200 karakteres szöveg |

| 4. | DRV | AEE hardver verzió | 200 karakteres szöveg |

| 5. | DFW | AEE szoftver verzió | 5 karakteres szöveg |

| 6. | DFH | AEE-ben futó szoftver SHA256 algoritmussal kiszámított ellenőrző kódja | 64 karakteres szöveg |

| 7. | DFT | Az AEE-ben futó szoftver legutóbbi frissítésének időpontja. | szabványos dátum és idő adat másodperc pontossággal |

| 8. | DMT | Az AEE-ben lévő modem kiolvasott típus megnevezése, | 32 karakteres szöveg |

| 9. | DMF | Az AEE-ben lévő modem kiolvasott szoftver-verziója. | 200 karakteres szöveg |

| 10. | DME | Az AEE-ben lévő modem kiolvasott IMEI száma. | 50 karakteres szöveg |

| 11. | DMS | Az AEE-ben lévő SIM kiolvasott IMSI száma. | 50 karakteres szöveg |

| 12. | AKN | Akkumulátor gyári száma | 50 karakteres szöveg |

| 13. | TSZ | Üzemeltető adó törzsszáma | 20 karakteres szöveges |

| 14. | NAM | Üzemeltető neve | 100 karakteres szöveg |

| 15. | IRS | Üzemeltető székhely irányítószám | 6 karakteres szöveg |

| 16. | TEL | Üzemeltető székhely település | 50 karakteres szöveg |

| 17. | KZT | Üzemeltető székhely közterület neve | 50 karakteres szöveg |

| 18. | KZJ | Üzemeltető székhely közterület jellege | 20 karakteres szöveg |

| 19. | HSZ | Üzemeltető székhely házszám | 50 karakteres szöveg |

| 20. | VAT | Aktuális ÁFA-tábla (a vonatkozó NAV üzenet) | 200 karakteres szöveges |

| 21. | GSM | A legutóbb használt cella egyedi azonosítója | 20 karakteres szöveg |

| 22. | TNA | Pénztárgép telephely (üzlet) elnevezése | 100 karakteres szöveg |

| 23. | TZC | Pénztárgép telephely irányítószám | 6 karakteres szöveg |

| 24. | TCY | Pénztárgép telephely település | 50 karakteres szöveg |

| 25. | TKN | Pénztárgép telephely közterület neve | 50 karakteres szöveg |

| 26. | TKJ | Pénztárgép telephely közterület jellege | 20 karakteres szöveg |

| 27. | THH | Pénztárgép telephely házszám | 50 karakteres szöveg |

| 28. | DPH | A pénztárgép hardver gyártói típusmegjelölése | 50 karakteres szöveg |

| 29. | DPV | A pénztárgép hardververziója | 50 karakteres szöveg |

| 30. | DPF | A pénztárgépben futó szoftver verziószáma | 50 karakteres szöveg |

| 31. | DPS | A pénztárgépben futó szoftver SHA256 algoritmussal kiszámított ellenőrző kódja, AEE-vel felszerelt adóügyi nyomtató esetén üres | 64 karakteres szöveg |

| 32. | VCC | Legutóbb használt üzembe helyezési kód | 16 karakteres szöveg |

| 33. | MIS | A pénztárgépen a legutóbbi beavatkozást végző műszerész igazolványának száma | 12 karakteres szöveg |

| 34. | APN | Pénztárgép AP száma | 9 karakteres szöveg |

| 35. | COM | A pénztárgép által használt kommunikációs protokoll verziószáma | Cnnnn, ahol nnnn a kommunikációs protokoll verziószáma. |

| 36. | XMV | A legfrissebb séma verziószáma, aminek a pénztárgép által képzett naplóállományok megfelelnek. | Xnnnn, ahol nnnn a séma verziószáma. |

| 37. | HSH | Ellenőrző kód | 64 HEXA karakter |

## Az ezen rendelet 5. mellékletében foglaltak szerint kommunikáló pénztárgép esetén a COM mezőben „C0002” értéket kell szerepeltetni.

## 5.3.2. Pénztárgép rendszerállapota bejegyzés azonosító: STA

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | SST | Pénztárgép állapot: „0”, ha a pénztárgép működik és nincs blokkolva „1”, ha a pénztárgép blokkolt állapotban van „2”, ha a pénztárgép hibás | 1 karakteres szöveg |

| 4. | SFL | Az AEE-ben működő adattárolón lévő szabad tároló kapacitás (Kbyte) | 10 karakteres numerikus |

| 5. | SSG | Az AEE-ben működő modem által mért hálózati térerőt (-1)dBm - (-199)dBm-ig terjedő skálán negatív egész számmal ábrázolva. | 4 karakteres numerikus |

| 6. | SAC | Akkumulátor töltöttség egész számmal, vezető nullák nélkül (%) | 3 karakteres numerikus |

| 7. | SMT | GSM hálózatból kiolvasott pontos idő | szabványos dátum és idő adat másodperc pontossággal |

| 8. | SCC | Pénztárgépben az utolsó STA rekord küldése óta jelentkezett hibák belső kódjainak listája. | 400 karakteres szöveg a gyártó által kialakított struktúrában |

| 9. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 5.3.3. Pénztárgép forgalmazási mérőszámai bejegyzés azonosító: OPR

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | ODS | A legutóbbi bekapcsolás óta a modem által küldött bájtok száma, beleértve a megszakadt kapcsolatok adatait is. | 12 karakteres numerikus |

| 4. | ODR | A legutóbbi bekapcsolás óta a modem által fogadott bájtok számát, beleértve a megszakadt kapcsolatok adatait is, | 12 karakteres numerikus |

| 5. | ODF | A legutóbbi bekapcsolás óta a mobil adatkapcsolat kiépítésére tett sikertelen kísérletek száma. | 5 karakteres numerikus |

| 6. | OSF | A legutóbbi bekapcsolás óta az SSL adatcsatorna felépítésére tett sikertelen kísérletek száma. | 5 karakteres numerikus |

| 7. | NET | A legutóbbi bejelentkezés során használt átviteli technológia: 0 – GSM 1 – 2G technológia 2 – 2,5G technológia 3 – 3G technológia 4 – 4G technológia | 1 karakteres szöveg |

| 8. | PRV | A legutóbbi bejelentkezés során használt infrastruktúrát biztosító fizikai mobilszolgáltató: 0 – Magyar Telekom 1 – Telenor 2 – Vodafone 3 – Egyéb | 1 karakteres szöveg |

| 9. | OCC | AEE belső mérőszámai, ahol „N” a belső mérőszám azonosítóját, „E” a mért paraméter értékét jelenti. | 400 karakteres szöveg a forgalmazó által definiált struktúrában |

| 10. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 5.3.4. Pénztárgép földrajzi helye bejegyzés azonosító: POS

## Ezt a bejegyzést csak az olyan pénztárgépeknek kell elhelyezni a naplóállományokban, amelyek képesek a GPS alapú helymeghatározásra.

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | GSA | Pénztárgép földrajzi szélessége fokban, legfeljebb 5 tizedesjegy pontossággal, előjelet használva, a WGS84 szabvány szerint | 20 karakteres szöveges |

| 4. | GSB | Pénztárgép földrajzi hosszúsága fokban, legfeljebb 5 tizedesjegy pontossággal, előjelet használva, a WGS84 szabvány szerint | 20 karakteres szöveges |

| 5. | GSH | Pénztárgép tengerszint feletti magassága méterben, a WGS84 szabvány szerint | 5 karakteres szöveg |

| 6. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 5.4. Óraállítás naplózása

## A pénztárgépben működő AEE órájának bármilyen okból történő átállítását az alábbi bejegyzéssel kell naplózni.

## Óraállítás bejegyzés azonosító: TUD

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | max 5 hosszú numerikus |

| 2. | OLD | Azaz idő, amikor az átállítás régi idő szerint bekövetkezik. | szabványos dátum és idő adat másodperc pontossággal |

| 3. | NEW | Beállított új idő | szabványos dátum és idő adat másodperc pontossággal |

| 4. | CHT | ha a rendszer nem diszkréten változtatja az időt, hanem egy időtávon gyorsítja vagy lassítja az időt, akkor az átmenet ideje másodpercben | 10 karakteres numerikus |

| 5. | CAS | az időállítás módja: 1-GSM szinkronizáció, 2-Szervizes beavatkozás, 3-Üzemeltető által módosítva 4-Számítógép alapú pénztárgépeknél a számítógép órájához szinkronizálva 5-Egyéb automatikus szinkronizáció | 1-5 számok egyike |

| 6. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6. Bizonylatok kibocsátására vonatkozó bejegyzések

## A jelen mellékletben felsorolt bizonylatok kibocsátását az itt meghatározott szerkezetű és adattartalmú bejegyzésekkel kell naplózni az AEE naplóállományában. A Rendelet előírásaival összhangban az AEE-nek egy adott bejegyzés naplófájlban történő elhelyezésére akkor kell képesnek lennie, ha az adott pénztárgépen készíthető adott típusú bizonylat.

## Gyakorló üzemmódban kibocsátott bizonylatok naplózására akkor kell képesnek lennie az AEE-nek, ha az adott pénztárgép gyakorló üzemmódba kapcsolható.

## A bizonylatkibocsátásokra vonatkozó bejegyzésekben szereplő „Bizonylat számláló értéke” kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül.

## A több példányban nyomtatott bizonylatok kibocsátását egy bejegyzéssel kell naplózni úgy, hogy a bejegyzés megfelelő mezőjében a nyomtatási példányszám kerül elhelyezésre.

## Az önkiszolgáló üzemanyagkút rendszeren a bizonylat példányszámaként nullát kell szerepeltetni, amennyiben a bizonylat nyomtatása halasztottan történik, vagy a vevő kérésére nem történik meg.

## 6.1 Pénztárnyitás bizonylat

## A pénztárnyitás bizonylat az adóügyi nap nyitását kísérő bizonylat. Ennek kibocsátását az alábbi bejegyzéssel kell naplózni az AEE naplóállományában.

## Bejegyzés azonosító: CON (gyakorló üzemmódban: COT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | DNO | a megnyitott adóügyi nap sorszáma | 20 karakteres numerikus |

| 6. | DRC | a nyitó pénzkészlet adatai | lista |

| 6.1 | > FE1 | forint készpénz forintban | 20 karakteres numerikus |

| 6.2 | > FEV | a valutában befizetett összeg adatai | lista, max. 20 |

| 6.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 6.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 6.2.3 | > > CRA | a valuta egy egységének forintban kifejezett, adózó által alkalmazott értéke (árfolyama) legfeljebb hat értékes jegy pontossággal | 20 karakteres numerikus |

| 6.2.4 | > > CFT | a valuta összegének értéke egész forintban, a feltüntetett árfolyamon számolva | 20 karakteres numerikus |

| 6.3 | > FE3 | nyitó készlet egyéb fizetőeszköz tekintetében | lista 20 |

| 6.3.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 6.3.2 | > > FES | nyitó pénzkészlet a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 7. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 8. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 9. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveges |

| 10. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 11. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.2. Nyugta, egyszerűsített számla

## Nyugta kibocsátása esetén a bejegyzés azonosító: NYN (gyakorló üzemmód esetén NYT)

## Egyszerűsített számla kibocsátása esetén a bejegyzés azonosító: ESN (gyakorló üzemmód esetén EST)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke. | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat nyitásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | NSZ | a bizonylat száma bbbb/ccccc formátumban, ahol bbbb: adóügyi nap sorszáma ccccc: adott napon kibocsátott bizonylat sorszáma | 20 karakteres szöveg |

| 6. | IID | Csak egyszerűsített számla esetén a számlaszám, n/aaaaaaaaa/bbbb/ccccc formátumban, ahol n: kétvállalkozós pénztárgép esetén az üzemeltető jele (A vagy B) aaaaaaaaa: AP szám bbbb: adóügyi nap sorszáma ccccc: egyszerűsített számla napi számlálója | 50 karakteres szöveg |

| 7. | ITL | A bizonylaton szereplő összes tételre vonatkozóan, tételenként | lista (max. 1.000) |

| 7.1 | > NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 7.2 | > PN | a tételhez tartozó cikkszám | 50 karakteres szöveg |

| 7.3 | > UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, legfeljebb négy tizedes pontossággal | 8+4 karakteres numerikus |

| 7.4 | > QY | a tételnél a bizonylaton szereplő mennyiség, maximum 4 tizedesjegy pontossággal | 8+4 karakteres numerikus |

| 7.5 | > IU | a tételnél a bizonylaton szereplő mennyiségi egység | 10 karakteres szöveges |

| 7.6 | > TY | Az adott tétel jellege: „”: értékesítés „s”: értékesítés sztornó „e”: engedmény „es”: engedmény sztornó „k”: nem üzletpolitikai kedvezmény „ks”: nem üzletpolitikai kedvezmény sztornó „f”: felár „fs”: felár sztornó „g”: göngyöleg visszaváltás „gs”: göngyöleg visszaváltás sztornó | 5 karakteres szöveg |

| 7.7 | > SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 7.8 | > VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 7.9 | > RM | a tételsorra vonatkozó, legfeljebb 40-szer ismételhető megjegyzés mező | 50 karakteres szöveg |

| 8. | DRC | a fióktartalom változásának adatai | lista |

| 8.1 | > FE1 | forint készpénz fióktartalom változása forintban | 20 karakteres numerikus |

| 8.2 | > FEV | a valutás fióktartalom változásának adatai | lista, max. 10 |

| 8.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 8.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 8.2.3 | > > CRA | a valuta egy egységének forintban kifejezett, adózó által alkalmazott értéke (árfolyama) legfeljebb hat értékes jegy pontossággal | 20 karakteres numerikus |

| 8.2.4 | > > CFT | a valuta összegének értéke egész forintban, a feltüntetett árfolyamon számolva | 20 karakteres numerikus |

| 8.3 | > FE2 | bankkártya fiókegyenleg módosulása egész forintban | 20 karakteres numerikus |

| 8.4 | > FEE | egészségpénztári fiókegyenleg módosulása forintban, csak egyszerűsített számla esetén | 20 karakteres numerikus |

| 8.5 | > FE3 | fióktartalom módosulása egyéb fizetőeszköz tekintetében | lista, max. 20 |

| 8.5.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 8.5.2 | > > FES | Fióktartalom módosulása a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 9. | RND | a bizonylaton szereplő kerekítés összege, egész forintban számolva, szükség esetén negatív előjellel, ha van ilyen adat | 20 karakteres numerikus |

| 10. | TRA | Kétvállalkozós pénztárgépeknél használt mező (átvitel) | 20 karakteres numerikus |

| 11. | RCV | Kétvállalkozós pénztárgépeknél használt mező (áthozat) | 20 karakteres numerikus |

| 12. | PNU | Kétvállalkozós pénztárgépeknél használt mező (iker bizonylat száma) | 50 karakteres szöveg |

| 13. | VED | Egyszerűsített számla esetén a termék beszerzőjének, szolgáltatás igénybevevőjének adatai az ÁFA tv. rendelkezései szerint | lista |

| 13.1 | > NAM | Beszerző vagy igénybevevő neve | 50 karakteres szöveg |

| 13.2 | > IRS | Irányítószám | 20 karakteres szöveg |

| 13.3 | > TEL | Település | 50 karakteres szöveg |

| 13.4 | > KZT | Közterület neve | 50 karakteres szöveg |

| 13.5 | > KZJ | Közterület jellege | 20 karakteres szöveg |

| 13.6 | > HSZ | Házszám | 50 karakteres szöveg |

| 13.7 | > ASZ | Adószám | 20 karakteres szöveg |

| 14. | SUM | A bizonylaton szereplő tételsorok összege forintban | 20 karakteres numerikus |

| 15. | NYL | Egyedi vevő azonosító | 20 karakteres szöveg |

| 16. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 17. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveg |

| 18. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 19. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 20. | CTS | Időbélyeg, a bizonylat zárásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 21. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.3. Napi forgalmi jelentés (NFN)

## Napi forgalmi jelentés bizonylat kibocsátásával kell kísérni a pénztárgépen az adóügyi nap lezárását. A napi forgalmi jelentést közvetlen megelőzően pénztárjelentést is automatikusan nyomtatnia kell a pénztárgépnek. A napi forgalmi jelentés kibocsátását az alábbi bejegyzéssel kell naplózni az AEE naplóállományába.

## Napi forgalmi jelentés bejegyzés azonosító: NFN (gyakorló üzemmódban: NFT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | ZSZ | a zárás sorszáma négy karakteren, szükség esetén vezető nullákkal feltöltve | 4 karakteres szöveg |

| 6. | GYF | Napi forgalom forgalmi gyűjtők szerinti összesítése | lista |

| 7. | > GYJ | Forgalmi gyűjtő jele 3 karakteren (A00..E99) | 3 karakteres szöveg |

| 8. | > GYE | Az adott forgalmi gyűjtőbe tartozó napi tételek bruttó összértéke | 20 karakteres numerikus |

| 9. | NSF | a napi forgalom összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 10. | NSH | a napi felár összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 11. | NSS | a napi sztornó összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 12. | NSY | a napi engedmény összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 13. | NSV | a napi visszáru összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 14. | NDB | a napi nyugták és egyszerűsített számlák száma összesen | 20 karakteres numerikus |

| 15. | NNS | napi nyugták száma | 20 karakteres numerikus |

| 16. | NES | napi egyszerűsített számlák száma | 10 karakteres numerikus |

| 17. | NPB | napi pénzmozgás bizonylatok száma | 10 karakteres numerikus |

| 18. | NIR | napi megszakítások száma | 10 karakteres numerikus |

| 19. | NST | a napi sztornó bizonylatok száma összesen | 20 karakteres numerikus |

| 20. | STS | napi sztornó bizonylatok összértéke összesen, egész forintban, pozitív számként | 10 karakteres numerikus |

| 21. | SGY | Napi sztornó bizonylatok forgalmi gyűjtőnként | lista (max. 500) |

| 21.1 | > GYJ | Gyűjtő jele három karakteren | 3 karakteres szöveg |

| 21.2 | > GYE | Napi sztornó értéke az adott gyűjtőben | 20 karakteres numerikus |

| 22. | NSW | a napi visszáru bizonylatok száma összesen, ide nem értve a göngyölegjegyeket | 20 karakteres numerikus |

| 23. | VSS | napi visszáru bizonylatok értéke összesen, egész forintban, pozitív számként, ide nem értve a göngyölegjegyeket | 20 karakteres numerikus |

| 24. | VGY | Napi visszáru bizonylatok értéke forgalmi gyűjtőnként | lista (max. 500) |

| 24.1 | > GYJ | Gyűjtő jele három karakteren | 3 karakteres szöveg |

| 24.2 | > GYE | Napi visszáru értéke az adott gyűjtőben | 20 karakteres numerikus |

| 25. | GGY | Napi göngyöleg visszaváltás értéke forgalmi gyűjtőnként | lista (max. 500) |

| 25.1 | > GYJ | Gyűjtő jele három karakteren | 3 karakteres szöveg |

| 25.2 | > GYE | Napi göngyöleg visszaváltás értéke az adott gyűjtőben | 20 karakteres numerikus |

| 26. | NSG | a göngyölített forgalom | 50 karakteres numerikus |

| 27. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 28. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveges |

| 29. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 30. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 31. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.4. Pénztárjelentés

## Bejegyzés azonosító: PJN (gyakorló üzemmódban: PJT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | CRO | Nyitó pénzkészlet adatai | lista |

| 5.1 | > FE1 | forint készpénz forintban | 20 karakteres numerikus |

| 5.2 | > FEV | a valuták adatai (többszörözhető rekord) | (lista) |

| 5.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 5.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 5.3 | > FE3 | fióktartalom módosulása egyéb fizetőeszköz tekintetében | lista |

| 5.3.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 5.3.2 | > > FES | Fióktartalom módosulása a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 6. | SEL | Értékesítéshez, sztornó- és visszáruhoz kapcsolódó be- és kifizetések egyenlege fizetőeszközönként | lista |

| 6.1 | > FE1 | forint készpénz forintban | 20 karakteres numerikus |

| 6.2 | > FEV | a valuták adatai (többszörözhető rekord) | (lista) |

| 6.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 6.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 6.3 | > FE2 | bankkártyás bevételek egész forintban | 20 karakteres numerikus |

| 6.4 | > FEE | egyszerűsített számlákon feltüntetett egészségpénztári bevételek | 20 karakteres numerikus |

| 6.5 | > FE3 | egyéb fizetőeszközökben megszerzett bevételek fizetőeszközönként | lista |

| 6.5.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 6.5.2 | > > FES | Bevétel a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 7. | CIO | Nem értékesítéshez kötődő pénztári ki- és befizetések napi egyenlege fizetőeszközönként | lista |

| 7.1 | > FE1 | forint készpénz forintban | 20 karakteres numerikus |

| 7.2 | > FEV | a valuták adatai (többszörözhető rekord) | (lista) |

| 7.2.1 | > > CAM | a valuta összege (valutában) | 20 karakteres numerikus |

| 7.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 7.3 | > FE2 | bankkártyás befizetések és banki utalással végrehajtott kifizetések egyenlege egész forintban | 20 karakteres numerikus |

| 7.4 | > FE3 | egyéb fizetőeszközökben teljesített ki- és befizetések egyenlege fizetőeszközönként | lista |

| 7.4.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 7.4.2 | > > FES | Egyenleg a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 8. | CUS | Aktuális fióktartalom fizetőeszközönként | lista |

| 8.1 | > FE1 | forint készpénz forintban | 20 karakteres numerikus |

| 8.2 | > FEV | a valuták adatai (többszörözhető rekord) | (lista) |

| 8.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 8.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 8.3 | > FE2 | bankkártyás bevételek, befizetések, illetve a bankszámlára utalással teljesített kifizetések egyenlege egész forintban | 20 karakteres numerikus |

| 8.4 | > FEE | egyszerűsített számlákon feltüntetett egészségpénztári bevételek | 20 karakteres numerikus |

| 8.5 | > FE3 | egyéb fizetőeszközökben megszerzett bevételek, ki- és befizetések egyenlege fizetőeszközönként | lista |

| 8.5.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 8.5.2 | > > FES | Egyenleg a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 9. | IRN | Napi nyugtamegszakítások száma | 20 karakteres numerikus |

| 10. | IRV | Napi megszakított nyugták összértéke (a megszakítás előtti állapotok szerint) | 20 karakteres numerikus |

| 11. | NSD | Napi tételsztornó száma | 20 karakteres numerikus |

| 12. | NSE | Napi tételsztornó összértéke | 20 karakteres numerikus |

| 13. | TIP | Napi felszolgálói díj összege | 20 karakteres numerikus |

| 14. | INE | Egyes speciális értékesítések napi összege | 20 karakteres numerikus |

| 15. | INS | Egyes speciális értékesítések napi sztornó összege | 20 karakteres numerikus |

| 16. | INV | Számlával kísért értékesítés napi visszáru összege | 20 karakteres numerikus |

| 17. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 18. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveges |

| 19. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 20. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 |

| 21. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.5. Pénzmozgás bizonylat

## Pénzmozgás bizonylattal kell kísérni minden olyan tranzakciót, ami nem értékesítéshez, illetve sztornó vagy visszáru bizonylat kibocsátásához kötődik, de módosítja a fióktartalmat (ideértve a bankkártyás befizetéseket, illetve a bankszámlára utalással teljesített kifizetések egyenlegét is). Ugyancsak pénzmozgás bizonylatot kell kibocsátani, ha egy korábban rögzített bizonylaton a fizetési eszközök téves rögzítése folytán a fióktartalom összetételének módosítása szükséges.

## Pénzmozgás bizonylat bejegyzés azonosító: PMN (gyakorló üzemmódban: PMT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | PMS | Pénzmozgás bizonylat sorszáma M/nnnn/sssss alakban, ahol nnnn az adóügyi nap sorszáma, sssss a pénzmozgás bizonylatok napi számlálója | 10 karakteres szöveg |

| 6. | RSN | a pénztári befizetés, kifizetés vagy fizetőeszköz csere jogcímei: Befizetés okok: 01 - váltópénz bevitel 02 - pénztáros pénzfelvétel 03 - díjbeszedés 04 - sorsjegy eladás 05 - előleg 06 - pénztárhiány 07 - borravaló 08 – egyéb befizetés Kifizetés okok: 31 - fölözés 32 - pénztáros levétel 33 - utalvány kivét 34 - ajándékkártya kivét 35 - bérkifizetés 36 - munkabér előleg 37 - postaköltség 38 - egyéb rezsi 39 - áruvásárlás 40 - záróösszeg levétel 41 - egyéb kifizetés Fizetőeszköz csere: 60 - fizetőeszköz csere | 2 karakteres szöveg |

| 7. | DRC | a fióktartalom változásának adatai | (lista) |

| 7.1 | > FE1 | forint készpénz fióktartalom változása forintban | 20 karakteres numerikus |

| 7.2 | > FEV | a valutás fióktartalom változásának adatai | (lista, max 10.) |

| 7.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 7.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 7.2.3 | > > CRA | a valuta egy egységének forintban kifejezett, adózó által alkalmazott értéke (árfolyama) legfeljebb hat értékes jegy pontossággal | 20 karakteres numerikus |

| 7.2.4 | > > CFT | a valuta összegének értéke egész forintban, a feltüntetett árfolyamon számolva | 20 karakteres numerikus |

| 7.3 | > FE2 | bankkártya fiókegyenleg módosulása egész forintban | 20 karakteres numerikus |

| 7.4 | > FEE | egészségpénztári fiókegyenleg módosulása forintban, csak egyszerűsített számla esetén | 20 karakteres numerikus |

| 7.5 | > FE3 | fióktartalom módosulása egyéb fizetőeszköz tekintetében | lista |

| 7.5.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 7.5.2 | > > FES | Fióktartalom módosulása a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 8. | PBA | a bizonylathoz kapcsolódó visszajáró összege egész forintban | 20 karakteres numerikus |

| 9. | PRD | kerekítési különbözet összege forintban (pozitív, ha a vevő szempontjából számolt előjellel | 20 karakteres numerikus |

| 10. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 11. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 99-szer feltüntethető egyedi mező | 200 karakteres szöveges |

| 12. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 13. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 14. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.6. Egyes speciális értékesítések bizonylata, illetve ennek sztornó és visszáru bizonylata

## Az egyes speciális értékesítések bizonylatával kell kísérni minden olyan értékesítést és szolgáltatásnyújtást, amelyhez kötődően az eladó utólag számla kibocsátását fogja eszközölni az adott tranzakcióról a vevő, vagy érdekkörében eljáró más személy részére, és az értékesítés helyszínén fizetés nem történik. Az ilyen bizonylatok kibocsátását az alábbi bejegyzéssel kell naplózni az AEE naplóállományában.

## Az egyes speciális értékesítések bizonylatának sztornó és visszáru bizonylatát is egyes speciális értékesítések bizonylataként kell naplózni, a tételsorok TY mezőjében megfelelően használt jelöléseket alkalmazva.

## Bejegyzés azonosító: IVN (gyakorló üzemmódban: IVT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | ORN | Bizonylatszám X/aaaa/bbbbb alakban, ahol: X: a bizonylat típusának jelölése, egészségkártyás bizonylat esetén „EK”, üzemanyagkártyás bizonylat esetén „UK” aaaa: az adóügyi nap sorszáma bbbbb: a bizonylat sorszáma | 20 karakteres szöveg |

| 6. | EPN | az egészségpénztár neve, amennyiben értelmezhető | 50 karakteres szöveg |

| 7. | EPA | az egészségpénztár címe, amennyiben értelmezhető | 200 karakteres szöveg |

| 8. | EPC | az egészségpénztár kódja, amennyiben értelmezhető | 50 karakteres szöveg |

| 9. | ERN | a vevő tagszáma (egészségpénztári azonosítószáma) , amennyiben értelmezhető | 50 karakteres szöveg |

| 10. | ECN | az egészségkártya száma , amennyiben értelmezhető | 20 karakteres szöveg |

| 11. | VED | A vevő adatai | lista |

| 11.1 | > NAM | Beszerző vagy igénybevevő neve | 50 karakteres szöveg |

| 11.2 | > IRS | Irányítószám | 20 karakteres szöveg |

| 11.3 | > TEL | Település | 50 karakteres szöveg |

| 11.4 | > KZT | Közterület neve | 50 karakteres szöveg |

| 11.5 | > KZJ | Közterület jellege | 20 karakteres szöveg |

| 11.6 | > HSZ | Házszám | 50 karakteres szöveg |

| 12. | > ASZ | Adószám | 20 karakteres szöveg |

| 13. | FCN | üzemanyagkártya száma (legalább négy számjegy), amennyiben értelmezhető | 20 karakteres szöveg |

| 14. | CID | engedélyezési azonosítószám, amennyiben értelmezhető | 20 karakteres szöveg |

| 15. | FRN | a rendszám, kizárólag betűket és számokat feltüntetve, amennyiben értelmezhető | 20 karakteres szöveg |

| 16. | ITL | A bizonylat összes tételére vonatkozóan, tételenként | lista (max 1.000) |

| 16.1 | > NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 16.2 | > PN | a tételhez tartozó cikkszám | 50 karakteres szöveg |

| 16.3 | > UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, legfeljebb 4 tizedes pontossággal | 20 karakteres numerikus |

| 16.4 | > QY | a tételnél a bizonylaton szereplő mennyiség, maximum 4 tizedesjegy pontossággal | 20 karakteres numerikus |

| 16.5 | > IU | a tételnél a bizonylaton szereplő mennyiségi egység | 10 karakteres szöveges |

| 16.6 | > TY | Az adott tétel jellege: „”: értékesítés „s”: értékesítés sztornó „e”: engedmény „es”: engedmény sztornó „k”: nem üzletpolitikai kedvezmény „ks”: nem üzletpolitikai kedvezmény sztornó „f”: felár „fs”: felár sztornó "v": visszáru "vs": visszáru sztornó „g”: göngyöleg visszaváltás „gs”: göngyöleg visszaváltás sztornó | 5 karakteres szöveg |

| 16.7 | > SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 16.8 | > VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 16.9 | > RM | a tételsorra vonatkozó, legfeljebb 40-szer ismételhető megjegyzés mező | 50 karakteres szöveg |

| 17. | SUM | Bizonylat összesen forintban, amennyiben értelmezhető | 20 karakteres numerikus |

| 18. | SUV | Bizonylat összesen valutában, amennyiben értelmezhető | lista (max. 10) |

| 18.1 | > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 18.2 | > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 19. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 20. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveg |

| 21. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 22. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 23. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.7. Sztornó bizonylat (SZN)

## Sztornó bizonylatot kell kibocsátani, ha egy korábban kibocsátott bizonylattal bizonylatolt tranzakció nem történt meg. A sztornó bizonylat kibocsátását az alábbi bejegyzéssel kell naplózni az AEE naplóállományában.

## Sztornó bizonylat bejegyzés azonosító: SZN (gyakorló módban: SZT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylatszámláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | SBS | A sztornó bizonylat száma S/bbbb/ccccc alakban (kétvállalkozós pénztárgépeken S/X/bbbb/ccccc alakban), ahol: X: Az üzemeltető jele (A vagy B) bbbb: adónap sorszáma ccccc: bizonylat sorszáma | 20 karakteres szöveg |

| 6. | SBN | a sztornózott nyugta, egyszerűsített számla vagy visszáru bizonylat egyedi azonosítója | 50 karakteres szöveg |

| 7. | RSN | a sztornózás oka: S1 – ügyfél elállása S2 – kezelői hiba: téves bevitel S3 – kezelői hiba: téves fizetőeszköz bevitel S4 – kezelői hiba: termék nincs készleten S5 – technikai: téves bizonylattípus kibocsátása S6 – technikai: sikertelen fizetőeszköz használat S7 – technikai: téves ügyfél adat/hibás bevitel S8 – technikai: próbavásárlás S0 – egyéb | 2 karakteres szöveg |

| 8. | VED | A vevő adatai | lista |

| 8.1 | > NAM | Beszerző vagy igénybevevő neve, vagy a sztornó jegyzőkönyv egyedi azonosítója | 50 karakteres szöveg |

| 8.2 | > IRS | Irányítószám | 20 karakteres szöveg |

| 8.3 | > TEL | Település | 50 karakteres szöveg |

| 8.4 | > KZT | Közterület neve | 50 karakteres szöveg |

| 8.5 | > KZJ | Közterület jellege | 20 karakteres szöveg |

| 8.6 | > HSZ | Házszám | 50 karakteres szöveg |

| 8.7 | > ASZ | Adószám | 20 karakteres szöveg |

| 9. | ITL | A bizonylat összes tételére vonatkozóan, tételenként | lista |

| 9.1 | > NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 9.2 | > PN | a tételhez tartozó cikkszám | 50 karakteres szöveg |

| 9.3 | > UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, legfeljebb négy tizedes pontossággal | 8+4 karakteres numerikus |

| 9.4 | > QY | a tételnél a bizonylaton szereplő mennyiség, maximum 4 tizedesjegy pontossággal | 8+4 karakteres numerikus |

| 9.5 | > IU | a tételnél a bizonylaton szereplő mennyiségi egység | 10 karakteres szöveges |

| 9.6 | > TY | Az adott tétel jellege: „”: értékesítés „s”: értékesítés sztornó „e”: engedmény „es”: engedmény sztornó „k”: nem üzletpolitikai kedvezmény „ks”: nem üzletpolitikai kedvezmény sztornó „f”: felár „fs”: felár sztornó „g”: göngyöleg visszaváltás „gs”: göngyöleg visszaváltás sztornó | 5 karakteres szöveg |

| 9.7 | > SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 9.8 | > VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 9.9 | > RM | a tételsorra vonatkozó, legfeljebb 40-szer ismételhető megjegyzés mező | 50 karakteres szöveg |

| 10. | SUM | Bizonylat összesen forintban | 20 karakteres numerikus |

| 11. | PCR | a sztornó bizonylathoz kapcsolódó kerekítési különbözet összege forintban | 20 karakteres numerikus |

| 12. | TRA | Kétvállalkozós pénztárgépeknél használt mező (átvitel) | 20 karakteres numerikus |

| 13. | RCV | Kétvállalkozós pénztárgépeknél használt mező (áthozat) | 20 karakteres numerikus |

| 14. | PNU | Kétvállalkozós pénztárgépeknél használt mező (iker bizonylat száma) | 50 karakteres szöveg |

| 15. | DRC | a fióktartalom változásának adatai | lista |

| 15.1 | > FE1 | forint készpénz fióktartalom változása forintban | 20 karakteres numerikus |

| 15.2 | > FEV | a valutában fizetett összeg adatai (többszörözhető rekord) | lista, max. 10 |

| 15.3 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 15.3.1 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 15.3.2 | > > CRA | a valuta egy egységének forintban kifejezett, adózó által alkalmazott értéke (árfolyama) legfeljebb hat értékes jegy pontossággal | 20 karakteres numerikus |

| 15.3.3 | > > CFT | a valuta összegének értéke egész forintban, a feltüntetett árfolyamon számolva | 20 karakteres numerikus |

| 15.4 | > FE2 | bankkártya fiókegyenleg módosulása egész forintban | 20 karakteres numerikus |

| 15.5 | > FEE | egészségpénztári fiókegyenleg módosulása forintban, csak egyszerűsített számla esetén | 20 karakteres numerikus |

| 15.6 | > FE3 | fióktartalom módosulása egyéb fizetőeszköz tekintetében | lista, max. 20 |

| 15.6.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 15.6.2 | > > FES | Fióktartalom módosulása a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 16. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 17. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveg |

| 18. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 19. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 20. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.8. Visszáru bizonylat

## Visszáru bizonylat kibocsátását az alábbi bejegyzéssel kell naplózni az AEE naplóállományába.

## Visszáru bizonylat (göngyölegjegy bizonylat) bejegyzés azonosító: VBN (gyakorló üzemmódban: VBT)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | VBS | A visszáru bizonylat száma V/bbbb/ccccc (kétvállalkozós pénztárgépen V/X/bbbb/ccccc) alakban, ahol: X: Az üzemeltető jele (A vagy B) bbbb: adónap sorszáma ccccc: bizonylat sorszáma | 20 karakteres szöveg |

| 6. | VDB | a visszáruzott nyugta vagy egyszerűsített számla sorszáma, a göngyölegjegy esetén "GJ" | 50 karakteres szöveg |

| 7. | RSN | a visszáruzás oka: V1 – hibás áru V2 – ügyfél elállása a vásárlástól V3 – egyéb | 2 karakteres szöveg |

| 8. | VED | A vevő adatai (göngyölegjegy esetén nem szerepel) | lista |

| 8.1 | > NAM | Beszerző vagy igénybevevő neve | 50 karakteres szöveg |

| 8.2 | > IRS | Irányítószám | 20 karakteres szöveg |

| 8.3 | > TEL | Település | 50 karakteres szöveg |

| 8.4 | > KZT | Közterület neve | 50 karakteres szöveg |

| 8.5 | > KZJ | Közterület jellege | 20 karakteres szöveg |

| 8.6 | > HSZ | Házszám | 50 karakteres szöveg |

| 8.7 | > ASZ | Adószám | 20 karakteres szöveg |

| 9. | ITL | A bizonylat összes tételére vonatkozóan, tételenként | lista (max 1.000) |

| 9.1 | > NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 9.2 | > PN | a tételhez tartozó cikkszám | 50 karakteres szöveg |

| 9.3 | > UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, legfeljebb 4 tizedes pontossággal | 8+4 karakteres numerikus |

| 9.4 | > QY | a tételnél a bizonylaton szereplő mennyiség, maximum 4 tizedesjegy pontossággal | 8+4 karakteres numerikus |

| 9.5 | > IU | a tételnél a bizonylaton szereplő mennyiségi egység | 10 karakteres szöveges |

| 9.6 | > TY | Az adott tétel jellege: „v”: visszáru „vs”: visszáru sztornó „g”: göngyöleg visszaváltás „gs”: göngyöleg visszaváltás sztornó „f”: felár „fs”: felár sztornó „e”: engedmény „es”: engedmény sztornó | 5 karakteres szöveg |

| 9.7 | > SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 9.8 | > VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 9.9 | > RM | a tételsorra vonatkozó, legfeljebb 40-szer ismételhető megjegyzés mező | 50 karakteres szöveg |

| 10. | SUM | Bizonylat összesen forintban | 20 karakteres numerikus |

| 11. | PCR | a visszáru bizonylathoz kapcsolódó kerekítési különbözet összege forintban | 20 karakteres numerikus |

| 12. | TRA | Kétvállalkozós pénztárgépeknél használt mező (átvitel) | 20 karakteres numerikus |

| 13. | RCV | Kétvállalkozós pénztárgépeknél használt mező (áthozat) | 20 karakteres numerikus |

| 14. | PNU | Kétvállalkozós pénztárgépeknél használt mező (iker bizonylat száma) | 50 karakteres szöveg |

| 15. | DRC | a fióktartalom változásának adatai | lista |

| 15.1 | > FE1 | forint készpénz fióktartalom változása forintban | 20 karakteres numerikus |

| 15.2 | > FEV | a valutás fióktartalom változásának adatai (többszörözhető rekord) | lista, max. 10 |

| 15.2.1 | > > CAM | a valuta összege (valutában) | 10 karakteres numerikus |

| 15.2.2 | > > CTY | a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 15.2.3 | > > CRA | a valuta egy egységének forintban kifejezett, adózó által alkalmazott értéke (árfolyama) legfeljebb hat értékes jegy pontossággal | 20 karakteres numerikus |

| 15.2.4 | > > CFT | a valuta összegének értéke egész forintban, a feltüntetett árfolyamon számolva | 20 karakteres numerikus |

| 15.3 | > FE2 | bankkártya fiókegyenleg módosulása egész forintban | 20 karakteres numerikus |

| 15.4 | > FEE | egészségpénztári fiókegyenleg módosulása forintban, csak egyszerűsített számla esetén | 20 karakteres numerikus |

| 15.5 | > FE3 | fióktartalom módosulása egyéb fizetőeszköz tekintetében | lista, max. 20 |

| 15.5.1 | > > FEN | Fizetőeszköz neve: ERZSU - Erzsébet utalványesetén SZÉCHK - Széchenyi-kártya esetén AJÁND - Ajándék utalvány esetén HŰSÉG - Hűségkártya esetén SMART - Smartcard esetén GÖNGY - göngyölegjegy esetén KUPON - Kupon esetén egyéb esetben a fizetőeszköz nevét kell eltárolni | 20 karakteres szöveg |

| 15.5.2 | > > FES | Fióktartalom módosulása a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 16. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 17. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveg |

| 18. | CPY | A bizonylat példányszáma | 5 karakteres numerikus |

| 19. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0 |

| 20. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.9. Fogyasztási összesítő bizonylat

## Éttermi pénztárgépek kötelező szolgáltatása a fogyasztási összesítő bizonylat nyomtatási lehetősége. Kizárólag ezzel a bejegyzéstípussal naplózható a vevő részére átnyújtott, fogyasztott tételeket és összegeket tartalmazó nem adóügyi bizonylat.

## Fogyasztási összesítő bizonylat bejegyzés azonosító: FSN (gyakorló üzemmódban: FST)

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | BSR | Bizonylat számláló értéke. | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a bizonylat nyitásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | NSZ | a bizonylat száma F/bbbb/ccccc formátumban, ahol bbbb: adóügyi nap sorszáma ccccc: adott napon kibocsátott bizonylat sorszáma | 20 karakteres szöveg |

| 6. | ITL | A bizonylaton szereplő összes tételre vonatkozóan, tételenként | lista (max. 1.000) |

| 6.1 | > NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 6.2 | > PN | a tételhez tartozó cikkszám | 50 karakteres szöveg |

| 6.3 | > UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, legfelejbb négy tizedes pontossággal | 8+4 karakteres numerikus |

| 6.4 | > QY | a tételnél a bizonylaton szereplő mennyiség, maximum 4 tizedesjegy pontossággal | 8+4 karakteres numerikus |

| 6.5 | > IU | a tételnél a bizonylaton szereplő mennyiségi egység | 10 karakteres szöveges |

| 6.6 | > TY | Az adott tétel jellege egységesen: „x”, törölt tétel esetés „xs” | 5 karakteres szöveg |

| 6.7 | > SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 6.8 | > VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 6.9 | > RM | a tételsorra vonatkozó, legfeljebb 40-szer ismételhető megjegyzés mező | 50 karakteres szöveg |

| 7. | SUM | A bizonylaton szereplő tételsorok összege forintban | 20 karakteres numerikus |

| 8. | ZQQ | A nyomtatott bizonylaton szereplő további adatok eltárolásához használható, bizonylatonként maximum 199-szer feltüntethető egyedi mező | 200 karakteres szöveg |

| 9. | CPY | A bizonylat példányszáma | 5 karakteres szöveg |

| 10. | NAV | A bizonylaton szereplő NAV ellenőrző kód | 5 karakteres szöveg |

| 11. | WDN | Fogyasztásösszesítő egyedi azonosítója | 10 karakteres szöveg |

| 12. | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 13. | CTS | Időbélyeg, a bizonylat zárásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 14. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6.10. Egyéb, a pénztárgépen nyomtatott dokumentum

## A pénztárgépen lehetőség van egyéb dokumentumokat is kinyomtatni, amennyiben arra a pénztárgép kezelése, az üzletmenet, e rendelet előírásai vagy egyéb ok miatt szükség van. Az ilyen dokumentumok nem bizonylatolhatnak olyan eseményt, ami az adott értékesítési pont adóügyi elszámolását vagy fióktartalmát módosítaná.

## Az egyéb dokumentumok nyomtatását az alábbi bejegyzéssel kell naplózni az AEE naplóállományában.

## Egyéb dokumentum nyomtatása bejegyzés azonosító: EDN (gyakorló üzemmódban EDT)

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

## ”

6. melléklet a 9/2016. (III. 25.) NGM rendelethez

„5. melléklet a 48/2013. (XI. 15.) NGM rendelethez

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

I/1. Normál bejelentkezés

Az AEE a pénztárgép üzembe helyezett állapotában rendszeresen normál bejelentkezést hajt végre a NAV szerveréhez. A normál bejelentkezést haladéktalanul végre kell hajtani, ha a következő események közül legalább egy bekövetkezik:

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

A NAV szerver e mellékletben részletezett utasításainak végrehajtásáról az e mellékletben részletezett forgatókönyvek szerint az AEE az

„ANS~XXXXXXXXX~YY~HHHHHHHHHH” üzenetet küldi, ahol

YY – a NAV legutóbbi üzenetében foglaltakra vonatkozó visszajelzés kódja

Az YY lehetséges értékei:

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

A működtető szoftver frissítése során az e mellékletben részletezett forgatókönyv szerint az AEE az

„UPDREQ~NNN~XXXXXXXXX~HHHHHHHHHH” üzenetet küldi, ahol

NNN – a következő szoftver szelet sorszáma három számjegyen

I/5. A működtető szoftver adott verziójának elkérése

Az AEE a pénztárgép rendszerbe állítását követően a

„REQFW~V~XXXXXXXXX” üzenet elküldésével kezdeményezheti a NAV-nál a működtető szoftver adott verziójának telepítését, ahol

V – az igényelt szoftver verziószáma.

Ennek hatására az e mellékletben leírt forgatókönyv szerint megtörténik a szoftverfrissítés, amennyiben az lehetséges. A „V” helyén álló „L” az üzenetben a szoftver legfrissebb verzióját jelenti.

I/6. Első hitelesített bejelentkezés az AEE üzembe helyezésének folyamatában

Az AEE az üzembe helyezési folyamat részeként, az e mellékletben részletezett forgalmazás során a

„HELO~XXXXXXXXX~HHHHHHHHHH” üzenetet küldi.

I/7. Üzembe helyezési folyamat megindítása

Az AEE a rendszerbe állítását követően a

„DEFFST~XXXXXXXXX~UHK~HHHHHHHHHH” üzenettel, az üzemeltetés befejezését követően a

„DEFMOD~XXXXXXXXX~UHK~S~HHHHHHHHHH” üzenet elküldésével kezdeményezheti a NAV-nál az új üzembe helyezési folyamat megindítását, ahol

UHK – az üzembe helyezéshez előzőleg beszerzett 16 számjegyből álló üzembe helyezési kód

S – a legutóbbi napzárásra vonatkozó bejegyzést tartalmazó naplóállomány sorszáma.

Az új üzembe helyezési folyamat kizárólag a pénztárgép szervizmenüjéből indítható akkor, ha a pénztárgép hálózati áramforrásról üzemel, nincs nyitott adóügyi nap és a legutóbbi adóügyi nap zárását tartalmazó naplóállomány, valamint minden korábbi naplóállomány külső adathordozón az üzemeltető birtokában van. Az első vagy az új üzembe helyezés az e mellékletben részletezett forgalmazás eredményeként történhet meg.

I/8. Üzemeltetés befejezése

Az AEE a pénztárgép üzembe helyezett állapotában a

„SUSPEND~XXXXXXXXX” üzenettel kezdeményezi az üzemeltetés befejezését.

Az üzemeltetés befejezésének folyamata kizárólag akkor indítható, ha a pénztárgép hálózati áramforrásról üzemel. Az üzemeltetés befejezése az e mellékletben részletezett forgalmazás eredményeként valósulhat meg.

I/9. Üzemeltetés folytatása

Az AEE az üzemeltetés befejezését követően a

„SUSPUNDO~XXXXXXXXX” üzenettel kezdeményezi az üzemeltetés folytatását a meglévő üzemeltető vonatkozásában.

Az üzemeltetés folytatása az e mellékletben részletezett forgalmazás eredményeként valósulhat meg.

I/10. Az AEE-NAV kommunikáció tesztelése

Az AEE a pénztárgép rendszerbe állítását követően a

„PING~XXXXXXXXX” üzenet elküldésével tesztelheti az AEE-NAV kommunikációt.

Ezt az üzenetet kizárólag erre irányuló kezelői beavatkozás válthatja ki. A pénztárgépen lehetővé kell tenni olyan kezelői beavatkozást, ami ezen üzenet küldését váltja ki. A kommunikáció tesztelését az AEE egy percen belül legfeljebb kettő, egy napon belül legfeljebb száz alkalommal kezdeményezheti.

I/11. A NAV szerver által kért állapotjelentés üzenet

Az AEE a NAV szerver e mellékletben megjelölt utasítására az e mellékletben részletezett forgatókönyv szerint a

„STATUS~XXXXXXXXX~UZE=Q1~BLO=Q2~DEF=Q3~VAT=Q4~FRW=Q5~EUR=Q6~CON=Q7~UDC=Q8~PRN=Q9~STS=Q10~HHHHHHHHHH” üzenetet elküldésével jelenti az itt megjelölt folyamatok mindegyikének aktuális állapotát a pénztárgépen.

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

Az AEE az üzenetben szereplő folyamatok állapotának változásakor az e mellékletben leírt forgatókönyv szerint a

„STATUS~XXXXXXXXX~UZE=Q1~BLO=Q2~DEF=Q3~VAT=Q4~FRW=Q5~EUR=Q6~CON=Q7~UDC=Q8~PRN=Q9~STS=Q10” üzenetet elküldésével jelenti az itt megjelölt folyamatok mindegyikének aktuális állapotát a pénztárgépen. A Q1-Q10 lehetséges értékei és jelentésük azonos az I/11. üzenetnél leírtakkal.

II. Az AEE által fogadott üzenetek

II/1. Felszólítás azonnali bejelentkezésre

Az AEE részére küldött „CMSSL~XXXXXXXXX” üzenet szólítja fel a pénztárgépet azonnali elsőbbségi bejelentkezés végrehajtására.

Az üzenetet a bekapcsolt pénztárgépben működő AEE-nek nek mindenkor fogadnia kell, az üzenet fogadását követően haladéktalanul elsőbbségi bejelentkezést kell végrehajtania az e mellékletben részletezett forgatókönyv szerint.

II/2. Utasítás adatszolgáltatásra

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul a NAV a

„TRMNOW~F~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t azonnali adatszolgáltatásra, ahol

F – az a naplófájl sorszám, aminél nagyobb sorszámú naplóállományok küldésére vonatkozik az utasítás.

Erre az AEE haladéktalanul:

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

A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul a „PTGBLCK~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t a pénztárgép blokkolt állapotba hozására.

Ennek hatására az AEE blokkolja a pénztárgépet és az e mellékletben részletezett forgatókönyv szerinti választ küldi.

II/5. Utasítás a pénztárgép blokkolásának feloldására

A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul az „UNBLCK~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t a pénztárgép blokkolt állapotának feloldására.

Ennek hatására az AEE feloldja a pénztárgép blokkolt állapotát és az e mellékletben részletezett forgatókönyv szerinti választ küldi.

II/6. A pénztárgép működtető szoftver frissítése (firmware update)

A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul, vagy az AEE ezirányú igényére a „FRWUPD~ééééhhnnóóppmm~HHHHHHHHHH” üzenettel ad utasítást a működtető szoftver frissítésére, ahol

ééééhhnnóóppmm – a működtető szoftver telepítésére kijelölt végső időpont.

A működtető szoftver akkor telepítendő, ha nincs nyitott adóügyi nap a pénztárgépen. A pénztárgép nem teheti lehetővé adóügyi nap megnyitását a működtető szoftver sikeres telepítése nélkül az üzenetben megjelölt időpont után.

Az e mellékletben részletezett forgatókönyv szerint a NAV az egyes szoftver szeletek tulajdonságait az

„UPDDTL~NNN~CCCC~KKKKK~HHHHHHHHHH” üzenettel jelzi, ahol

NNN – a szoftver szeletek száma

CCCC – az adott szoftver szelet 32 bites CRC ellenőrző kódja 8 karakteren

KKKKK – a szoftver egészének SHA256 algoritmussal képzett ellenőrző kódja 64 karakteren

Az üzenetben a ~CCCC szakasz értelemszerűen ismétlődik annyiszor, ahány szeletből áll a szoftver.

II/7. Utasítás az egyes forgalmi gyűjtőkhöz kapcsolódó ÁFA kulcsok és jelölő címkék módosítására

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a NAV az egyes forgalmi gyűjtőkhöz tartozó ÁFA kulcsok módosítására a

„VATUPD~XXXXXXXXX~ééééhhnnóóppmm~A-AAAA-BBBB-CCCC~B-AAAA-BBBB-CCCC~C-AAAA-BBBB-CCCC~D-AAAA-BBBB-CCCC ~E-AAAA-BBBB-CCCC~HHHHHHHHHH” üzenet elküldésével ad utasítást az AEE részére, ahol

ééééhhnnóóppmm – Azon időpont éve, hónapja, napja, órája, perce, másodperce, amit követően az üzenetben megadott kulcsokat és kategória címkéket alkalmazni kell a pénztárgépen.

A, B ,C ,D ,E – a változással érintett forgalmi gyűjtők első karaktere

AAAA – a megadott időponttól az adott karakterrel kezdődő jelű forgalmi gyűjtőkre érvényes ÁFA-kulcs, százalékban kifejezve, százalékjel nélkül, szükség esetén tizedesvesszőt alkalmazva

BBBB – az adott ÁFA kulcshoz tartozó ÁFA tartalom, százalékban kifejezve, százalékjel nélkül, szükség esetén tizedesvesszőt alkalmazva

CCCC – az érintett forgalmi gyűjtőkre érvényes címke, aminek hossza maximálisan 8 karakter.

Egy gyűjtőhöz minden esetben egy „AAAA”, egy „BBBB” és egy „CCCC” érték tartozik.

A VATUPD üzenet minden esetben a gyűjtők teljes készletét tartalmazza függetlenül attól, hogy egy-egy gyűjtő adatai módosultak-e.

Az ÁFA kulcsok és kategória címkék módosítása a NAV üzenet alapján történik, azt a pénztárgépen más módon csak az egyedi mentesítéssel rendelkező gépeken lehet beállíthatóvá tenni.

Az ÁFA tábla frissítését a pénztárgépnek zárt adóügyi napnál kell végrehajtania úgy, hogy az üzenetben megjelölt időpontot követően nem végezheti el a pénztárgép új adóügyi nap megnyitását, ha nem került sor a frissítés érvényesítésére.

II/8. Utasítás üzemeltetői vagy telephely adatok frissítésére a pénztárgépen

A NAV az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a

„DEFUPD~XXXXXXXXX~P1a~P2bbb~P3ccc~P4ddd~P5eee~P6fff~P7ggg~P8hhh~HHHHHHHHHH” üzenettel ad utasítást a pénztárgép üzemeltetői vagy telephely adatainak módosítására. Az egyes paraméterek lehetséges értékeit és jelentését az alábbi táblázat foglalja össze:

Az üzenetben szereplő P1 paraméter értékétől függően a P2-P8 paraméterek jelentése az alábbi:

| P1-nél szereplő ’a’ értéke | Változás tárgya | bbb jelentése (P2) | ccc jelentése (P3) | ddd jelentése (P4) | eee jelentése (P5) | fff jelentése (P6) | ggg jelentése (P7) | hhh jelentése (P8) |

| 1 | Pénztárgép üzemeltető adatai, üzemanyagkúton használt kétvállalkozós pénztárgép esetén az üzemanyag tulajdonos adózó adatai változnak | Adózó adószáma 12345678- 1-12 formátumban | Adózó neve | Adózó székhelyének új irányító-száma | Adózó székhely település | Adózó székhely közterület neve | Adózó székhely közterület jellege | Adózó székhely házszám |

| 2 | Üzemanyagkúton használt kétvállalkozós pénztárgépen az üzemeltető adózó adatai változnak | Adózó adószáma 12345678- 1-12 formátumban | Adózó neve | Adózó székhelyének új irányító-száma | Adózó székhely település | Adózó székhely közterület neve | Adózó székhely közterület jellege | Adózó székhely házszám |

| 3 | a pénztárgép üzemeltetési helye változik | (üres) | Üzlet neve | Üzlet irányítószáma | Üzlet település | Üzlet közterület neve | Üzlet közterület jellege | Üzlet házszáma |

A pénztárgépnek az egyes paraméterek vonatkozásában az alábbi maximális hosszúságú értékeket kell kezelnie, figyelemmel az adatokban szerepeltethető karakterek tárigényére:

| Paraméter | Maximális hossz (karakter) |

| P1 | 1 |

| P2 | 20 |

| P3 | 100 |

| P4 | 6 |

| P5 | 50 |

| P6 | 50 |

| P7 | 20 |

| P8 | 50 |

Az érkezett fejlécadatok nyomtatásakor a pénztárgép nyomtatója egy-egy sortörés, illetve sorvégi kötőjel karaktert szúrhat be a megfelelő megjelenítés érdekében. A bizonylat fejlécére nyomtatott adatoknak meg kell egyezni az üzenetben elküldött adatokkal, az így beszúrt karakterektől eltekintve.

Az üzenet fogadását követően az AEE-nek gondoskodnia kell a jelzett módosítások érvényesítéséről a pénztárgépen úgy, hogy a módosítás végrehajtására zárt adóügyi nap mellett, az üzenet fogadását követő első napnyitás előtt kerüljön sor. A pénztárgépnek a módosítás végrehajtásáról az e mellékletben részletezett forgatókönyv szerinti választ kell küldenie a NAV-nak.

II/9. Utasítás az euró átálláshoz kapcsolódó dátumok beállítására

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a NAV az

EURD~XXXXXXXXX~D1~D2~D3~aaa~HHHHHHHHHH" üzenet megküldésével ad utasítást az euró átálláshoz kapcsolódó dátumok módosítására, ahol

D1 – a felkészülési időszak kezdete ééééhhnnóóppmm formátumban

D2 – az átállás időpontja ééééhhnnóóppmm formátumban

D3 – a kivezetési időszak vége ééééhhnnóóppmm formátumban

aaa – a rögzítésre kerülő HUF/EUR árfolyam hat értékes jegy pontossággal, tizedesvesszőt alkalmazva, legfeljebb 12 karakteren

Az üzenet fogadását követően az AEE-nek gondoskodnia kell a jelzett módosítások átvezetéséről a pénztárgépen és az e mellékletben részletezett forgatókönyv szerinti választ kell küldenie a NAV-nak.

II/10. Utasítás az AEE normál bejelentkezési gyakoriságának módosítására

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyv szerint a NAV a

„CONSET~XXXXXXXXX~DTNEXT~DTCONT~HHHHHHHHHH” üzenettel határozza meg az AEE következő normál bejelentkezésének időpontját és az azt követő bejelentkezési gyakoriságot, ahol

DTNEXT – Az AEE következő normál bejelentkezésének elvárt időpontja az üzenet fogadásától számítva, percben. Lehetséges értékei 1 és 9999 közötti egész számok.

DTCONT – Az AEE normál bejelentkezési gyakorisága az üzenet fogadását követő első normál bejelentkezést követően, percben. Lehetséges értékei 1 és 9999 közötti egész számok.

Az üzenet fogadását követően az AEE-nek gondoskodnia kell a jelzett módosítások átvezetéséről a pénztárgépen és az e mellékletben részletezett forgatókönyv szerinti választ kell küldenie a NAV-nak.

II/11. Utasítás az AEE alaphelyzetbe állítására

Az AEE normál vagy elsőbbségi bejelentkezésére, illetve egyéb üzeneteire válaszul az e mellékletben részletezett forgatókönyvek szerint a NAV az

„UPDCLR~XXXXXXXXX~R~HHHHHHHHHH” üzenettel ad utasítást az AEE-ben futó frissítési folyamatok egyikének vagy mindegyikének lezárására, illetve a jelzett paraméterek alapértelmezésre állítására, az alábbiak szerint:

| R értéke | Elvárt művelet |

| VAT | Lezárja és sikertelennek tekinti a futó ÁFA tábla frissítési folyamatot |

| FRW | Lezárja és sikertelennek tekinti a futó szoftverfrissítési folyamatot |

| DEF | Lezárja és sikertelennek tekinti a futó adózói adat frissítési folyamatot |

| EUR | Lezárja és sikertelennek tekinti a futó euró átállási dátum frissítési folyamatot a jövőbeni dátumokra vonatkozóan |

| PRN | Lezárja és sikertelennek tekinti a futó technikai tájékoztatás bizonylat nyomtatás folyamatot |

| CON | Az alapértelmezett 30 percre állítja a normál bejelentkezések időközét |

| FIL | Az alapértelmezett 1024 kilobájtra állítja a naplóállomány méretkorlátot |

| ALL | A fenti műveletek mindegyikét elvégzi. |

Az üzenet fogadását követően az AEE-nek végre kell hajtania az elvárt műveleteket.

II/12. Utasítás a naplófájl méretkorlát megváltoztatására

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyvek szerint a NAV a

FILESIZE~XXXXXXXXX~N~HHHHHHHHHH, üzenettel ad utasítást az AEE-ben vezetett naplóállomány méretkorlátjának beállítására, ahol

N – az új méretkorlát, kilobájtban megadva.

Amennyiben az AEE-ben vezetett naplófájl mérete eléri a megadott méretkorlátot, azt az AEE-nek le kell zárnia és a naplózást egy újonnan nyitott naplófájlban kell folytatnia. Az első FILESIZE üzenet fogadását megelőzően ez a méretkorlát 1024 kilobájt.

Az AEE működési sajátosságainak megfelelően alkalmazhat a FILESIZE utasításban megadottnál alacsonyabb méretkorlátot is.

II/13. Utasítás technikai tájékoztatás bizonylat nyomtatására

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul az e mellékletben részletezett forgatókönyvek szerint a NAV a

PRNT~XXXXXXXXX~SZOVEG~HHHHHHHHHH, üzenettel ad utasítást az adott üzenet kinyomtatására a pénztárgép nyugtanyomtatóján, ahol

SZOVEG – az üzenet legfeljebb 1024 karakter hosszúságú szövege, ami kizárólag betűket, számokat, valamint a szóköz, kérdőjel, felkiáltójel, pont, vessző, kötőjel, zárójel, alulvonás(_), csillag (*), százalék (%), egyenlő (=), plusz (+), bekezdésjel (§), törtvonal (/), visszaperjel (\) és kukac (@) karaktereket tartalmazhat.

Az üzenet fogadását követő első napzárást követően a pénztárgépnek ki kell nyomtatnia a kapott üzenetet a pénztárgép nyomtatóján. Az üzenetben szereplő „\n” karaktersorozatot „új sor” karakterként kell értelmezni a nyomtatáskor.

II/14. Utasítás állapotjelentésre

Az AEE normál vagy elsőbbségi bejelentkezésére válaszul a NAV a

„STSREQ~HHHHHHHHHH” üzenet elküldésével utasítja az AEE-t állapotjelentés küldésére.

Erre az AEE haladéktalanul elküldi a teljes körű állapotjelentést az e mellékletben részletezett forgatókönyv szerint.

III. Az AEE-NAV forgalmazások forgatókönyvei

A forgalmazási forgatókönyvek irányának oszlopában alkalmazott rövidítések és az egyes szerverekkel folytatott kommunikáció

MSG: A NAV üzenet szervere (https://opg.nav.gov.hu/msg)

NFL: A NAV naplófájl szervere (https://opg.nav.gov.hu/nfl)

SWU: A NAV szoftverfrissítés szerver (https://opg.nav.gov.hu/swu)

RMS: A NAV regisztrációs folyamathoz kapcsolódó üzenetszervere (https://opgreg.nav.gov.hu/msg)

REG: A NAV regisztrációs eljárás szervere (https://opgreg.nav.gov.hu/reg)

SSG: A NAV üzembe helyezési szervere (https://opgreg.nav.gov.hu/ssg)

Az egyes szerverekkel váltott üzenetek belső felépítése:

Az AEE→MSG, AEE→RMS, AEE→SWU, AEE→SSG irányú üzenetnél a tartalom típusa „urlencoded”, az üzenet karaktersorozatot tartalmazó form paraméter neve: „MSG”.

AEE→REG irányban a tartalom típusa „content type= multipart/form-data”, a fájlt azonosító elem neve: „REG”. Ekkor egy pkcs#7 formátumú fájl kerül továbbításra mely tartalmazza a regisztrációs fájlt, annak aláírását és a tanúsítványt.

AEE→NFL irányban a tartalomtípus „content type= multipart/form-data”, a fájlt azonosító elem neve: „NFL”. Ekkor egy pkcs#7 formátumú fájl kerül továbbításra mely tartalmazza a naplófájlt és annak aláírását. Ikervállalkozós pénztárgép esetén a második fájlt „NFL2” néven kell azonosítani és egy másik boundary-ba kell elhelyezni.

REG→AEE irányában, a pénztárgép rendszerbe állításakor leküldésre kerül az autentikációs tanúsítvány. A tartalom típusa „content type=application/octet-stream”, a leküldendő fájl tartalma közvetlen beleírásra kerül.

SWU→AEE irányban, szoftver frissítésekor leküldésre kerül(nek) a szoftver bináris fájl(ok). A tartalom típusa „content type=application/octet-stream”, a leküldendő szoftver fájl tartalma közvetlen beleírásra kerül.

MSG→AEE, NFL→AEE, SSG→AEE illetve RMS→AEE irányú kommunikáció során, a küldött üzenetre kapott válasz esetén, a tartalom típusa text/plain, az érkezett üzenet paraméternevet nem tartalmaz.

Az egyes forgatókönyvek közötti átmenet lehetősége

Az e mellékletben megadott forgatókönyvekben szereplő „ACK~03~HHHHHHHHHH” vagy „ACK~04~HHHHHHHHHH” visszaigazolás helyett a NAV szervernek lehetősége van az „ACK~09~HHHHHHHHHH” üzenetet küldeni. Ezt az üzenetet az addig lezajlott forgalmazásra vonatkozóan az AEE-nek úgy kell értelmezni, mint az „ACK~03~HHHHHHHHHH” vagy „ACK~04~HHHHHHHHHH” üzenetet, de az SSL kapcsolat bontása helyett haladéktalanul egy normál bejelentkezés üzenetet (TRMRDY) kell küldenie az MSG-nek.

Kommunikációs hiba kezelése a NAV szerver oldalon.

Ha az alább ismertetett forgatókönyvek szerinti forgalmazások során a NAV által küldött üzenetre az üzenet elküldését követő 30 percen belül az AEE nem küldi el a lehetséges válaszok egyikét, vagy a lehetséges válaszok helyett normál vagy elsőbbségi bejelentkező üzenetet küld, akkor a NAV szerver az adott üzenetet elveszettnek tekinti. A NAV szerver az elveszettnek tekintett üzenetet újra megkísérli elküldeni. Kétszeri sikertelen ismétlést követően az adott folyamatot a NAV szerver meghiúsultnak tekinti, a NAV szerver az AEE következő bejelentkezésekor UPDCLR utasítást küld.

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

Egy adózói vagy telephely adat frissítési folyamaton belül a NAV legfeljebb kettő, kétvállalkozós pénztárgépen legfeljebb három DEFUPD üzenetet küld úgy, hogy az üzenetek P1 paraméterének értéke különbözik. A pénztárgép adózói vagy telephely adatainak frissítésére irányuló üzenet fogadását a pénztárgép akkor és csak akkor tekintheti sikeresnek, ha a 6. lépésben jelölt visszaigazolás megtörtént, egyébként teljes egészében sikertelennek kell tekintenie.

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

A folyamat során a NAV elküldi a kért szoftver adatszeletet; a szeleteket a sikeres CRC-ellenőrzés után az AEE-nek össze kell raknia, majd ellenőriznie kell az adatállomány SHA256 algoritmussal képzett ellenőrző kódjának megfelelőségét.

Amennyiben a működtető szoftver letöltése nem kezdődött meg az FRWUPD üzenet fogadását követően 60 percen belül, az AEE-nek meg kell ismételnie a folyamatot az SSL csatorna kiépítése után a 4. lépéstől kezdve a FRWUPD üzenet fogadását követő 4 órán belül.

Szoftver frissítés elakadása esetén a már letöltött szeleteket nem kell újra letölteni, hacsak a NAV erre vonatkozóan az UPDCLR parancs kiadásával utasítást nem ad.

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

A regisztrációs fájlt az AEE tárolójára „0” sorszámmal, a naplóállományok elnevezésére vonatkozó előírás szerint elnevezve kell eltárolni. A regisztrációs állomány adatmezőinek feltöltésekor a rendelkezésre nem álló adózói adatokat megfelelő számú „0” karakterrel kell kitölteni. Az üzembe helyezési kód mezőjében 16 db „0” szerepeltetendő.

Amennyiben a 4a. lépésben szereplő üzenet elküldése már megtörtént, a sikertelenül zárult rendszerbe állítási folyamatot csak ugyanazokkal az adatokkal kísérelheti meg újra az AEE, amelyeket a sikertelenül zárult folyamatban küldte el. Ha a 11a. lépésben szereplő üzenet küldését követően az AEE újabb rendszerbe állítási folyamatot nem indíthat.

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

Az üzembe helyezési folyamat kizárólag akkor tekinthető sikeresen befejezettnek, ha sikeresen megtörtént minden olyan módosítás, amire a NAV utasítást adott, majd az AEE fogadta a 12a. lépésben szereplő visszaigazoló üzenetet. A pénztárgép adóügyi nap nyitását kizárólag a sikeresen lezárult üzembe helyezési folyamatot követően teheti lehetővé.

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

Az átszemélyesítés kizárólag akkor tekinthető sikeresen befejezettnek, ha sikeresen megtörtént minden olyan módosítás, amire a NAV utasítást adott, majd az AEE fogadta a 10a. lépésben szereplő visszaigazoló üzenetet. A pénztárgép adóügyi nap nyitását kizárólag a sikeresen lezárult üzembe helyezési folyamatot követően teheti lehetővé. Átszemélyesítés után a naplóállományok sorszámozása ismétlés és kihagyás nélkül folytatódik.

Sikertelenül zárult átszemélyesítés újra megkísérelhető.

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

Ha az üzemeltetés befejezése folyamat sikeresen lezárul, akkor újabb üzembe helyezésig, illetve az üzemeltetés folytatása folyamat lezárultáig a pénztárgép nem lehet alkalmas adóügyi nap megnyitására.

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

A sikertelenül zárult folyamat megismételhető.

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

A technikai tájékoztatás bizonylat nem adóügyi bizonylat.

19. eset: Az AEE-NAV kommunikáció tesztelése

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PING~XXXXXXXXXX | AEE→MSG |

| 3. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 4. | A pénztárgép operátori kijelzőjén megjelenik a „Kommunikációs csatorna él” felirat, majd 60 másodperc múlva az AEE bontja az SSL kapcsolatot. |

20. eset: A NAV állapotjelentést kér

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Az AEE bejelentkezése (elsőbbségi vagy normál) | PRIOR~YY~XXXXXXXXX~S~N~T vagy TRMRDY~XXXXXXXXX~S~N~T | AEE→MSG |

| 3. | Utasítás állapotjelentés adására | STSREQ~HHHHHHHHHH | MSG→AEE |

| 4. | Állapotjelentés adása | STATUS~XXXXXXXXX~UZE=Q1~BLO=Q2~DEF=Q3~VAT=Q4~FRW=Q5~EUR=Q6~CON=Q7~UDC=Q8~PRN=Q9~STS=Q10~HHHHHHHHHH | AEE→MSG |

| 5. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | MSG→AEE |

| 6. | Az AEE bontja az SSL kapcsolatot |

21. eset: Állapotjelentés

| Lépés | Leírás | Üzenet | Irány |

| 1. | Az AEE felépíti az SSL kapcsolatot |

| 2. | Állapotjelentés adása | STATUS~XXXXXXXXX~UZE=Q1~BLO=Q2~DEF=Q3~VAT=Q4~FRW=Q5~EUR=Q6~CON=Q7~UDC=Q8~PRN=Q9~STS=Q10 | AEE→SSG |

| 3. | NAV visszaigazolás | ACK~04~HHHHHHHHHH | SSG→AEE |

| 4. | Az AEE bontja az SSL kapcsolatot |

”
