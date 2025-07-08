## Felügyeleti Szolgáltató rendszerében AFE-ként tárolt adok szerkezetére vonatkozó követelmények

## 1) Az FSZ-nak az automatában keletkezett adatokat UTF-8-as kódlap szerinti karakterkódolású, digitálisan aláírt XML típusú naplóállományokban (p7b) kell tárolnia. Az XML állomány séma ellenőrző állományát (XSD állomány) a NAV közleményben teszi közzé.

## 2) Az FSZ-nak a NAV szerverétől kapott, 3. melléklet szerinti utasítás alapján történő adattovábbításkor a NAV által megadott azonosító számú AFE-hez tartozó és a még el nem küldött naplóállományok NAV szerverre küldésének folyamatát el kell indítania.

## 3) Az FSZ-nak minden általa felügyelt AFE-hez a naplóállományt a naplófájl megnyitásának időpontja szerinti AAAAAAAAA_BBBBBBBB_ééééhhnnóóppmm_s.p7b néven kell eltárolnia, ahol

## a) AAAAAAAAA: Az AFE AP száma 9 karakteren,

## b) BBBBBBBB: Az üzemeltető adó törzsszáma 8 karakteren,

## c) éééé: az év száma négy számjegyen,

## d) hh: a hónap sorszáma két számjegyen,

## e) nn: a nap sorszáma két számjegyen,

## f) óó: az óra száma két számjegyen,

## g) pp: a perc száma két számjegyen,

## h) mm: a másodperc száma két számjegyen,

## i) s: az állomány 1-től kezdődően, kihagyás és ismétlés nélkül képzett sorszáma a felügyelt AFE élettartama során.

## 4) A FSZ-nak az 1. pont szerinti, az AFE-kból érkező adatállományokhoz kölcsönösen egyértelműen kell hozzárendelnie az általa tárolt naplófájlokat. Az azonos AFE azonosítóhoz tartozó azonos sorszámú naplóállományokat kell összetartozónak tekinteni. Az összetartozó naplóállományok között a FSZ felelőssége biztosítani az AFE által küldött naplóállományból az értékesítési eseményekhez tartozó adatok maradéktalan átvételét a NAV felé küldött állományokba.

## 5) A jelen mellékletben meghatározott bejegyzéseket (továbbiakban: bejegyzések) a digitálisan aláírt XML állományban a NAV által közleményben közzétett XSD állományleíró struktúrának megfelelő tartalommal és szerkezetben kell elhelyezni.

## 6) A FSZ által létrehozott állományokban 32-nél kisebb kódú karakterek a CHR(10) sorvégjel és a CHR(13) sortörés karakter kivételével nem szerepelhetnek.

## 7) Minden bejegyzést az adott naplóállományban 1-től kezdődő folyamatos sorszámmal kell ellátni (bejegyzés sorszám). Az értékesítésre, a napzárásra, illetve az egyéb eltárolt adatokra vonatkozó bejegyzéseket az adott AFE vonatkozásában együtt futó, 1-től kezdődő, folyamatos sorszámozással is el kell látni (bizonylat sorszám).

## 8) A naplóállományban a numerikus értékeket a szükséges számú számjegyen, vezető nullák nélkül kell ábrázolni, kivéve ha ezzel ellentétes előírás szerepel adott adatnál. A pénznem adatok bejegyzésének formátuma forint esetében tagolás nélküli, egészre kerekített értékek tizedes nélkül, kivéve, ha ezzel ellentétes előírás szerepel adott adatnál. Az euróra történő átállást követően a pénzösszegre vonatkozó adatokat tagolás nélküli, két tizedesre kerekített, tizedesvesszővel elválasztott számokban kell tárolni.

## 9) A jelen mellékletben szereplő ellenőrző kódok képzésére az SHA256 algoritmust kell alkalmazni. Az algoritmus eredményeképpen előálló 64 karakteres kódban szereplő A-F hexadecimális számjegyeket minden esetben nagybetűként kell értelmezni és feltüntetni. Az SHA256 algoritmus bemenő adata az a karaktersorozat, amely az alábbi részekből tevődik össze az alábbi felsorolás sorrendjében:

## a) A bemenő karaktersorozat első hatvannégy karaktere az adott AFE vonatkozásában legutóbb lezárt naplóállomány utolsóként bejegyzett (LCL) bejegyzésének 64 karakteres ellenőrző kódja. Amennyiben még nem létezik legutóbb lezárt szöveges állomány, akkor a bemenő karaktersorozat első 64 karaktere 64 db „F”.

## b) A bemenő karaktersorozat 65-128. karaktere az adott bejegyzést megelőzően rögzített bejegyzés 64 karakteres ellenőrző kódja. Ha nem létezik az adott szöveges állományban előző bejegyzés, akkor a bemenő karaktersorozat 65-128. karaktere 64 db „F”.

## c) A bemenő karaktersorozat további karakterei az adott bejegyzés azonosítója, valamint minden mezőjének értéke a jelen mellékletben feltüntetett sorrendben, a mezőazonosító kódok nélkül.

## 10) Egy adott bejegyzésben minden mezőben fel kell tüntetni az abban szerepeltetendő adatot, ha az az adott konkrét esemény tekintetében releváns.

## 11) A naplófájlokban minden dátum/idő adatot az XML 1.0 szabvány szerinti „éééé-hh-nnTóó:pp:mm+óó:pp” formátumban kell feltüntetni, ahol az év, hónap, nap, óra, perc, másodperc minden esetben a helyi (magyar) idő szerint értendő. Téli időszámítás esetén az időzóna jelölésére a „+01:00”, nyári időszámítás esetén a „+02:00” jelölés használandó.

## 12) Az e mellékletben leírt szerkezetű naplóállomány verziószáma „X0006”.

## 13) Ha a vonatkozó sémadefinícióban kötelezőként szereplő mező értéke nem áll rendelkezésre vagy a mező az adott kontextusban nem értelmezhető, a naplóállományban az adott mezőt üres értékkel kell szerepeltetni. A nem kötelező mezőket az XML állományban nem kell szerepeltetni, amennyiben nincs releváns tartalmuk.

## 14) A naplóállományok megnyitását – minden esetben a naplóállományok első bejegyzéseként – az alábbi bejegyzéssel kell naplózni:

## Naplóállomány nyitása bejegyzés azonosító: LON

## 6K68573_0

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | APN | Az AFE AP száma | 9 karakteres szöveg |

| 4. | TSZ | Üzemeltető adó törzsszáma | 8 karakteres szöveg |

| 5. | LFN | Naplófájl sorszáma | 8 karakteres szám |

| 6. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 15) A automatában bekövetkező egyes eseményeket az alábbi bejegyzéssel kell naplózni:

## Bejegyzés azonosító: EVT

## 6K68573_1

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | EVC | Esemény kódja | 3 karakteres szöveg |

| 4. | EVD | Esemény leíró adata | üres / 400 karakteres szöveg |

| 5. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 16) A naplózott esemény jellegét az EVC mező kódolja az alábbiak szerint. Egyes eseményeknél az eseményt jellemző adatot is szerepeltetni kell az EVD mezőben az alábbiak szerint. Ha az esemény jellegéből következően nincs ilyen, az eseményt jellemző adat, akkor az EVD mező üres.

| Esemény | EVC mező értéke | EVD mezőben szereplő adat |

| Naplóállomány zárása (a naplóállomány utolsó bejegyzése) | LCL | (üres) |

| Az AFE a saját akkumulátoráról kezd működni (áramszünet kezdete) | POF | (üres) |

| Az AFE külső áramforrásról folytatja a működését (áramszünet vége) | PIN | (üres) |

| Az AFE saját áramforrása lemerül | BDN | (üres) |

| Az AFE a saját áramforrás lemerülése után újra működni kezd vagy működés közben újraindul | RST | „B”, ha az újraindulás az áramforrás lemerülése után megy végbe, „O” egyébként |

| Az automatában észlelt hiba miatt az automata blokkolt állapotba került | BLS | „N”, ha a blokkolásra a NAV adott utasítást, „E” egyébként. |

| Az automata hiba miatt történt blokkolt állapotának vége | BLF | „N”, ha a blokkolásra a NAV adott utasítást, „E” egyébként. |

| Üzenet küldése a NAV részére | MGO | Az üzenet szövege |

| Üzenet fogadása a NAV-tól | MGI | Az üzenet szövege |

| Euró üzemmód beállítása | EUR | (üres) |

| Automata szüneteltetés megkezdése | STB | A szüneteltetés végének várható dátuma |

| Automata szüneteltetés vége | STF | (üres) |

## 17) A NAV szerverről érkező tanúsítványok és kulcsok fogadására vonatkozó bejegyzések esetén az EVD mező tartalma a „CERT”, illetve a „KEY” karaktersorozat.

## 18) A NAV szerver részére küldött naplófájl esetén a bejegyzés EVD mezőjének tartalma a küldött állomány teljes neve.

## 19) Az AFE működése során minden naplóállományban legalább egyszer szerepeltetni kell az „AFE működési információi”, „AFE rendszerállapota”, illetve „AFE forgalmazási mérőszámai”, bejegyzéseket.

## 20) Az AFE működési információi bejegyzés szerkezete és adattartalma a következő:

## AFE működési információi bejegyzés azonosítója: INF

## 6K68573_3

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | DTY | AFE gyártói típusnév | 200 karakteres szöveg |

| 4. | DRV | AFE hardver verzió | 200 karakteres szöveg |

| 5. | DFW | AFE szoftver verzió | 5 karakteres szöveg |

| 6. | DFH | AFE-ben futó szoftver SHA256 algoritmussal kiszámított ellenőrző kódja | 64 karakteres szöveg |

| 7. | DFT | Az AFE-ben futó szoftver legutóbbi frissítésének időpontja. | szabványos dátum és idő adat másodperc pontossággal |

| 8. | DMT | Az AFE-ben lévő modem kiolvasott típus megnevezése, | 32 karakteres szöveg |

| 9. | DMF | Az AFE-ben lévő modem kiolvasott szoftver-verziója. | 200 karakteres szöveg |

| 10. | DME | Az AFE-ben lévő modem kiolvasott IMEI száma. | 50 karakteres szöveg |

| 11. | DMS | Az AFE-ben lévő SIM kiolvasott IMSI száma. | 50 karakteres szöveg |

| 12. | AKN | Akkumulátor gyári száma | 50 karakteres szöveg |

| 13. | TSZ | Üzemeltető adó törzsszáma | 20 karakteres szöveges |

| 14. | NAM | Üzemeltető neve | 100 karakteres szöveg |

| 15. | IRS | Üzemeltető székhely irányítószám | 6 karakteres szöveg |

| 16. | TEL | Üzemeltető székhely település | 50 karakteres szöveg |

| 17. | KZT | Üzemeltető székhely közterület neve | 50 karakteres szöveg |

| 18. | KZJ | Üzemeltető székhely közterület jellege | 20 karakteres szöveg |

| 19. | HSZ | Üzemeltető székhely házszám | 50 karakteres szöveg |

| 20. | VAT | Üres | - |

| 21. | GSM | A legutóbb használt cella egyedi azonosítója | 20 karakteres szöveg |

| 22. | TNA | Automata NAV által kiadott, U12345678 alakú regisztrációs száma | 9 karakteres szöveg |

| 23. | TZC | Automata telephely irányítószám | 6 karakteres szöveg |

| 24. | TCY | Automata telephely település | 50 karakteres szöveg |

| 25. | TKN | Automata telephely közterület neve | 50 karakteres szöveg |

| 26. | TKJ | Automata telephely közterület jellege | 20 karakteres szöveg |

| 27. | THH | Automata telephely házszám | 50 karakteres szöveg |

| 28. | DPH | Az automata hardver gyártói típusmegjelölése | 50 karakteres szöveg |

| 29. | DPV | Az automata hardververziója | 50 karakteres szöveg |

| 30. | DPF | Az AFE által támogatott automata vezérlési protokollok listája | 50 karakteres szöveg |

| 31. | DPS | Az automata által aktuálisan elfogadható fizetőeszközök: 1-forint készpénz (érme és/vagy bankjegy) 2-egyéb készpénz (érme és/vagy bankjegy) 4-bankkártya 8-zseton vagy egyéb értékesítést számláló eszköz A mezőbe a támogatott fizetőeszközök itt jelzett értékének összegét kell feltüntetni. | 64 karakteres szöveg |

| 32. | VCC | A legutóbb használt üzembe helyezési kód | 16 karakteres szöveg |

| 33. | MIS | Az automatán az AFE vonatkozásában a legutóbbi beavatkozást végző AFE telepítő egyedi azonosítószáma | 12 karakteres szöveg |

| 34. | APN | Az AFE AP száma | 9 karakteres szöveg |

| 35. | COM | Az AFE által használt kommunikációs protokoll verziószáma | Cnnnn, ahol nnnn a kommunikációs protokoll verziószáma. |

| 36. | XMV | A legfrissebb séma verziószáma, aminek a FSZ által képzett naplóállományok megfelelnek. | Xnnnn, ahol nnnn a séma verziószáma. |

| 37. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 21) Az e rendelet 3. mellékletében foglaltak szerint kommunikáló FSZ esetén a COM mezőben „C0002” értéket kell szerepeltetni.

## 22) Az automata rendszerállapotát a következő tartalmú és szerkezetű bejegyzés naplózza:

## AFE rendszerállapota bejegyzés azonosító: STA

## 6K68573_4

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | SST | Automata állapot: „0”, ha az AFE működik és nincs blokkolt állapotban „1”, ha az AFE blokkolt állapotban van „2”, ha az AFE hibás | 1 karakteres szöveg |

| 4. | SFL | Az AFE-ben működő adattárolón lévő szabad tároló kapacitás (Kbyte) | 10 karakteres numerikus |

| 5. | SSG | Az AFE-ben működő modem által mért hálózati térerőt (-1)dBm - (-199)dBm-ig terjedő skálán negatív egész számmal ábrázolva. | 4 karakteres numerikus |

| 6. | SAC | Az AFE akkumulátor töltöttség egész számmal, vezető nullák nélkül (%) | 3 karakteres numerikus |

| 7. | SMT | GSM hálózatból kiolvasott illetve a FSZ idő szerverétől kapott pontos idő | szabványos dátum és idő adat másodperc pontossággal |

| 8. | SCC | Automatában az utolsó STA rekord küldése óta jelentkezett hibák belső kódjainak listája. | 400 karakteres szöveg a gyártó által kialakított struktúrában |

| 9. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 23) Az AFE forgalmazási mérőszámai bejegyzés tartalma és szerkezete a következő:

## AFE forgalmazási mérőszámai bejegyzés azonosító: OPR

## 6K68573_5

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám (bejegyzés sorszáma) naplófájlon belül (1-től sorszámozva) | 5 karakteres szám |

| 2. | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 3. | ODS | A legutóbbi bekapcsolás óta a modem által küldött bájtok száma, beleértve a megszakadt kapcsolatok adatait is. | 12 karakteres numerikus |

| 4. | ODR | A legutóbbi bekapcsolás óta a modem által fogadott bájtok számát, beleértve a megszakadt kapcsolatok adatait is, | 12 karakteres numerikus |

| 5. | ODF | A legutóbbi bekapcsolás óta a mobil adatkapcsolat kiépítésére tett sikertelen kísérletek száma. | 5 karakteres numerikus |

| 6. | OSF | A legutóbbi bekapcsolás óta az SSL adatcsatorna felépítésére tett sikertelen kísérletek száma. | 5 karakteres numerikus |

| 7. | NET | A legutóbbi bejelentkezés során használt átviteli technológia: 0 – GSM 1 – 2G technológia 2 – 2,5G technológia 3 – 3G technológia 4 – 4G technológia | 1 karakteres szöveg |

| 8. | PRV | A legutóbbi bejelentkezés során használt infrastruktúrát biztosító fizikai mobilszolgáltató: 0 – Magyar Telekom 1 – Telenor 2 – Vodafone 3 – Egyéb | 1 karakteres szöveg |

| 9. | OCC | AFE belső mérőszámai, ahol „N” a belső mérőszám azonosítóját, „E” a mért paraméter értékét jelenti. | 400 karakteres szöveg a Felügyeleti Szolgáltató által definiált struktúrában |

| 10. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 24) Az AFE órájának bármilyen okból történő átállítását az alábbi bejegyzéssel kell naplózni.

## Óraállítás bejegyzés azonosító: TUD

## 6K68573_6

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | max 5 hosszú numerikus |

| 2. | OLD | Azaz idő, amikor az átállítás régi idő szerint bekövetkezik. | szabványos dátum és idő adat másodperc pontossággal |

| 3. | NEW | Beállított új idő | szabványos dátum és idő adat másodperc pontossággal |

| 4. | CHT | ha a rendszer nem diszkréten változtatja az időt, hanem egy időtávon gyorsítja vagy lassítja az időt, akkor az átmenet ideje másodpercben | 10 karakteres numerikus |

| 5. | CAS | az időállítás módja: 1-GSM szinkronizáció, 3-Üzemeltető által módosítva 5-Egyéb automatikus szinkronizáció | 1-5 számok egyike |

| 6. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 25) Az automatán lebonyolított értékesítést az alább meghatározott szerkezetű és adattartalmú bejegyzésekkel kell naplózni az AFE naplóállományában.

## Értékesítés bejegyzés azonosító: NYN

## 6K68573_7

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | 5 karakteres szám |

| 2. | BSR | Bizonylat sorszám | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, az értékesítés kezdetének pontos ideje az AFE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | Az üzemeltető adóalany adó törzsszáma | 8 karakteres szöveg |

| 5. | NSZ | Az értékesítés sorszáma bbbb/ccccc formátumban, ahol bbbb: adóügyi nap sorszáma ccccc: adott napon végzett értékesítés sorszáma | 10 karakteres szöveg |

| 6. | ITL | Az értékesítésben szereplő összes tételre vonatkozóan, tételenként | lista (max. 1.000) |

| 6.1 | > NA | a tétel megnevezése, ha rendelkezésre áll | 200 karakteres szöveg |

| 6.2 | > PN | a tételhez tartozó cikkszám, ha rendelkezésre áll | 50 karakteres szöveg |

| 6.3 | > UN | a tétel egységára forintban, tizedesvesszővel elválasztva, legfeljebb négy tizedes pontossággal | 8+4 karakteres numerikus |

| 6.4 | > QY | a tétel mennyisége, maximum 4 tizedesjegy pontossággal | 8+4 karakteres numerikus |

| 6.5 | > IU | a tétel mennyiségi egysége | 10 karakteres szöveges |

| 6.6 | > TY | Egységesen üres („”) | üres |

| 6.7 | > SU | a tételnél szereplő összérték forintban | 20 karakteres numerikus |

| 6.8 | > VC | A tételnél feltüntetett forgalmi gyűjtő jele három karakteren. Ha nem áll rendelkezésre, akkor egységesen „V00” | 3 karakteres szöveg |

| 6.9 | > RM | a tételsorra vonatkozó, legfeljebb 40-szer ismételhető megjegyzés mező | 50 karakteres szöveg |

| 7. | DRC | a bevétel változásának adatai | lista, használata nem kötelező |

| 7.1 | > FE1 | üres, vagy a forint készpénz bevétel változása forintban | 20 karakteres numerikus |

| 7.2 | > FEV | üres, vagy a valutás bevétel változásának adatai | lista, max. 10 |

| 7.2.1 | > > CAM | üres, vagy a valuta összege (valutában) | 10 karakteres numerikus |

| 7.2.2 | > > CTY | üres, vagy a valuta neme 3 karakteren, nagybetűvel, a Magyar Nemzeti Bank jelölése szerint (pl. EUR) | 3 karakteres szöveg |

| 7.2.3 | > > CRA | üres, vagy a valuta egy egységének forintban kifejezett, adózó által alkalmazott értéke (árfolyama) legfeljebb hat értékes jegy pontossággal | 20 karakteres numerikus |

| 7.2.4 | > > CFT | üres, vagy a valuta összegének értéke egész forintban, a feltüntetett árfolyamon számolva | 20 karakteres numerikus |

| 7.3 | > FE2 | üres, vagy bankkártyás bevétel módosulása egész forintban | 20 karakteres numerikus |

| 7.4 | > FE3 | Üres, vagy a bevétel módosulása egyéb fizetőeszköz tekintetében | lista, max. 20 |

| 7.5.1 | > > FEN | Üres, vagy a fizetőeszköz neve | 20 karakteres szöveg |

| 7.5.2 | > > FES | Üres, vagy a bevétel módosulása a fizetőeszköz tekintetében, forintban | 20 karakteres numerikus |

| 8. | RND | Egységesen „0” érték. | 20 karakteres numerikus |

| 9. | SUM | A bizonylaton szereplő tételsorok összege forintban | 20 karakteres numerikus |

| 10. | NYL | Üres | 20 karakteres szöveg |

| 11. | NAV | A naplóállományban szereplő előző bejegyzésre képzett ellenőrző kód 8., 24., 32., 48. és 64. karaktere | 5 karakteres szöveg |

| 12. | CPY | Egységesen „1” | 5 karakteres numerikus |

| 13. | CNC | Értékesítés megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1, egyébként 0. |

| 14. | CTS | Időbélyeg, az értékesítés zárásának pontos ideje az AFE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 15. | HSH | Ellenőrző kód | 64 HEXA karakter |

## 26) Napi forgalmi jelentés bejegyzést minden üzemeltetési napon egyszer el kell helyezni a naplóállományában úgy, hogy két bejegyzés között legfeljebb 25 óra telhet el. A napi forgalmi jelentést az alábbi bejegyzéssel kell naplózni az AFE naplóállományában.

## Napi forgalmi jelentés bejegyzés azonosító: NFN

## 6K68573_8

| Sorszám | Mező azonosító | Mező tartalmának leírása | Formátum |

| 1. | RSR | Bejegyzés sorszám | 5 karakteres szám |

| 2. | BSR | Bizonylat sorszám | 10 karakteres numerikus |

| 3. | DTS | Időbélyeg, a napzárás pontos ideje az AFE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 4. | TSZ | Az üzemeltető adó törzsszáma | 8 karakteres szöveg |

| 5. | ZSZ | a zárás sorszáma négy karakteren, szükség esetén vezető nullákkal feltöltve | 4 karakteres szöveg |

| 6. | GYF | Napi bevétel forgalmi gyűjtők szerinti összesítése | lista |

| 7. | > GYJ | Forgalmi gyűjtő jele 3 karakteren (A00..E99) | 3 karakteres szöveg |

| 8. | > GYE | Az adott forgalmi gyűjtőbe tartozó napi tételek bruttó összértéke | 20 karakteres numerikus |

| 9. | NSF | a napi forgalom összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 10. | NDB | a napi értékesítések száma | 20 karakteres numerikus |

| 11. | NIR | napi megszakított értékesítések száma | 10 karakteres numerikus |

| 12. | NSG | a göngyölített forgalom | 50 karakteres numerikus |

| 13. | NAV | A naplóállományban szereplő előző bejegyzésre képzett ellenőrző kód 8., 24., 32., 48. és 64. karaktere | 5 karakteres szöveg |

| 14. | CPY | Egységesen „1” | 5 karakteres numerikus |

| 15. | CNC | Egységesen „0” | 1 karakteres szöveg |

| 16. | HSH | Ellenőrző kód | 64 HEXA karakter |

5. melléklet a 31/2016. (IX. 2.) NGM rendelethez[^41]

Igazgatási szolgáltatási díjak

|  | A | B | C |

| 1. | Tételszám | Megnevezés | Díjtétel |

| 2. | 1. | Felügyeleti szolgáltatói engedély kiadása | engedélyenként 600 000 Ft |

| 3. | 2. | Felügyeleti szolgáltatói engedély módosítása (egy éven belül az első módosítás) | 300 000 Ft |

| 4. | 3. | Felügyeleti szolgáltatói engedély módosítása [egy éven belül a második, vagy az azt követő módosítás(ok)] | módosításonként 400 000 Ft |

[^41]: Az 5. melléklet a 7/2018. (III. 19.) NGM rendelet 3. §-ával megállapított szöveg.
