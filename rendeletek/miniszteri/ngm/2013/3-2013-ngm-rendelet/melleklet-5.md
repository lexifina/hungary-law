## Az Adóügyi Ellenőrző Egységben (AEE) tárolt bizonylati adatok tartalmára

## és szerkezetére vonatkozó előírások

## 1. Az AEE-nek a pénztárgépben keletkezett adatokat az eszköz üzembe helyezésétől, illetve a legutóbbi adatszolgáltatástól az aktuális pillanatig terjedő időszakra vonatkozóan ANSI 1250-es kódlap szerinti karakterkódolású szöveges állományokban kell tárolnia.

## 2. Az AEE-nek a NAV szerverétől kapott, 5. melléklet szerinti utasítás alapján történő adattovábbításkor a legutóbbi bejegyzéssel érintett szöveges állományt le kell zárnia, és azt a NAV szerverei felé el kell küldenie. Az AEE-nek minden adattovábbítás megkezdését követően új szöveges állományt kell nyitnia, és abban kell folytatnia a bejegyzések rögzítését. Az AEE-nek a szöveges állományt annak megnyitását követő 24 óra elteltével akkor is le kell zárnia és újat kell nyitnia, ha ezen idő alatt nem történt adattovábbítás a NAV szervere felé.

## 3. Az AEE-nek az elküldött állományt az elküldés megkezdésének időpontja szerinti AAAAAAAAA_ééééhhnnóóppmm_s.txt néven kell eltárolnia, ahol

## a) AAAAAAAAA: A pénztárgép AP száma 9 karakteren,

## b) éééé: az év száma négy számjegyen,

## c) hh: a hónap sorszámát két számjegyen,

## d) nn: a nap sorszáma két számjegyen,

## e) óó: az óra száma két számjegyen,

## f) pp: a perc száma két számjegyen,

## g) mm: a másodperc száma két számjegyen,

## h) s: a fájl 1-től kezdődően, kihagyás és ismétlés nélkül képzett sorszáma az AEE élettartama során.

## 4. Az AEE első üzembehelyezésekor, az elsőként nyitott állományban szereplő, 5. pontban megadott bejegyzést követően

## a) az„ONA” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az adatszolgáltatással érintett pénztárgép AP számát kilenc karakteren,

## d) a „~” karaktert, majd az AEE szoftverének azonosítóját

## e) a „~” karaktert, majd az AEE szoftverének verziószámát,

## f) a „~” karaktert, majd az a)-e) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## g) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 5. Az AEE-nek szöveges állomány nyitásakor, minden esetben a szöveges állomány első bejegyzéseként

## a) az „LON” karaktersorozatot,

## b) a „~” karaktert, majd a pénztárgép AP számát 9 karakteren,

## c) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## d) a „~” karaktert, majd az a)-c) pontok adataiból és – ha ilyen létezik – az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## e) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 6. Az AEE-nek szöveges állomány zárásakor, minden esetben a szöveges állomány utolsó bejegyzéseként

## a) az „LCL” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az a)-b) pontok adataiból és az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 7. Az AEE-nek a pénztárgép áramellátásának megindulása és az AEE saját áramforrásról történő működésének vége esetén

## a) a „PIN” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)-b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 8. Az AEE-nek a pénztárgép áramellátásának megszűnése és az AEE saját áramforrásról történő működésének kezdete esetén

## a) a „POF” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)-b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 9. Az AEE-nek a saját áramforrása lemerülése és a pénztárgépről érkező áramellátás megszűnése esetén

## a) a „BDN” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)-b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 10. Az AEE-nek a saját áramforrásának lemerülése utáni első üzemelés elindulásakor

## a) az „RST” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)-b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 11. A pénztárgép blokkolt állapotba kerülése esetén

## a) a „BLS” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 12. A pénztárgép blokkolt állapotának megszűnése esetén

## a) a „BLF” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)-b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 13. A pénztárgép gyakorló üzemmódba kerülése esetén

## a) a „TRI” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében

## 14. A pénztárgép gyakorló üzemmódból való visszakapcsolása esetén

## a) a „TRF” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–b) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## d) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében

## 15. Pénztárnyitás esetén

## a) a „CHO” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd a pénztár nyitó pénzkészletét forintban,

## d) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–c) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## e) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 16. A NAV szerverétől érkező üzenet fogadása esetén

## a) az „MGI” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd a szerver által küldött teljes üzenetet

## d) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–c) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## e) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 17. Üzenet küldése esetén a NAV szerver részére

## a) az „MGO” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd a szervernek küldött teljes üzenetet

## d) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–c) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## e) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 18. A pénztárgép első üzembe helyezése, illetve áthelyezése esetén

## a) a „PLC” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## c) a „~” karaktert, majd a pénztárgép szervizes által megadott aktuális címét,

## d) a „~” karaktert, majd a bejegyzést végző műszerész műszerészi igazolványának számát,

## e) a „~” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–d) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## f) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 19. A kiadott bizonylatok adatait az AEE az alábbi bejegyzés-szerkezettel tárolja el.

## a) A bejegyzés első eleme a bejegyzés típusát jelzőhárom karakter, ami:

## 1. nyugta esetén: „NYN”,

## 2. egyszerűsített számla esetén: „ESN”,

## 3. napi forgalmi jelentés esetén „NFN”,

## 4. pénztárjelentés esetén: „PJN”,

## 5. pénztári befizetés bizonylat esetén: „PBN”,

## 6. pénztári kifizetés bizonylat esetén: „PKN”,

## 7. üzemanyagkártyás értékesítési bizonylat esetén: „KBN”,

## 8. egészségkártyás értékesítési bizonylat esetén: „EBN”,

## 9. sztornó bizonylat esetén: „SZN”,

## 10. visszáru bizonylat esetén: „VBN”,

## 11. gyakorló üzemmódban kiadott nyugta esetén: „NYT”,

## 12. gyakorló üzemmódban kiadott egyszerűsített számla esetén: „EST”,

## 13. gyakorló üzemmódban kiadott napi forgalmi jelentés esetén „NFT”,

## 14. gyakorló üzemmódban kiadott pénztárjelentés esetén: „PJT”,

## 15. gyakorló üzemmódban kiadott pénztári befizetés bizonylat esetén: „PBT”,

## 16. gyakorló üzemmódban kiadott pénztári kifizetés bizonylat esetén: „PKT”,

## 17. gyakorló üzemmódban kiadott üzemanyagkártyás értékesítési bizonylat esetén: „KBT”,

## 18. gyakorló üzemmódban kiadott egészségkártyás értékesítési bizonylat esetén: „EBT”,

## 19. gyakorló üzemmódban kiadott sztornó bizonylat esetén: „SZT”,

## 20. gyakorló üzemmódban kiadott visszáru bizonylat esetén: „VBT”

## 21. visszavont nyugta esetén: „NYC”,

## 22. visszavont egyszerűsített számla esetén: „ESC”,

## 23. visszavont napi forgalmi jelentés esetén „NFC”,

## 24. visszavont pénztárjelentés esetén: „PJC”,

## 25. visszavont pénztári befizetés bizonylat esetén: „PBC”,

## 26. visszavont pénztári kifizetés bizonylat esetén: „PKC”,

## 27. visszavont üzemanyagkártyás értékesítési bizonylat esetén: „KBC”,

## 28. visszavont egészségkártyás értékesítési bizonylat esetén: „EBC”,

## 29. visszavont sztornó bizonylat esetén: „SZC”,

## 30. visszavont visszáru bizonylat esetén: „VBC”,

## b) A bejegyzés második eleme a „~” karakter, majd egy számláló értéke, amelynek kezdeti értéke „1” és minden bizonylat AEE-ben való eltárolását követően 1-gyel nő, a kiadott bizonylat típusától függetlenül.

## c) A bejegyzés harmadik eleme a „~” karakter, majd a bizonylat kiadásának pontos ideje az AEE órája szerint, ééééhhnnóóppmm formátumban, 14 számjegyen ábrázolva.

## d) A bejegyzés negyedik eleme a „~” karakter, majd a pénztárgépet működtető adóalany adó törzsszáma, 8 számjegyen.

## e) A bejegyzésben szereplő bizonylat típusa szerint az ea)–ei) pontokban részletezett adattartalmat az adott felsorolás sorrendjében kell elhelyezni a szöveges állományban.

## ea) Nyugta vagy egyszerűsített számla esetén:

## 1) a „~” karakter, majd a bizonylat száma 1234/00001 formátumban,

## 2) az adott bizonylat tartalma gyűjtőnként megjelenítve, kizárólag az adott bizonylaton ténylegesen használt gyűjtőkre vonatkozóan, „~XXXn” alakban, ahol:

## ~: a 126-os kódú karakter,

## XXX: a gyűjtő jele három karakteren,

## n: a bizonylaton szereplő tételek bruttó összege az adott gyűjtőben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül

## 3) a „~SUM” karaktersorozat és a bizonylaton szereplő bruttó összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül

## 4) a „~TAX” karaktersorozat és a bizonylaton szereplő összes ÁFA összege, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül

## 5) amennyiben a bizonylat tartalmaz engedményt, akkor a „~DCN” karaktersorozat és a bizonylaton szereplő összes engedmény összege, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül

## 6) amennyiben a bizonylat tartalmaz kerekítést, akkor a „~RND” karaktersorozat és a bizonylaton szereplő kerekítés összege, egész forintban számolva, szükség esetén negatív előjellel.

## 7) Amennyiben ez az adat a kinyomtatott bizonylaton szerepel, akkor a „~PMD” karaktersorozat és a fizetési mód jele, ami készpénz esetén „0”, bankkártya esetén „1”, egyéb fizetési mód esetén „2”.

## 8) Amennyiben ilyen adat a kinyomtatott bizonylaton szerepel, akkor a „~HCN” karaktersorozat és a vásárlói kártya, hűségkártya azonosítója.

## 9) Egyszerűsített számla esetén a „~VDA” karaktersorozat és a termék beszerzőjének, szolgáltatás igénybevevőjének adatai az ÁFA tv. rendelkezései szerint.

## 10) A bizonylaton szereplő összes tételre vonatkozóan, tételenként:

## i) az „~INA” karaktersorozat és a tétel bizonylaton szereplő megnevezése

## ii) az „~IUN” karaktersorozat és a tétel bizonylaton szereplő egységára forintban

## iii) az „~IQY” karaktersorozat és a tételnél a bizonylaton szereplő mennyiség

## iv) az „~ISU” karaktersorozat és a tételnél a bizonylaton szereplő összérték forintban

## v) az „~IVC” karaktersorozat és a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren.

## eb) Napi forgalmi jelentés esetén

## 1) a zárás sorszáma négy karakteren, szükség esetén vezető nullákkal feltöltve,

## 2) az adott nap bruttó bevétele gyűjtőnként megjelenítve, kizárólag az adott bizonylatot érintő gyűjtőkre vonatkozóan, „~XXXn” alakban, ahol:

## ~: a 126-os kódú karakter,

## XXX: a gyűjtő jele három karakteren

## n: a bizonylaton szereplő tételek bruttó összege az adott gyűjtőben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 3) a „~NSF” karaktersorozat és a napi forgalom összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 4) a „~NSH” karaktersorozat és a napi felár összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 5) a „~NSS” karaktersorozat és a napi sztornó összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 6) a „~NSY” karaktersorozat és a napi engedmény összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 7) a „~NSV” karaktersorozat és a napi visszáru összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 8) a „~NSZ” karaktersorozat és a napi nyugták és egyszerűsített számlák száma összesen, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 9) a „~NST” karaktersorozat és a napi sztornó bizonylatok száma összesen, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 10) a „~NSW” karaktersorozat és a napi visszáru bizonylatok száma összesen, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 11) a „~NSG” karaktersorozat és a göngyölített forgalom összesen, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## ec) Pénztárjelentés esetén

## 1) a „~JBA” karaktersorozat és a napi bevételek összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül,

## 2) a „~JKA” karaktersorozat és a napi kiadások összesen, bruttó összegben, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## ed) Pénztári befizetés bizonylat esetén a befizetett összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## ee) Pénztári kifizetés bizonylat esetén a kifizetett összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## ef) Üzemanyagkártyás értékesítési bizonylat esetén

## 1) a „~FSN” karaktersorozat és a bizonylatszám „UK/123456789/000001”alakban,

## 2) a „~FAN” karaktersorozat és a vevő adószáma 12345678-1-12 alakban,

## 3) a „~FRN” karaktersorozat és a rendszám, kizárólag betűket és számokat feltüntetve,

## 4) a „~FTL” karaktersorozat és a bizonylaton szereplő bruttó összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## eg) Egészségkártyás értékesítési bizonylat esetén

## 1) a „~ESN” karaktersorozat és a bizonylatszám „EK/123456789/000001”alakban,

## 2) a „~EPC” karaktersorozat és az egészségpénztár kódja,

## 3) a „~ERN” karaktersorozat és a vevő tagszáma,

## 4) a „~ETS” karaktersorozat és a bizonylaton szereplő bruttó összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## eh) Sztornó bizonylat esetén

## 1) a „~SBN” karaktersorozat és a sztornózott nyugta vagy egyszerűsített számla sorszáma 123456789/1234/00001 alakban,

## 2) a „~STO” karaktersorozat és a vevő részére kifizetett összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## ei) Visszáru bizonylat esetén

## 1) a „~VBN” karaktersorozat és a visszáru nyugta vagy egyszerűsített számla – a göngyölegjegy kivételével –sorszáma 123456789/1234/00001 alakban,

## 2) a „~VTS” karaktersorozat, majd a vevő részére kifizetett összeg, egész forintban számolva, a szükséges számú számjegyen ábrázolva, vezető nullák nélkül.

## f) Amennyiben a nyomtatott bizonylaton szereplő adatok eltárolásához szükséges egyedi mező, akkor a használt egyedi mezők mindegyikére vonatkozóan a „~ZQQ” karaktersorozat, majd az adott egyedi mezőben szereplő adat. A „QQ” az egyedi mező sorszámát jelöli. Az egyedi mezőket 01-től kell egyesével számozni.

## g) Az a)–f) pontban felsorolt adatokat követően a bejegyzés további karakterei a „~HSH” karaktersorozat és az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–f) pontok tartalmából az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karaktere, figyelembe nem véve az ea) 9. pontjában szereplő adatot.

## h) A bejegyzést minden esetben az „Új sor” karakter zárja.

## 20. Tétel törlése esetén – ha a bizonylat készítése folytatódik és az kiadásra kerül – az adott bizonylatra vonatkozó bejegyzést követően

## a) a „DIT” karaktersorozatot,

## b) a „~” karaktert, majd az aktuális időpontot ééééhhnnóóppmm formátumban,

## a bizonylaton szereplő összes tételre vonatkozóan, tételenként:

## i) az „~INA” karaktersorozat és a tétel bizonylaton szereplő megnevezése

## ii) az „~IUN” karaktersorozat és a tétel bizonylaton szereplő egységára forintban

## iii) az „~IQY” karaktersorozat és a tételnél a bizonylaton szereplő mennyiség

## iv) az „~ISU” karaktersorozat és a tételnél a bizonylaton szereplő összérték forintban

## v) az „~IVC” karaktersorozat és a tételnél a bizonylaton feltüntetett forgalmi gyűjtő jele három karakteren,

## c) a bizonylat készítése során törölt összes tételre vonatkozóan, tételenként:

## ca) a „~DNA” karaktersorozatot és a törölt tétel megnevezését,

## cb) a „~DUN” karaktersorozatot és a törölt tétel egységárát forintban,

## cc) a „~DQY” karaktersorozatot és a törölt tételnél megadott mennyiséget,

## cd) a „~DSU” karaktersorozatot és a törölt tételre vonatkozó összértéket forintban,

## ce) a „~DVC” karaktersorozatot és a tételre vonatkozó forgalmi gyűjtő jelét három karakteren,

## d) a „~HSH” karaktert, majd az előző bejegyzésre képzett ellenőrző kódból, az előzőleg lezárt szöveges állomány utolsó ellenőrző kódjából, valamint az a)–c) pontok adataiból az SHA256 algoritmussal a 21. pont szerint képzett ellenőrző kód 64 karakterét,

## e) az „új sor” karaktert

## kell elhelyezni a szöveges állományban, a felsorolás sorrendjében.

## 21. A jelen melléklet 4–20. pontjában szereplő ellenőrző kód képzésekor az SHA256 algoritmus bemenő adata az a karaktersorozat, amely az alábbi részekből tevődik össze az alábbi felsorolás sorrendjében:

## a) A bemenő karaktersorozat első hatvannégy karaktere az AEE által legutóbb lezárt szöveges állomány utolsó bejegyzését lezáró „Új sor” karakter előtti 64 karakteres ellenőrző kód, amelyben az A–F hexadecimális számjegyeket nagybetűkként kell értelmezni. Amennyiben még nem létezik legutóbb lezárt szöveges állomány, akkor a bemenő karaktersorozat első 64 karaktere 64 db „F”.

## b) A bemenő karaktersorozat 65–128. karaktere az adott bejegyzést megelőző bejegyzést lezáró „Új sor” karakter előtti 64 karakteres ellenőrző kód, amelyben az A–F hexadecimális számjegyeket nagybetűkként kell értelmezni. Ha nem létezik az adott szöveges állományban előző bejegyzés, akkor a bemenő karaktersorozat 65–128. karaktere 64 db „F”.

## c) A bemenő karaktersorozat további karakterei az adott bejegyzésben szereplő, 4–20. pontokban meghatározott adattartalom az ott meghatározott sorrendben, a bejegyzés végén elhelyezendő 64 karakteres ellenőrző kódot megelőző karakterrel bezárólag.

## 22. A jelen melléklet 4–20. pontjában szereplő ellenőrző kódot karaktersorozatként kell feltüntetni úgy, hogy az A–F számjegyek nagybetűkként szerepeljenek.

## 23. Az AEE által létrehozott szöveges állományokban 32-nél kisebb kódú karakterek és a 126-os kódú karakter („~”) kizárólag a rendeletben megkövetelt esetekben és módon szerepelhet. Amennyiben valamilyen feltüntetendő adatban eredetileg szerepel 32-nél kisebb kódú vagy 126-os kódú karakter, azt az AEE-ben létrehozott szöveges állományokban szóközzel, illetve kötőjellel kell helyettesíteni.

## 24. Az AEE a napi zárásokról külön naplóállományt is vezet, a 3. melléklet I. rész A) pont 9. alpontja szerinti tájékoztatás céljára.

5. melléklet a 3/2003 . (II. 15.) NGM rendelethez[^4]

[^4]: Az 5. melléklet a 70. § (3) bekezdése alapján 2013. május 1-jén lép hatályba.
