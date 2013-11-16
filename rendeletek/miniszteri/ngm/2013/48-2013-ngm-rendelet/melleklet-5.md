## Az Adóügyi Ellenőrző Egységben (AEE) tárolt bizonylati adatok tartalmára és szerkezetére vonatkozó előírások

## 1. Az AEE-nek a pénztárgépben keletkezett adatokat UTF-8-as kódlap szerinti karakterkódolású, XML típusú naplóállományokban kell tárolnia. Az állomány struktúrájának leírását és a séma ellenőrző állományt (XSD állomány) a NAV közleményben teszi közzé.

## 2. Az AEE-nek a NAV szerverétől kapott, 5. melléklet szerinti utasítás alapján történő adattovábbításkor az AEE-n lévő összes adózó nyitott szöveges állományát le kell zárnia, és azt a NAV szervere felé el kell küldenie. Az AEE-nek minden állomány lezárását követően adózónként új szöveges állományt kell nyitnia, és az adott adózóhoz rendelt szöveges állományban kell folytatnia a bejegyzések rögzítését. Az AEE-nek a szöveges állományt annak megnyitását követő 24 óra elteltével akkor is le kell zárnia és újat kell nyitnia, ha ezen idő alatt nem történt adattovábbítás a NAV szervere felé.

## 3. Az AEE-nek az elküldött állományt az elküldés megkezdésének időpontja szerinti AAAAAAAAA_BBBBBBBB_ééééhhnnóóppmm_s.xml néven kell eltárolnia, ahol

## a) AAAAAAAAA: A pénztárgép AP száma 9 karakteren,

## b) BBBBBBBB: Az adózó törzsszáma 8 karakteren

## c) éééé: az év száma négy számjegyen,

## d) hh: a hónap sorszáma két számjegyen,

## e) nn: a nap sorszáma két számjegyen,

## f) óó: az óra száma két számjegyen,

## g) pp: a perc száma két számjegyen,

## h) mm: a másodperc száma két számjegyen,

## i) s: az állomány 1-től kezdődően, kihagyás és ismétlés nélkül képzett sorszáma az AEE élettartama során.

## 4. A jelen mellékletben meghatározott bejegyzések (továbbiakban bejegyzés típusok) tartalmára vonatkozó egységes szabályok a következők.

## 4.1. A bejegyzéseket az XML állományban a NAV által közleményben közzétett XSD állományleíró struktúrának megfelelően kell megvalósítani.

## 4.2. Az AEE által létrehozott állományokban 32-nél kisebb kódú karakterek a CHR(10) sorvégjel kivételével nem szerepelhetnek.

## 4.3. Minden bejegyzést az adott naplóállományban 1-től kezdődő folyamatos sorszámmal kell ellátni.

## 4.4. A naplóállományban a numerikus értékeket a szükséges számú számjegyen, vezető nullák nélkül kell ábrázolni, kivéve ha ezzel ellentétes előírás szerepel adott adatnál. A pénznem adatok bejegyzésének formátuma forint esetében tagolás nélkül egészre kerekített értékek tizedes nélkül, kivéve ha ezzel ellentétes előírás szerepel adott adatnál. Az EURO-ra történő átállást követően tagolás nélkül két tizedesre kerekítve, tizedesvesszővel elválasztva.

## 4.5. A jelen mellékletben szereplő ellenőrző kódok képzésére az SHA256 algoritmust kell alkalmazni. Az algoritmus eredményeképpen előálló 64 karakteres kódban szereplő A-F hexadecimális számjegyeket minden esetben nagybetűkként kell értelmezni és feltüntetni. Az SHA256 algoritmus bemenő adata az a karaktersorozat, amely az alábbi részekből tevődik össze az alábbi felsorolás sorrendjében:

## a) A bemenő karaktersorozat első hatvannégy karaktere az AEE által legutóbb lezárt szöveges állomány utolsóként bejegyzett (LCL) bejegyzésének 64 karakteres ellenőrző kódja. Amennyiben még nem létezik legutóbb lezárt szöveges állomány, akkor a bemenő karaktersorozat első 64 karaktere 64 db „F”.

## b) A bemenő karaktersorozat 65-128. karaktere az adott bejegyzést megelőzően rögzített bejegyzésének 64 karakteres ellenőrző kódja. Ha nem létezik az adott szöveges állományban előző bejegyzés, akkor a bemenő karaktersorozat 65-128. karaktere 64 db „F”.

## c) A bemenő karaktersorozat további karakterei az adott bejegyzés azonosítója, 4.3. pont szerinti sorszáma, valamint minden mezőjének értéke a jelen mellékletben feltüntetett sorrendben, a mezőazonosító kódok nélkül.

## 5. Az AEE-nek szöveges állomány nyitásakor, minden esetben a szöveges állomány első

## bejegyzése

## Bejegyzés azonosító: LON

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a. | RAZ | Bejegyzés azonosító: LON | 3 karakteres szöveg |

| 3. | b | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 4. | c | APN | Pénztárgép AP száma | 9 karakteres szöveg |

| 5. | d | TSZ | Üzemeltető törzsszáma (kétvállalkozós pénztárgép esetén az üzemanyag tulajdonos törzsszáma) | 8 karakteres szöveg |

| 6. | e | THT | TSZ: kétvállalkozós pénztárgép esetén az üzlet üzemeltetőjének törzsszáma | 8 karakteres szöveg |

| 7. | f | HSH | Ellenőrző kód | 64 HEXA karakter |

## 6. A pénztárgépben bekövetkezett események naplózására

## Bejegyzés azonosító: EVT

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a. | RAZ | Bejegyzés azonosító: EVT | 3 karakteres szöveg |

| 3. | b | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 4. | c | EVC | Esemény kódja | 3 karakteres szöveg |

| 5. | d | EVD | Esemény leíró adata | üres / 200 karakteres szöveg |

| 6. | e | HSH | Ellenőrző kód | 64 HEXA karakter |

## EVC lehetséges értékei:

## 1. LCL: Az AEE szöveges állomány zárásakor, minden esetben a szöveges állomány utolsó bejegyzéseként

## 2. PIN: Az AEE a pénztárgép áramellátásának megindulása és az AEE saját áramforrásról történő működésének vége esetén

## 3. POF: Az AEE a pénztárgép áramellátásának megszűnése és az AEE saját áramforrásról történő működésének kezdete esetén

## 4. BDN: Az AEE saját áramforrás lemerülése és a pénztárgépről érkező áramellátás megszűnése esetén

## 5. RST: Az AEE saját áramforrás lemerülése utáni első üzemelés elindulásakor

## 6. BLS: Pénztárgép blokkolt állapotba került

## 7. BLF: Pénztárgép blokkolt állapotba megszűnése esetén

## 8. TRI: Pénztárgép gyakorló üzemmódba kerülése esetén

## 9. TRF: Pénztárgép gyakorló üzemmódba kerülés megszűnése

## 10. CHO: Pénztárnyitás esetén

## 11. MGI: NAV szerverétől érkező üzenet esetén

## 12. MGO: NAV szerverének küldött üzenet esetén

## EVD lehetséges értékei

## CHO → Pénztár nyitó pénzkészlet forintban

## MGI → teljes fogadott üzenet

## MGO → teljes küldött üzenet

## egyéb esetekben nem töltendő

## 7. A pénztárgép műszaki jellemzőiről szóló információk, amelyeket naponta egyszer kell rögzíteni az aktuálisan nyitott naplóállományba.

## Bejegyzés azonosító: INF

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a. | RAZ | Bejegyzés azonosító: INF | 3 karakteres szöveg |

| 3. | b | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 4. | c | DTY | AEE gyártói típusnév | 200 karakteres szöveg |

| 5. | d | DRV | AEE hardver verzió | 200 karakteres szöveg |

| 6. | e | DFW | AEE szoftver verzió | 200 karakteres szöveg |

| 7. | f | DFH | AEE egységben futó szoftver SHA256 algoritmussal kiszámított ellenőrző kódja | 64 karakteres szöveg |

| 8. | g | DFT | Az AEE egységben futó szoftver legutóbbi frissítésének időpontja. | szabványos dátum és idő adat másodperc pontossággal |

| 9. | h | DMT | Az AEE egységben lévő modem kiolvasott típus megnevezése, | 32 karakteres szöveg |

| 10. | i | DMF | Az AEE egységben lévő modem kiolvasott szoftver-verziója. | 200 karakteres szöveg |

| 11. | j | DME | Az AEE egységben lévő modem kiolvasott IMEI száma. | 50 karakteres szöveg |

| 12. | k | DMS | Az AEE egységben lévő SIM kiolvasott IMSI száma. | 50 karakteres szöveg |

| 13. | l | TZC | Pénztárgép telephely irányítószám | 6 karakteres szöveg |

| 14. | m | TCY | Pénztárgép telephely település | 50 karakteres szöveg |

| 15. | n | TKN | Pénztárgép telephely közterület neve | 50 karakteres szöveg |

| 16. | o | TKJ | Pénztárgép telephely közterület jellege | 50 karakteres szöveg |

| 17. | p | THH | Pénztárgép telephely házszám | 10 karakteres szöveg |

| 18. | q | DPH | A pénztárgép hardver gyártói típusmegjelölése | 50 karakteres szöveg |

| 19. | r | DPV | A pénztárgép hardver verziója | 50 karakteres szöveg |

| 20. | s | DPF | A pénztárgépben futó szoftver verziója | 50 karakteres szöveg |

| 21. | t | DPS | A pénztárgépben futó szoftver SHA256 algoritmussal kiszámított ellenőrző kódja | 64 karakteres szöveg |

| 22. | u | VCC | Üzembehelyezési kód | 50 karakteres szöveg |

| 23. | w | APN | Pénztárgép AP száma | 9 karakteres szöveg |

| 24. | x | HSH | Ellenőrző kód | 64 HEXA karakter |

## 8. A pénztárgép rendszerállapot statisztika adatok, amelyeket naponta egyszer kell rögzíteni az aktuálisan nyitott naplóállományba

## Bejegyzés azonosító: STA

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a. | RAZ | Bejegyzés azonosító: STA | 3 karakteres szöveg |

| 3. | b | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 4. | c | SST | Pénztárgép állapot | 5 karakteres szöveg |

| 5. | d | SFL | Az AEE egységben működő SD kártyán lévő szabad tároló kapacitás (Kbyte) | 10 karakteres numerikus |

| 6. | e | SSG | Az AEE-ben működő modem által mért hálózati térerőt 0-100-ig terjedő skálán normalizálva, egész számmal ábrázolva. | 3 karakteres numerikus |

| 7. | f | SAC | Akkumulátor töltöttség egész számmal, vezető nullák nélkül (%) | 3 karakteres numerikus |

| 8. | g | SMT | GSM hálózatból kiolvasott pontos idő | szabványos dátum és idő adat másodperc pontossággal |

| 9. | h | SCC | Pénztárgépben az utolsó STA rekord küldése óta jelentkezett hibák belső kódjainak listája. | R01n~R99n... |

| 10. | i | HSH | Ellenőrző kód | 64 HEXA karakter |

## SST lehetséges értékei:

## 1. „0”, ha a pénztárgép működik és nincs blokkolva

## 2. „1”, ha a pénztárgép blokkolt állapotban van

## 3. „2”, ha a pénztárgép hibás állapotban van

## 9. A pénztárgép műszaki mérőszámai, amelyeket naponta egyszer kell rögzíteni az aktuálisan nyitott naplóállományba.

## Rekord azonosító: OPR

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a. | RAZ | Bejegyzés azonosító: OPR | 3 karakteres szöveg |

| 3. | b | DTS | Időbélyeg | szabványos dátum és idő adat másodperc pontossággal |

| 4. | c | ODS | A legutóbbi bekapcsolás óta a modem által küldött bájtok száma, beleértve a megszakadt kapcsolatok adatait is. | 12 karakteres numerikus |

| 5. | d | ODR | A legutóbbi bekapcsolás óta a modem által fogadott bájtok számát, beleértve a megszakadt kapcsolatok adatait is, | 12 karakteres numerikus |

| 6. | e | ODF | A legutóbbi bekapcsolás óta a mobil adatkapcsolat kiépítésére tett sikertelen kísérletek száma. | 5 karakteres numerikus |

| 7. | f | OSF | A legutóbbi bekapcsolás óta az SSL adatcsatorna felépítésére tett sikertelen kísérletek száma. | 5 karakteres numerikus |

| 8. | g | OCC | AEE egység belső mérőszámai, ahol „N” a belső mérőszám azonosítóját, „E” a mért paraméter értékét jelenti. | N01n#N99n... - 20 karakteres szöveg E01n#E99n... - 50 karakteres szöveg |

| 9. | h | HSH | Ellenőrző kód | 64 HEXA karakter |

## 10. Nyugta vagy egyszerűsített számla

## Bejegyzés azonosító:

## - Nyugta esetén: NYN

## - Egyszerűsített számla esetén: ESN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a. | RAZ | Bejegyzés azonosító: NYN vagy ESN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat nyitásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | NSZ | a bizonylat száma 1234/00001 formátumban | 10 karakteres szöveg |

| 7. | f |  | A bizonylaton szereplő összes tételre vonatkozóan, tételenként |  |

| 8. | fa | NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 9. | fb | UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, két tizedes pontossággal | 20 karakteres numerikus |

| 10. | fc | QY | a tételnél a bizonylaton szereplő mennyiség | 5 karakteres numerikus |

| 11. | fd | SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 12. | fe | VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 13. | g |  | A bizonylaton szereplő összes törölt tételre vonatkozóan, tételenként |  |

| 14. | ga | NA | a törölt tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 15. | gb | UN | a törölt tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, két tizedes pontossággal | 20 karakteres numerikus |

| 16. | gc | QY | a törölt tételnél a bizonylaton szereplő mennyiség | 5 karakteres numerikus |

| 17. | gd | SU | a törölt tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 18. | ge | VC | a törölt tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 19. | h | PMD | a fizetési mód jele, ami készpénz esetén „1”, bankkártya esetén „2”, egyéb fizetési mód esetén „3”. n: az adott fizetési móddal fizetett részösszeg, egész forintban számolva | FM1n#FM3n |

| 20. | i | GYJ | nyugta tartalma gyűjtőnként, kizárólag az adott bizonylaton ténylegesen használt gyűjtőkre, vonatkozólag, ahol n: a bizonylaton szereplő tételek bruttó összege az adott gyűjtőben, egész forintban számolva | A01n#E99n |

| 21. | j | SUM | a bizonylaton szereplő bruttó összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül | 20 karakteres numerikus |

| 22. | k | TAX | az adott bizonylat forgalmi gyűjtőnkénti bruttó összege YYYn alakban, ahol: YYY: a forgalmi gyűjtő jele három karakteren, n: a bizonylaton szereplő tételek bruttó összege az adott forgalmi gyűjtőben, egész forintban számolva | X01YYYn#X99YYYn |

| 23. | l | DCN | a bizonylaton szereplő összes engedmény összege, egész forintban számolva, ha van ilyen adat. | 20 karakteres numerikus |

| 24. | m | RND | a bizonylaton szereplő kerekítés összege, egész forintban számolva, szükség esetén negatív előjellel, ha van ilyen adat. | 20 karakteres numerikus |

| 25. | n | HCN | a vásárlói kártya, hűségkártya azonosítója | 50 karakteres szöveg |

| 26. | o | VDA | Egyszerűsített számla esetén a termék beszerzőjének, szolgáltatás igénybevevőjének adatai az ÁFA tv. rendelkezései szerint | 200 karakteres szöveg |

| 27. | p | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z99X... |

| 28. | q | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 29. | r | CTS | Időbélyeg, a bizonylat zárásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 30. | s | HSH | Ellenőrző kód | 64 HEXA karakter |

## 11. Napi forgalmi jelentés

## Bejegyzés azonosító: NFN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: NFN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | f | ZSZ | a zárás sorszáma négy karakteren, szükség esetén vezető nullákkal feltöltve | 4 karakteres szöveg |

| 7. | g | GYJ | a napi forgalom összesen forgalmi gyűjtőnként, ahol n: a bizonylaton szereplő tételek bruttó összege az adott forgalmi gyűjtőben, egész forintban számolva | A01n#E99n |

| 8. | h | NSF | a napi forgalom összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 9. | i | NSH | a napi felár összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 10. | j | NSS | a napi sztornó összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 11. | k | NSY | a napi engedmény összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 12. | l | NSV | a napi visszáru összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 13. | m | NDB | a napi nyugták és egyszerűsített számlák száma összesen | 20 karakteres numerikus |

| 14. | n | NST | a napi sztornó bizonylatok száma összesen, | 20 karakteres numerikus |

| 15. | o | NSW | a napi visszáru bizonylatok száma összesen | 20 karakteres numerikus |

| 16. | p | NSG | a göngyölített forgalom összesen | 50 karakteres numerikus |

| 17. | q | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 18. | s | HSH | Ellenőrző kód | 64 HEXA karakter |

## 12. Pénztári jelentés

## Bejegyzés azonosító: PJN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: PJN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | JBA | napi bevételek összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 7. | f | JKA | a napi kiadások összesen, bruttó összegben, egész forintban számolva | 20 karakteres numerikus |

| 8. | g | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 9. | h | HSH | Ellenőrző kód | 64 HEXA karakter |

## 13. pénztári befizetés bizonylat

## Bejegyzés azonosító: PBN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: PBN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | PIA | a befizetett összeg, egész forintban számolva | 20 karakteres numerikus |

| 7. | f | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 8. | g | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 9. | h | HSH | Ellenőrző kód | 64 HEXA karakter |

## 14. Pénztári pénz vagy utalvány kifizetési bizonylat

## Bejegyzés azonosító pénzkifizetés esetén: PKN

## Bejegyzés azonosító utalvány kifizetés esetén: UKN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: PKN vagy UKN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | POA | PKN esetén: a kifizetett összeg, egész forintban, UKN esetén a kifizetett utalványok összege egész forintban | 20 karakteres numerikus |

| 7. | f | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 8. | g | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 9. | h | HSH | Ellenőrző kód | 64 HEXA karakter |

## 15. Üzemanyagkártyás értékesítési bizonylat

## Bejegyzés azonosító: KBN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: KBN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | FSN | a bizonylatszám „UK/123456789/000001” alakban | UK/nnnnnnnnn/nnnnnn |

| 7. | f | FAN | a vevő adószáma 12345678-1-12 alakban | nnnnnnnn-n-nn |

| 8. | g | FRN | a rendszám, kizárólag betűket és számokat feltüntetve | 20 karakteres szöveg |

| 9. | h |  | A bizonylaton szereplő összes tételre vonatkozóan, tételenként |  |

| 10. | ha | NA | a tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 11. | hb | UN | a tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, két tizedes pontossággal | 20 karakteres numerikus |

| 12. | hc | QY | a tételnél a bizonylaton szereplő mennyiség | 5 karakteres numerikus |

| 13. | hd | SU | a tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 14. | he | VC | a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 15. | i |  | A bizonylaton szereplő összes törölt tételre vonatkozóan, tételenként |  |

| 16. | ia | NA | a törölt tétel bizonylaton szereplő megnevezése | 200 karakteres szöveg |

| 17. | ib | UN | a törölt tétel bizonylaton szereplő egységára forintban, tizedesvesszővel elválasztva, két tizedes pontossággal | 20 karakteres numerikus |

| 18. | ic | QY | a törölt tételnél a bizonylaton szereplő mennyiség | 5 karakteres numerikus |

| 19. | id | SU | a törölt tételnél a bizonylaton szereplő összérték forintban | 20 karakteres numerikus |

| 20. | ie | VC | a törölt tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren | 3 karakteres szöveg |

| 21. | j | FTL | a bizonylaton szereplő bruttó összeg, egész forintban számolva | 20 karakteres numerikus |

| 22. | k | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 23. | l | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 24. | m | HSH | Ellenőrző kód | 64 HEXA karakter |

## 16. Egészségkártyás értékesítési bizonylat

## Bejegyzés azonosító: EBN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: EBN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | EBS | a bizonylatszám „EK/123456789/000001” alakban | EK/nnnnnnnnn/nnnnnn |

| 7. | f | EPC | az egészségpénztár kódja | 50 karakteres szöveg |

| 8. | g | ERN | a vevő tagszáma | 50 karakteres szöveg |

| 9. | h | ETS | a bizonylaton szereplő bruttó összeg, egész forintban számolva | 20 karakteres numerikus |

| 10. | i | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 11. | j | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 12. | k | HSH | Ellenőrző kód | 64 HEXA karakter |

## 17. Storno bizonylat

## Bejegyzés azonosító: SZN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: SZN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | SBN | a sztornózott nyugta vagy egyszerűsített számla sorszáma 123456789/1234/00001 alakban | 20 karakteres szöveg |

| 7. | f | STO | a vevő részére kifizetett összeg, egész forintban számolva | 20 karakteres numerikus |

| 8. | g | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 9. | h | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 10. | i | HSH | Ellenőrző kód | 64 HEXA karakter |

## 18. Visszáru bizonylat

## Bejegyzés azonosító: VBN

## Bejegyzés mezői

|  | A | B | C | D |

| 1. |  | Mező azonosító | Mező tartalmának leírása | formátum |

| 2. | a | RAZ | Bejegyzés azonosító: VBN | 3 karakteres szöveg |

| 3. | b | BSR | Egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül. | 10 karakteres numerikus |

| 4. | c | DTS | Időbélyeg, a bizonylat kiadásának pontos ideje az AEE órája szerint | szabványos dátum és idő adat másodperc pontossággal |

| 5. | d | TSZ | A bizonylatot kiállító adóalany adó törzsszáma | 8 karakteres szöveg |

| 6. | e | VDB | a visszáru nyugta vagy egyszerűsített számla - a göngyölegjegy kivételével - sorszáma 123456789/1234/00001 alakban | 20 karakteres szöveg |

| 7. | f | VTS | a vevő részére kifizetett összeg, egész forintban számolva | 20 karakteres numerikus |

| 8. | g | ZQQ | Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan ZQQX ahol QQ az egyedi mező sorszáma, X az adott egyedi mezőben szereplő adat. | Z01X~Z02X... |

| 9. | h | CNC | Bizonylat megszakítása esetén a megszakítás tényének jelzése | megszakítás esetén 1 normál rögzítés esetén 0 |

| 10. | i | HSH | Ellenőrző kód | 64 HEXA karakter |

## 19. A 10-18 bejegyzések azonos tartalommal, de a következő bejegyzés azonosítóval ismétlődnek a pénztárgép gyakorló üzemmódjában:

|  | A | B | C | D |

| 1. | pont | megnevezés | normál bizonylat esetén | gyakorló üzemmódú bizonylat esetén |

| 2. | 10 | nyugta | NYN | NYT |

| 3. | 10 | egyszerűsített számla | ESN | EST |

| 4. | 11 | napi forgalmi jelentés | NFN | NFT |

| 5. | 12 | pénztárjelentés | PJN | PJT |

| 6. | 13 | pénztári befizetés bizonylat | PBN | PBT |

| 7. | 14 | pénztári kifizetés bizonylat | PKN | PKT |

| 8. | 14 | utalvány kifizetés bizonylat | UKN | UKT |

| 9. | 15 | üzemanyagkártyás értékesítési bizonylat | KBN | KBT |

| 10. | 16 | egészségkártyás értékesítési bizonylat | EBN | EBT |

| 11. | 17 | sztornó bizonylat | SZN | SZT |

| 12. | 18 | visszáru bizonylat | VBN | VBT |

5. melléklet a 48/2013. (XI. 15.) NGM rendelethez

## Az Adóügyi Ellenőrző Egység (AEE) és a NAV szerverei közötti kommunikáció protokolljára vonatkozó előírások

1. Az AEE és a NAV szerver (ezen mellékletben a továbbiakban: NAV) üzenetei az UTF-8-as kódlap szerint kódolt karaktersorozatok. Jelen melléklet tekintetében XXXXXXXXX az adatszolgáltatással érintett pénztárgép AP számát, HHHHHHHHHH a szerver által előállított, 10 hexadecimális számjegyből álló igazoló kódot jelöli. Amennyiben az AEE válaszüzeneteiben a HHHHHHHHHH igazoló kód szerepel, úgy minden esetben a megelőző NAV üzenetben szereplő kódot kell alkalmazni.

2. Az SMS üzenetek küldésére, vagy a közvetlen IP kommunikáció biztosítására a mobil szolgáltatóknak HTTPS kapcsolaton elérhető API felületet vagy IP interfészt kell biztosítaniuk a NAV számára. A szolgáltató kizárólag a NAV szerverétől fogadhat el üzenetküldési parancsot. Az üzenetek címzése az IMSI vagy MSISDN szám vagy IP cím alapján történik, az interfész jellege szerint.

Az AEE-nek képesnek kell lennie tárolni a NAV SSL tanúsítványának publikus kulcsát, kapcsolatot csak ezzel a tanúsítvánnyal ellenőrzötten építhet ki. A mobilhálózatra az üzenetek HTTPS protokollon POST metódussal kerülnek átadásra.

3. A NAV a „CMSSL~XXXXXXXXX” üzenetet küldi az AEE részére a 2. pont szerinti HTTPS szolgáltatás igénybevételével. A NAV szervere ezen üzenet küldését követően bontja a csomagkapcsolt adatátvitelt. Az üzenet fogadása utasítja az AEE-t titkosított csomagkapcsolt adatátvitel felépítésére.

4. Az AEE-nek a 3. pontban leírt üzenet fogadása után azonnal adatkapcsolatot kell létesítenie a NAV-val, SSL titkosított csatornán keresztül, és az általa felépített SSL csatornán az 5. pont szerinti üzenetet kell elküldenie. A további üzenetek minden esetben az AEE által felépített SSL titkosított csatornán keresztül kerülnek továbbításra, az AEE kizárólag az általa felépített SSL csatornán kezdeményezhet kommunikációt a NAV-val.

5. Az AEE a „TRMRDY~XXXXXXXXX~S~N~T” üzenetet küldi a NAV részére a pénztárgép utolsó bekapcsolásának időpontjához viszonyítottan minden harminc perc elteltével, ahol

a) „XXXXXXXXX” az adatszolgáltatással érintett pénztárgép AP számát jelöli,

b) „S” az AEE éppen nyitott szöveges állomány sorszáma,

c) „N” az AEE éppen nyitott szöveges állományában aktuálisan levő bejegyzések száma,

d) „T” az AEE által utoljára nyitott szöveges fájl megnyitása óta eltelt üzemidő percben.

Erre az üzenetre a NAV a 7., 8., 9., 10., 12., 13. vagy 16. pont szerinti üzenetet adja válaszul.

6. Az AEE a „PRIOR~YY~XXXXXXXXX” üzenet küldi a NAV részére, ha elsőbbségi adatszolgáltatási igényt akar jelezni, ahol YY jelöli az esemény kódját, ami az alábbi eseteket jelöli:

a) YY=01 – az AEE üzemelésének megkezdése esetén,

b) YY=02 – a pénztárgép áramellátásának megszűnése esetén,

c) YY=03 – a pénztárgép blokkolt állapotba kerülése esetén.

Erre az üzenetre a NAV a 7. vagy 8. pont szerinti üzenetet adja válaszul.

7. A NAV a „TRMNOW~F~HHHHHHHHHH” üzenetet küldi az AEE részére amelyben a naplófájl küldésére utasítja, ahol az „F” a NAV által utoljára a címzett AEE-től sikeresen fogadott állomány sorszáma, fogadott állomány hiányában „0” (nulla karakter). Az AEE-nek haladéktalanul végre kell hajtania a következő lépéseket:

a) azonnal, vagy az esetlegesen folyamatban levő bizonylat kiadásának befejezését és a vonatkozó bejegyzés elhelyezését követően azonnal le kell az AEE-n lévő összes adózóra vonatkozón a nyitva levő szöveges állományt, állományokat,

b) Az AEE minden olyan szöveges állományát el kell küldeni a NAV részére, amelynek a sorszáma nagyobb, mint a NAV üzenetében szereplő „F” szám. A küldés egyesével, sorszám szerint növekvő sorrendben történik. A következő fájlt az előző fogadását igazoló ACK nyugta megérkezését követően lehet küldeni.

c) Az elküldött fájl nevének formátuma „fájlnév~HHHHHHHHHH”, ahol fájlnév az éppen küldött naplófájl neve a 4. melléklet 4. pontjában előírt felépítés szerint. A beküldés POST metódussal és multipart/form-data adatkódolással, minden küldött fájl esetében a továbbítás binary kódolással történik. A naplófájlokat elektronikusan aláírva, PKCS#7 formátumban, az elektronikus tanúsítvány csatolása nélkül, bináris adatként kell küldeni a NAV részére.

Erre válaszul a NAV a 8. a), 8. c) vagy 8. d) pont szerinti üzenetet adja, amire az AEE-nek:

8. a) válasz esetén a naplófájl sikertelen küldése miatt a kapcsolatot le kell zárnia és 30 perc elteltével újabb TRMRDY üzenetet kell küldenie.

c) válasz esetén, a NAV sikeresen fogadta a nyugtázott naplóállományt, egyben utasítja az AEE-t a következő sorszámú, NAV számára még el nem juttatott, lezárt naplóállomány NAV szerverének való elküldésére a c) pontban meghatározott módon. Amennyiben nincs lezárt még nem továbbított naplóállomány, a kapcsolat lezárható.

d) válasz esetén a NAV sikeresen fogadta a naplóállományt, így a kapcsolat lezárható.

8. A NAV az „ACK~YY~HHHHHHHHHH” nyugtaüzenetet küldi AEE üzeneteire válaszul, ahol YY a nyugta jellegét jelölő státuszkód, mely a következő értékeket veheti föl:

a) YY=00 – általános hiba az üzenetben, kommunikációban, naplófájl fogadásban az így nyugtázott események nem voltak sikeresek,

b) YY=01 – sikeresen fogadott regisztrációs fájl fogadása esetén az AEE sikeresen regisztrálta a pénztárgépet a NAV regisztrációs szerverén a 15. pontban meghatározott eljárás eredményeképpen,

c) YY=02 – sikeresen fogadott naplófájl nyugta és következő naplófájl küldési utasítás,

d) YY=03 – sikeresen fogadott naplófájl nyugta további adási utasítás nélkül, melynek fogadását követően az AEE-nek azonnal bontania kell az SSL kapcsolatot,

e) YY=04 – sikeresen fogadott üzenet nyugta, melynek fogadását követően az AEE-nek azonnal bontania kell az SSL kapcsolatot.

9. Amennyiben a NAV a „PTGBLCK~HHHHHHHHHH” üzenetet küldi az AEE részére az 5. pontban definiált üzenetre válaszul, az AEE-nek haladéktalanul végre kell hajtania a következő műveleteket:

a) blokkolt állapotba kell hoznia a pénztárgépet,

b) a 11. pontban meghatározott üzenetet kell elküldenie a NAV részére a 01-es okkódot alkalmazva,

c) ezt a NAV egy a 8. e) pontban definiált ACK üzenettel nyugtázza.

10. Amennyiben a NAV a „UNBLCK~HHHHHHHHHH” üzenetet küldi a blokkolt állapotban lévő AEE részére az 5. pontban definiált üzenetre válaszul az AEE-nek haladéktalanul végre kell hajtania a következő műveleteket:

a) a blokkolt állapotban levő pénztárgép blokkolt állapotát meg kell szüntetnie,

b) a 11. pontban meghatározott üzenetet kell elküldenie a NAV részére a 02-es okkódot alkalmazva,

c) ezt a NAV egy a 8. e) pontban definiált ACK üzenettel nyugtázza.

11. az AEE-nek az „ANS~XXXXXXXXX~YY~HHHHHHHHHH” válaszüzenetet kell elküldenie a NAV részére a 9., 10., 12., 13. pontban meghatározott üzenetre válaszul, ahol YY a megelőző üzenetre utaló okkódot jelöli.

a) YY=01 – blokkolás utasítás végrehajtva,

b) YY=02 – blokkolás feloldás utasítás végrehajtva,

c) YY=03 – Áfa gyűjtő átállítás utasítás fogadva,

d) YY=04 – Áfa gyűjtő átállítás utasítás végrehajtva,

e) YY=05 – szoftverfrissítésre kész,

f) YY=06 – szoftverfrissítés letöltve,

g) YY=07 – szoftverfrissítés végrehajtva,

h) YY=08 – adózói törzsadat frissítés végrehajtva,

i) YY=09 – SSL tanúsítvány letöltve.

12. Amennyiben a NAV az 5. pontban definiált üzenetre válaszul a „FRWUPD~ééééhhnn~HHHHHHHHHH” üzenetet küldi az AEE részére, ahol a megadott időpont a szoftver frissítés előírt dátumát jelöli, akkor az AEE-nek azonnal végre kell hajtania a következőket:

a) a felépített SSL csatornán el kell küldenie a 11-es pontban definiált „ANS” válaszüzenetet YY=05 szoftverfrissítésre kész paraméterrel a NAV részére,

b) az a) pont szerinti üzenetre válaszul a NAV elküldi a szoftver műszaki tartalmának részleteit az alábbiak szerint:

ba) az üzenet első eleme az „UPDDTL” karaktersorozat,

bb) ezt követik a firmware-fájl minden szeletére „~NN~CCCC” formátumú üzenetek, ahol „N” az adott szelet sorszáma 1-től sorfolytonosan, legfeljebb két karakterben, vezető nullák nélkül, a „CRC” az adott szelet CRC ellenőrzőösszege 32 bit hosszan,

bc) a következő elemek a „~” karakter és a teljes firmware SHA256 algoritmussal készített ellenőrző kódja 64 karakterben,

bd) az adatsort a „~HHHHHHHHHH” karaktersorozat zárja, ahol a „HHHHHHHHHH” a NAV által előállított, 10 hexadecimális számjegyből álló igazoló kód) Az AEE egység a „UPDREQ~NN~XXXXXXXXX” üzenetekben kéri az adatszeleteket, ahol az „NN” jelöli a kért adatszelet sorszámát, az „XXXXXXXXX” az adatszolgáltatással érintett pénztárgép AP számát jelöli,

c) a d) pont szerinti üzenetre válaszul a NAV elküldi a kért firmware adatszeletet; a szeleteket a sikeres CRC-ellenőrzés után az AEE-nek össze kell raknia, majd ellenőriznie kell az adatállomány SHA256 algoritmussal képzett ellenőrző kódjának egyezését,

d) amennyiben az AEE szoftver letöltése nem kezdődött meg a b) pontban leírt üzenet elküldését követően 60 percen belül, az AEE-nek meg kell ismételnie az a), d) és e) lépéseket a d) pont végrehajtása után 4 órán belül,

e) sikeres letöltést követően a 11. pontban meghatározott „ANS” üzenetet kell elküldenie a NAV részére a 06-os okkódot alkalmazva,

f) a NAV a válaszüzenetre egy a 8. e) pontban definiált ACK üzenet küld; az AEE, ennek az üzenetnek a fogadását követően bontja a kapcsolatot,

g) az „ééééhhnn”’ karaktersorozatban megjelölt napon esedékes napi zárás után az AEE telepíti a leöltött firmware-t, sikeres telepítést követően a 11. pontban meghatározott „ANS” üzenetet kell elküldenie a NAV részére a 07-es okkódot alkalmazva,

h) a NAV a válaszüzenetre egy a 8. e) pontban definiált ACK üzenet küld; az AEE, ennek az üzenetnek a fogadását követően bontja a kapcsolatot.

13. A NAV az 5. pontban definiált üzenetre „VATUPD~XXXXXXXXX~ééééhhnnóóppmm~PPPAAAAA~HHHHHHHHHH” üzenetet küldi az AEE részére, egyes forgalmi gyűjtőkhöz tartozó ÁFA-kulcsok módosításának végrehajtására, amennyiben ez a vonatkozó jogszabályok módosítása miatt szükségessé válik, a változások hatálybalépését legalább 15 nappal megelőzően, ahol:

a) az üzenet első eleme a „VATUPD~” karaktersorozat,

b) második eleme a pénztárgép AP száma,

c) majd az a jövőbeli időpont ééééhhnnóóppmm formátumban, amikortól az üzenetben leírt ÁFA-kulcs módosításokat érvényesíteni kell,

d) az üzenet további elemei az összes olyan forgalmi gyűjtőre vonatkozóan, amelyhez tartozó ÁFA-kulcs módosul:

da) a „-” karakter és a változással érintett forgalmi gyűjtő jele három karakteren (PPP),

db) a da) pontban jelölt forgalmi gyűjtőhöz tartozó, b) pontban jelölt időponttól érvényes ÁFA-kulcs, százalékban kifejezve, százalékjel nélkül, szükség esetén tizedesvesszőt alkalmazva (AAAAA),

dc) több gyűjtő egy ütemben történő módosítása esetén elválasztásra # karaktert kell alkalmazni

e) a „~HHHHHHHHHH” karaktersorozat, ahol HHHHHHHHHH a NAV által előállított, 10 hexadecimális számjegyből álló üzenetazonosító kód.

Erre az üzenetre az AEE a 14. pont szerinti üzenetet adja válaszul.

14. A 13. pontban leírt üzenet fogadását követően az AEE-nek végre kell hajtania a következő műveleteket a felsorolás sorrendjében:

a) a NAV részére el kell küldenie a 11-es pontban definiált „ANS” válaszüzenetet „YY=03 ÁFA gyűjtők átállítási utasítása fogadva” kódot alkalmazva,

b) ezt a NAV egy a 8. e) pontban definiált ACK üzenettel nyugtázza,

c) legkésőbb az üzenetben jelzett időpont előtt 5 nappal a pénztárgép többi egységének át kell adnia az üzenetben szereplő adatokat úgy, hogy a pénztárgép az üzenetben szereplő időponttól kezdve az érintett forgalmi gyűjtőkre vonatkozóan a megadott ÁFA-kulcsokat alkalmazza,

d) a c) pontban jelzett módosítás végrehajtását követően haladéktalanul jelentenie kell a módosítás megtörténtét a NAV részére küldött a 11-es pontban definiált „ANS” válaszüzenettel „YY=04 ÁFA gyűjtők átállítási utasítás végrehajtva” kódot alkalmazva,

e) ezt a NAV a 8. e) pontban definiált ACK üzenettel nyugtázza.

15. A pénztárgép üzembe helyezése (megszemélyesítése) során az alábbi üzenetekkel kommunikál a NAV és az AEE egység:

a) a pénztárgép üzembehelyezésekor, illetve AEE csere esetén, be kell rögzíteni az üzembe helyezési kódot a pénztárgépbe, mely további adatokkal együtt INF típusú bejegyzésként kerül tárolásra a naplófájlba; a fájl nevében, ekkor a törzsszám „00000000” karaktersorozatot tartalmazza, mivel ekkor az még nem áll rendelkezésre; legkésőbb ekkor lehet a pénztárgépbe az AP számot berögzíteni,

b) az AEE elküldi az a) pont szerinti üzembe helyezési kódot tartalmazó elektronikusan aláírt naplófájlt a NAV szerverére, az első küldés alkalmával a tanúsítványt is tartalmazó PKCS#7 formátumban történik,

c) erre az üzenetre a NAV szervere két lehetséges választ küld:

ca) A NAV elküldi a megszemélyesítéshez (tanúsítványok és adózó adatok) szükséges adatokat a pénztárgépnek három, illetve kétvállalkozós pénztárgép esetén négy üzenetben

caa) elsőként a 16. pont szerinti P1=1 üzenetben az adózói törzsadatokat, melyet az AEE egység a 11. pontban leírt YY=08 kóddal nyugtáz,

cab) a másodikként a 16. pont szerinti P1=3 üzenetben az üzemeltetési telephely-adatokat, melyet az AEE egység a 11. pontban leírt YY=08 kóddal nyugtáz,

cac) harmadikként a NAV szerverének SSL-tanúsítványát, melyet az AEE egység a 11. pontban leírt YY=09 kóddal nyugtáz),

cad) negyedikként kétvállalkozós pénztárgép esetén a 16. pont szerinti P1=2 üzenetben az adózói törzsadatokat, melyet az AEE egység a 11. pontban leírt YY=08 kóddal nyugtáz, vagy

cb) elutasítja, ha a beküldött adatokban hiba van (hibás összerendelés, nem nyilvántartott hardverrevízió, már regisztrált AP, felhasznált üzembehelyezési kód stb.),

d) az AEE egység a letöltött tanúsítványokat és adózózói adatokat letárolja,

e) az AEE egység bontja az SSL-kapcsolatot, majd újraépíti azt a letöltött tanúsítvány segítségével végrehajtott eszközazonosítással,

f) az AEE a kulcsokat tartalmazó üzenet sikeres fogadásáról és betöltését követően „TRMRDY~XXXXXXXXX~S~N~T” üzenet küld,

g) ezt a NAV egy a 8. e) pontban definiált ACK üzenettel nyugtázza.

16. A pénztárgépek adózói adatainak frissítése a pénztárgépben

a) amennyiben a NAV az 5. pontban definiált üzenetre válaszul a „DEFUPD~XXXXXXXXX~P1n~P2n~P3n~P4n~P5n~P6n~P7n~P8n~HHHHHHHHHH” üzenetet küldi, úgy a P1-P8 paraméterekben átadott adatokkal frissíteni kell a pénztárgépben tárolt adózói adatokat, ahol az ’n’ a paraméter értéke az alábbi táblázat alapján:

|  | A | B | C | D | E | F | G | H |

| 1. | P1 változás típuskód | P2 | P3 | P4 | P5 | P6 | P7 | P8 |

| 2. | Értéke: 1 Értelmezése: adózói törzsadat (kétvállalkozós pénztárgép esetén az üzemanyag tulajdonosa) | frissítendő felhasználó adószáma | név | irányító- szám | település | közterület- neve | közterület jellege | házszám |

| 3. | Értéke: 2 Értelmezése: kétvállalkozós pénztárgép esetén az üzlet üzemeltetőjének adózói törzsadatai | frissítendő felhasználó adószáma | név | irányító- szám | település | közterület neve | közterület jellege | házszám |

| 4. | Értéke: 3 Értelmezése: üzemeltetési telephely | Üzemeltető adószáma | üzlet neve | irányító- szám | település | közterület neve | közterület jellege | házszám |

b) P1=1 vagy P=2 paraméter esetén az adóalany adatait frissíteni kell a küldött adatokkal,

P1=3 paraméter esetén a pénztárgép telephelyét kell frissíteni a kapott adatokkal,

c) a NAV részére el kell küldenie a 11-es pontban definiált „ANS” válaszüzenetet „YY-08 adózói törzsadat update” kódot alkalmazva,

d) ezt a NAV a 8. e) pontban definiált ACK üzenettel nyugtázza.

17. Az AEE-nek be kell jegyeznie a legutóbb megnyitott szöveges állományba a fogadott és a küldött üzeneteit is 4. melléklet előírásai szerint.

18. Az AEE-nek bontania kell az SSL kapcsolatot, amennyiben legalább 1 percig semmiféle kommunikáció sem történik a NAV-val.
