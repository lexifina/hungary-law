## „3. melléklet a 67/2016. (XII. 29.) NFM rendelethez

## A felajánlási ár tekintetében a földgáz beszerzési költség indokolt mértékének meghatározásakor figyelembe vett elismert fajlagos földgázár

## 1. Elismert ár meghatározása betárolási hónapban (kivéve szeptember hónapot):

## 1.1. Ha QTény >= (QFedezett + QHazaitermelés_tervezett), akkor

## Elismert ár = (QFedezett * PFedezettimport ár+ QHazaitermelés_tervezett* PHazaitermelés+ (QTény - QFedezett - QHazaitermelés_tervezett) * PAktuálisimport ár+QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 1.2. Ha QTény < (QFedezett + QHazaitermelés_tervezett), akkor

## 1.2.1. Elismert ár = (QHazaitermelés_tervezett* PHazaitermelés+ (QTény - QHazaitermelés_tervezett) * PFedezettimport ár+ QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) + CEGY) / QTény,

## QTöbblet =0

## PTöbblet =0

## 1.2.2. QTárolóifedezés= (QFedezett + QHazaitermelés_tervezett- QTény).

## 2. Elismert ár meghatározása szeptember hónapban:

## 2.1. Ha QTény >= (QFedezett + QHazaitermelés_tervezett), akkor

## Elismert ár = (QFedezett * PFedezettimport ár+ QHazaitermelés_tervezett* PHazaitermelés+ (QTény - QFedezett - QHazaitermelés_tervezett) * PAktuálisimport ár+ QBiztonságizárókészlet* (PAktuális_import_ár_téli_súlyozott_átlag- PFedezetttárolói ár) + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 2.2. Ha QTény < (QFedezett + QHazaitermelés_tervezett), akkor

## 2.2.1. Elismert ár = (QHazaitermelés_tervezett* PHazaitermelés+ (QTény - QHazaitermelés_tervezett) * PFedezettimport ár+ QBiztonságizárókészlet* (PAktuális_import_ár_téli_súlyozott_átlag- PFedezetttárolói ár) + CEGY) / QTény,

## QTöbblet =0

## PTöbblet =0

## 2.2.2. QTárolóifedezés= (QFedezett + QHazaitermelés_tervezett- QTény).

## 3. Elismert ár meghatározása kitárolási hónapban (kivéve december hónapot):

## 3.1. Ha QTény >= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés – QFedezett – QKedvezményesforrás– QTervezettimport) <= QHidegreelkülönített tárolói készlet, akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + QTervezettimport * PAktuálisimport ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés - QFedezett - QKedvezményesforrás - QTervezettimport) * PFedezetttárolói ár+ QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 3.2. Ha QTény >= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és QHidegreelkülönített tárolói készlet = 0, akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés - QFedezett - QKedvezményesforrás)* PAktuálisimport ár + QTöbblet-1*(PTöbblet-1 - PLikvidimport ár)- ELakosságicélú + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 3.3. Ha QTény >= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés – QFedezett – QKedvezményesforrás – QTervezettimport) > QHidegre_elkülönített tárolói készlet, de QHidegre_elkülönített tárolói készlet > 0, akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + QHidegre_elkülönített tárolói készlet * PFedezetttárolói ár + (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés – QFedezett – QKedvezményesforrás – QHidegre_elkülönített tárolói készlet) * PAktuálisimport ár + QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + CEGY) / QTény,

## QTöbblet =0

## PTöbblet =0

## 3.4. Ha QTény < (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és QTény > (QHazaitermelés_tervezett + QAllokálttárolói fedezés+ QFedezett + QKedvezményesforrás), akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés - QFedezett - QKedvezményesforrás) * Paktuálisimport ár + QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 3.5. Ha QTény <= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás) és QTény > (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett), akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés - QFedezett) * PKedvezményesforrás ár + QTöbblet-1* (PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + CEGY) / QTény

## QTöbblet = (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás - QTény)

## PTöbblet = PKedvezményesforrás ár

## 3.6. Ha QTény <= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett) és QTény > (QHazaitermelés_tervezett + QAllokálttárolói fedezés), akkor Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés) * PFedezettimport ár + QTöbblet-1* (PTöbblet-1 -PLikvidimport ár) - ELakosságicélú + CEGY) / QTény

## QTöbblet =(QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett - QTény) + QKedvezményesforrás

## PTöbblet =( (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett - QTény) * PFedezettimport ár+ QKedvezményesforrás* PKedvezményesforrás ár )/ QTöbblet

## 3.7. Ha QTény <= (QHazaitermelés_tervezett + QAllokálttárolói fedezés), akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + (QTény - QHazaitermelés_tervezett) * PFedezetttárolói ár + (QHazaitermelés_tervezett + QAllokálttárolói fedezés - QTény) * (PFedezetttárolói ár - PAktuálisimport ár) + QFedezett * (PFedezettimport ár - PAktuálisimport ár) + QTöbblet-1* (PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + CEGY) / QTény

## QTöbblet = (QHazaitermelés_tervezett + QAllokálttárolói fedezés - QTény) + QFedezett + QKedvezményesforrás

## PTöbblet =( (QHazaitermelés_tervezett + QAllokálttárolói fedezés - QTény) * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár) / QTöbblet

## 4. Elismert ár meghatározása december hónapban:p

## 4.1. Ha QTény >= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés - QFedezett - QKedvezményesforrás - QTervezettimport) <= QHidegreelkülönített tárolói készlet,akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + QTervezettimport* PAktuálisimport ár + (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés – QFedezett – QKedvezményesforrás – QTervezettimport) * PFedezett tárolói ár – (MtMt – MtMt–1) +QTöbblet-1* (PTöbblet-1 -PLikvidimport ár) - ELakosságicélú + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazaitermelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 4.2. Ha QTény >= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és QHidegreelkülönített tárolói készlet = 0, akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés* PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés - QFedezett - QKedvezményesforrás) * PAktuálisimport ár - (MtMt - MtMt-1) +QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazaitermelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 4.3. Ha QTény >= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés – QFedezett – QKedvezményesforrás – QTervezettimport) > QHidegreelkülönített tárolói készlet, de QHidegreelkülönített tárolói készlet > 0, akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + QHidegreelkülönített tárolói készlet * PFedezetttárolói ár + (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés – QFedezett – QKedvezményesforrás – QHidegreelkülönített tárolói készlet) * PAktuálisimport ár – (MtMt – MtMt–1) +QTöbblet-1*(PTöbblet-1 -PLikvidimport ár)- ELakosságicélú + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazaitermelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 4.4. Ha QTény < (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás + QTervezettimport) és QTény > (QHazaitermelés_tervezett + QAllokálttárolói fedezés+ QFedezett + QKedvezményesforrás) akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár + (QTény - QHazaitermelés_tervezett - QAllokálttárolói fedezés – Qfedezett- QKedvezményesforrás) * PAktuálisimport ár - (MtMt - MtMt-1) +QTöbblet-1*(PTöbblet-1 - PLikvidimport ár) + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazaitermelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet =0

## PTöbblet =0

## 4.5. Ha QTény <= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás) és QTény > (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett), akkor Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + QFedezett * PFedezettimport ár + (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés - QFedezett) * PKedvezményesforrásár– (MtMt – MtMt–1) +QTöbblet-1*(PTöbblet-1 -PLikvidimport ár)- ELakosságicélú + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazai termelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet = (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett + QKedvezményesforrás - QTény)

## PTöbblet = PKedvezményesforrás ár

## 4.6. Ha QTény <= (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett) és QTény > (QHazaitermelés_tervezett + QAllokálttárolói fedezés), akkor Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + QAllokálttárolói fedezés * PFedezetttárolói ár + (QTény – QHazaitermelés_tervezett – QAllokálttárolói fedezés) * PFedezettimport ár – (MtMt – MtMt–1) +QTöbblet-1*(PTöbblet-1 -PLikvidimport ár) - ELakosságicélú + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazaitermelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet =(QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett - QTény) + QKedvezményesforrás

## PTöbblet =( (QHazaitermelés_tervezett + QAllokálttárolói fedezés + QFedezett - QTény) * PFedezettimport ár+ QKedvezményesforrás* PKedvezményesforrás ár )/ QTöbblet

## 4.7. Ha QTény <= (QHazaitermelés_tervezett + QAllokálttárolói fedezés), akkor

## Elismert ár = (QHazaitermelés_tervezett * PHazaitermelés + (QTény - QHazaitermelés_tervezett) * PFedezetttárolói ár - (MtMt - MtMt-1) +QTöbblet-1* (PTöbblet-1 - PLikvidimport ár) - ELakosságicélú + Σ((QHazaitermelés_negyedéves tény – QHazaitermelés_negyedéves tervezett) * (PHazaitermelés_negyedéves átlag – PAktuálisimport ár_negyedéves átlag)) + CEGY) / QTény

## QTöbblet = (QHazaitermelés_tervezett + QAllokálttárolói fedezés - QTény) + QFedezett + QKedvezményesforrás

## PTöbblet =( (QHazaitermelés_tervezett + QAllokálttárolói fedezés - QTény) * PFedezetttárolói ár + QFedezett * PFedezettimport ár + QKedvezményesforrás * PKedvezményesforrás ár) / QTöbblet

## 5. Kiegyensúlyozási költség számításának módszertana:

## 5.1. Napi kiegyensúlyozási költség számítása

## 5.1.1. Ha QALL - QNOM >= 0, akkor

## CEGY_ESZ = min (QALL - QNOM, QALL * 0,05) * (Pmv - PAktuálisimport ár + Pelszámolóforgalmi díja)

## 5.1.2. Ha QALL - QNOM < 0, akkor

## CEGY_ESZ = min (QNOM - QALL, QALL * 0,05) * (PAktuálisimport ár - Pme + Pelszámolóforgalmi díja)

## 5.2. Havi kiegyensúlyozási költség számítása

## 6. E mellékletben alkalmazott rövidítések:

## 6.1. Betárolási hónap: minden olyan naptári hónap, amikor az egyetemes szolgáltatót ellátó földgázkereskedő egyetemes szolgáltató ellátása céljából nettó betárolást végez;

## 6.2. Kitárolási hónap: minden olyan naptári hónap, amikor az egyetemes szolgáltatót ellátó földgázkereskedő egyetemes szolgáltató ellátása céljából nettó kitárolást végez;

## 6.3. QTerv (tervezett értékesített mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által egyetemes szolgáltatónak a tárgyhónapban értékesített földgáz tervezett mennyisége kWh-ban, mely az egyetemes szolgáltatónak az adott tárgyhónapra vonatkozó 1. § (5) bekezdése, illetve 2. § (5) bekezdése szerinti éves igénybejelentéseinek összegével egyezik meg;

## 6.4. QTerv_éves (tervezett éves értékesített mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által egyetemes szolgáltatónak a tárgyévben értékesített földgáz tervezett mennyisége kWh-ban, mely az egyetemes szolgáltatónak az adott évre vonatkozó 1. § (5) bekezdése, illetve 2. § (5) bekezdése szerinti éves igénybejelentéseinek összegével egyezik meg, ahol QTerv_éves = ΣQTerv;

## 6.5. QTény (tény értékesített mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által egyetemes szolgáltatónak a tárgyhónapban értékesített földgáz tény mennyisége kWh-ban;

## 6.6. QFedezett (fedezett mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által a tárgyhónapra lefedezett mennyiség kWh-ban;

## 6.7. QTárolóifedezés(tárolói fedezett mennyiség): a betárolási időszak egyes hónapjaiban az egyetemes szolgáltatót ellátó földgázkereskedő által fedezett mennyiség (QFedezett), valamint a hazai termelésből beszerzett tervezett havi mennyiség (QHazaitermelés_tervezett) összegének és a tény értékesített mennyiségnek (QTény) a különbsége, amennyiben ez pozitív;

## 6.7.1. QRendelkezésreálló tárolói fedezés(tárolói fedezett mennyiség): a tárolói fedezett mennyiség (ΣQTárolóifedezés) csökkentve az allokált tárolói fedezett mennyiség ( Σ1M-1 (QAllokálttárolói fedezés) és a hidegre elkülönített tárolói készlet (Σ1M-1 (QHidegre_elkülönített tároló_havi)) adott hónapban felhasznált részének összegével.

## 6.8. QNyitókészlet: 2018. április 1-jén az egyetemes szolgáltatót ellátó földgázkereskedő által megadott, a tárolóban fizikailag bennlevő földgázkészlet kWh-ban. A 2018-as naptári évet követő betárolási időszakok kezdetén értéke megegyezik a hidegre elkülönített tárolói készlet mennyiségből a március 31-ére megmaradt maradványkészlettel;

## 6.9. PNyitókészlet: 2018. április 1-jén értéke a betárolási időszakot megelőző kitárolási időszak hónapjaiban érvényes import földgáz árak (PAktuálisimport ár) számtani átlaga, HUF/kWh-ban kifejezve; a 2018-as naptári évet követő betárolási időszakok kezdetén értéke a betárolási időszakot közvetlen megelőző kitárolási időszakban érvényes tárolói földgáz fedezett ára HUF/kWh-ban kifejezve (PFedezetttárolói ár);

## 6.10. QBiztonságizárókészlet: a Hivatal által elismert, ellátásbiztonsági okokból egyetemes szolgáltatási célú ellátásra betárolt QProfilozotttárolói összmennyiség készletből fel nem használt földgázkészlet kWh-ban megadott értéke az adott év március 31-én;

## 6.11. QAllokálttárolói fedezés (allokált tárolói fedezett mennyiség): QProfilozotttárolóiösszmennyiség-nek a kitárolási időszak adott hónapjára vonatkozó része, ahol az egyes hónapokra történő szétosztás a felhasználás tervezett havi mennyisége és a kitárolási időszakra vonatkozó felhasználás tervezett mennyisége arányában történik [QAllokálttárolói fedezés = QProfilozotttárolói összmennyiség * QTerv / ΣQTerv_tél, ahol ΣQTerv_tél a kitárolási időszak hónapjaira (október–március) eső QTerv értékek összege];

## 6.12. QHazaitermelés_tervezett(hazai termelésből beszerzett tervezett havi mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által hazai termelésből beszerezni kívánt, tervezett földgáz mennyisége tárgyhónapban, kWh-ban, melyet a Hivatal határoz meg előre olyan módon, hogy a tervezett hazai termelés profilja meg kell, hogy egyezzen az egyetemes szolgáltatók számára tervezett értékesítési profillal);

## 6.13. QHazaitermelés_negyedéves tervezett(hazai termelésből beszerzett egyenletes ütemezésű tervezett negyedéves mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által hazai termelésből beszerezni kívánt, tervezett földgáz mennyisége az adott naptári év negyedévében, kWh-ban, melyet a Hivatal a termelő adatszolgáltatása alapján határoz meg az egyetemes szolgáltatót ellátó földgázkereskedő számára;

## 6.14. QHazaitermelés_negyedéves tény(hazai termelésből beszerzett negyedéves tény mennyiség): az egyetemes szolgáltatót ellátó földgázkereskedő által hazai termelésből beszerzett földgáz tény mennyisége az adott naptári év negyedévében, kWh-ban;

## 6.15. PAktuálisimport ár(import földgáz ára az adott hónapban, HUF/kWh-ban kifejezve): PAktuálisimport ár= (fgS + sp) * EURHUF / 1000, ahol:

## 6.15.1. fgS: A szállítási hónapra vonatkozó ICE TTFI EUR/MWh ár az Intercontinental Exchange Inc. honlapján a Report Center „Indices - UK and European NaturalGas” részében publikált, a szállítási hónapra vonatkozó utolsó INDEX Price jegyzésár;

## 6.15.2. sp: eltérés (spread), értéke 1,05 EUR/MWh;

## 6.15.3. EURHUF: a szállítási hónapot követő hónap 16. napjával kezdődő, és a szállítási hónapot követő második hónap 15. napjával záródó időszakban a Bloomberg által a banki napokon közzétett BFIX EURHUF jegyzés budapesti idő szerint 14 óra 30 perckor érvényes értékeinek számtani átlaga. Banki napok alatt, a magyarországi munkaszüneti és a magyarországi munkarend áthelyezés eredményeképpen áthelyezésre kerülő munkanapok figyelmen kívül hagyásával, a hétfőtől péntekig terjedő napok értendők, beleértve a hétfői és pénteki napokat is;

## 6.16. PAktuálisimport ár_negyedéves átlag(import földgáz átlagos ára az adott naptári év negyedévében, HUF/kWh-ban kifejezve): az adott negyedév egyes hónapjaira vonatkozó PAktuálisimport ármennyiséggel súlyozott átlaga, ahol a mennyiségi súlyozás alapja az egyetemes szolgáltatók számára tervezett értékesítési profil;

## 6.17. PFedezettimport ár(import földgáz fedezett ára az adott hónapban, HUF/kWh-ban kifejezve): PFedezettimport ár= (fgSFedezett + sp) * EURHUFFedezett / 1000 + fk * EURHUF / 1000, ahol:

## 6.17.1. fgSFedezett: az egyetemes szolgáltatót ellátó földgázkereskedő által az adott hónapra kötött TTF-re vonatkozó fedezeti ügyletek mennyiséggel súlyozott átlagára EUR/MWh-ban (a fedezés az alábbi termékre történik: Argus European NaturalGas kiadvány „Complete European gasprices” részében közzétett, tárgyhónapra vonatkozó „TTF Ask” napi árak számtani átlaga a tárgyhónapot megelőző hónapban);

## 6.17.2. sp: eltérés (spread), értéke 1,05 EUR/MWh;

## 6.17.3. fk: tömegáru fedezési költség, értéke az fgSFedezett 0,25%-a + az fgSFedezett 0,075%-a;

## 6.17.4. EURHUFFedezett: az egyetemes szolgáltatót ellátó földgázkereskedő által az adott hónapra kötött EURHUF-ra vonatkozó fedezeti ügyletek mennyiséggel súlyozott átlagárfolyamának 0,1 HUF-fal növelt értéke;

## 6.18. PFedezetttárolói ár(tárolói földgáz fedezett ára az adott hónapban HUF/kWh-ban kifejezve) meghatározása:

## 6.18.1. Ha QAllokálttárolói fedezés +QHidegre_elkülönített tároló_havi<= QRendelkezésreálló tárolói fedezés, akkor

## PFedezetttárolói ár= (ΣQTárolóifedezés *(fgSFedezetttároló + sp) * EURHUFFedezetttároló / 1000 + fk * Σ(QTárolóifedezés * EURHUF) / 1000) / ( ΣQTárolóifedezés)

## 6.18.2. Ha QRendelkezésreálló tárolóifedezés > 0 és QAllokálttárolói fedezés +QHidegre_elkülönített tároló_havi> QRendelkezésreálló tárolói fedezés, akkor

## PFedezetttárolói ár= (QRendelkezésreálló tárolói fedezés * (ΣQTárolóifedezés *(fgSFedezetttároló + sp) * EURHUFFedezetttároló / 1000 + fk * Σ(QTárolóifedezés * EURHUF) / 1000) / ( ΣQTárolóifedezés)+ (QAllokálttárolói fedezés + QHidegre_elkülönített tároló_havi– QRendelkezésreálló tárolói fedezés) *(QTárolói_ténykészlet – ΣQTárolóifedezés – QNyitókészlet) * PNem_fedezett_tároló/ 1000 ) + QNyitókészlet * PNyitókészlet ) / (QTárolói_ténykészlet – ΣQTárolóifedezés)) / (QAllokálttárolói fedezés+ QHidegre_elkülönített tároló_havi)

## 6.18.3 Ha QRendelkezésreálló tárolói fedezés= 0, akkor

## PFedezetttárolói ár= (QTárolói_ténykészlet – ΣQTárolóifedezés – QNyitókészlet) * PNem_fedezett_tároló/ 1000) + QNyitókészlet * PNyitókészlet) / (QTárolói_ténykészlet – ΣQTárolóifedezés);

## 6.18.4 Ha6.18.2. kevesebb, mint a betárolási időszak végi egyetemes szolgáltatási célú fizikai készlet (QTárolói_ténykészlet), akkor:

## PFedezetttárolói ár = (ΣQTárolóifedezés * (fgSFedezetttároló + sp) * EURHUFFedezetttároló / 1000 + fk * Σ(QTárolóifedezés * EURHUF) / 1000 + QNyitókészlet * PNyitókészlet + (QTárolói_ténykészlet – ΣQTárolóifedezés – QNyitókészlet) * PNem_fedezett_tároló / 1000) / QTárolói_ténykészlet

## 6.18.5. Ahol:

## 6.18.5.1. fgSFedezetttároló: az egyetemes szolgáltatót ellátó földgázkereskedő által a betárolási időszakban a QTárolóifedezés(tárolói fedezett mennyiség)-ek keretében kötött TTF-re vonatkozó fedezeti ügyletek mennyiséggel súlyozott átlagára EUR/MWh-ban (a fedezés az alábbi termékre történik: Argus European NaturalGas kiadvány „Complete European gasprices” részében közzétett, tárgyhónapra vonatkozó „TTF Ask” napi árak számtani átlaga a tárgyhónapot megelőző hónapban);

## 6.18.5.2. sp: eltérés (spread), értéke 1,05 EUR/MWh;

## 6.18.5.3. fk: tömegáru fedezési költség, értéke az fgSFedezetttároló0,25%-a + az fgSFedezetttároló0,075%-a;

## 6.18.5.4. EURHUFFedezetttároló: az egyetemes szolgáltatót ellátó földgázkereskedő által, a betárolási időszakban a QTárolóifedezés(tárolói fedezett mennyiség)-ek keretében kötött EURHUF-ra vonatkozó fedezeti ügyletek mennyiséggel súlyozott átlagárfolyamának 0,1 HUF-fal növelt értéke;

## 6.18.5.5. PNem_fedezett_tároló: az adott betárolási időszak egyes hónapjaira vonatkozó PAktuálisimportárak (Qbeárazódott) mennyiségekkel súlyozott átlaga;

## 6.18.6. Commodity árazódási nap: A tárgyhónapot megelőző hónap első munkanapja.

## 6.18.7. Hátralévő nyári hónapok száma: A Commodity árazódási nap hónapját követő nyári hónapok száma, ahol nyárnak tekintendő április – szeptember időszak.

## 6.18.8. Tárolói fedezeti ügyletekhez tartozó kötési dátum: Az adott nyári betárolandó mennyiségek pénzügyi műveletekkel történő fedezéseihez tartozó kötési dátum az ügyletkötés dátumával azonos. Az ESZ szegmens nyári többlet- vagy alulfogyasztásának következtében fellépő fedezett fix tárolói pozícióváltozáshoz tartozó kötési dátum a mennyiségi változással érintett hónapot követő hónap 15. napja.

## 6.18.9. Qbeárazódott: (havi mennyiség kWh-ban) a Commodity árazódási napig megkötött tároló releváns tárolói fedezeti mennyiségekkel és beárazódott mennyiségekkel kiszámított lenti Q beárazódott képlettel azonos a beárazódott mennyiség.

## Qbeárazódott=(QTárolói_célkészlet - QHidegre_elkülönített tárolói készlet– Σ (QTárolóifedezés) – Σ1T-1 (Qbeárazódott)) / (hátralévő nyári hónapok száma)

## A fentiek alapján a Qbeárazódott , a QTárolóifedezés és a QHidegre_elkülönített tárolói készlet összege minden időpontban egyenlő a QTárolói_célkészlettel.

## 6.19. PHazaitermelés(hazai termelésből értékesített földgáz ára): a hazai termelésből beszerzett földgáz tárgyhónapra vonatkozóan HUF/kWh-ban meghatározott értékesítési ára, mely a hazai termelésű földgáz e rendelet szerint beszerzett, veszteség elszámolás nélkül számított árából kerül meghatározásra, figyelembe véve az ezt megelőzően átvett, de tárgyhónapig fel nem használt hazai termelésű földgáz veszteség elszámolás nélkül számított beszerzési árát is. A hazai termelésből értékesített földgáz árának mértékéről a Hivatal adatot szolgáltat az egyetemes szolgáltatót ellátó földgázkereskedő számára;

## 6.20. PHazaitermelés_negyedéves átlag(hazai termelésből beszerzett földgáz átlagos ára az adott naptári negyedévben): a tárgy naptári évet megelőző naptári év negyedéveire vonatkozó PHazaitermelésegyenletes ütemezésű tervezett napi mennyiségekkel (QHazaitermelés_negyedéves tervezett) súlyozott átlaga;

## 6.21. PAktuális_import_ár_téli_súlyozott_átlag(import földgáz mennyiséggel súlyozott átlagos ár az adott szeptemberi időpontot megelőző téli időszak alatt, HUF/kWh-ban kifejezve): az adott szeptembert közvetlen megelőző téli időszak (október - március) egyes hónapjaira vonatkozó PAktuális_import_ármennyiséggel súlyozott átlaga, ahol a mennyiségi súlyozás alapja a profilos zárókészlettel növelt tényfogyasztásnak és az adott hónap QTény tényfogyasztásának különbsége. A profilos zárókészlettel növelt tényfogyasztás az október - márciusi hónapok QTény tényfogyasztásainak és a QBiztonságizárókészletösszegének az október - március időszakra az egyetemes szolgáltatók számára tervezett értékesítés profil arányában való allokációja;

## 6.22. MtM (nyitott fedezeti ügyletek aktuális piaci értéke): az egyetemes szolgáltatót ellátó földgázkereskedő által kizárólag az egyetemes szolgáltatók ellátása érdekében kötött minden, a tárgyév utolsó napján nyitott, az egyetemes szolgáltatót ellátó földgázkereskedő számviteli nyilvántartásában a számvitelről szóló 2000. évi C. törvény 59/E. § alá nem tartozó fedezeti ügylet (beleértve a fedezett és tárolói fedezett mennyiségekre kötött tömegáru- és devizaügyleteket is) aktuális piaci értékének összege, a tárgyév utolsó napjára vonatkozóan meghatározva. Az MtM 2016. évi kezdeti értéke 0.

## 6.23. CEGY: az egyetemes szolgáltatót ellátó földgázkereskedő által végzett kiegyensúlyozó tevékenység indokolt havi költsége;

## 6.24. QNOM: a Get. 141/A. § és 141/J. § keretében földgázt vételező egyetemes szolgáltató számára (gáznapi igénybejelentésére) az egyetemes szolgáltatót ellátó földgázkereskedő által meghatározott napi nominált mennyiség [kWh];

## 6.25. QALL:a Get. 141/A. § és 141/J. § keretében földgázt vételező egyetemes szolgáltató adott gáznapi - a korrigált havi földgáz-forgalmi mérleg szerint - vételezett mennyisége [kWh];

## 6.26. Pelszámolóforgalmi díja: a kiegyensúlyozó földgáz-forgalmat elszámoló fél által felszámított forgalmi díj [Ft/kWh];

## 6.27. Pme: a szállítási rendszerüzemeltető által publikált gáznapi marginális eladási ár [Ft/kWh];

## 6.28. Pmv: a szállítási rendszerüzemeltető által publikált gáznapi marginális vételi ár [Ft/kWh];

## 6.29. n: az adott hónap napjainak száma.

## 6.30. QProfilozotttárolói összmennyiség (a kitárolási időszak hónapjaiban QTerv arányában felhasználandó - profilozott - tárolt mennyiség): értéke 2018/19-es gázév során 17 632 664 MWh, a további időszakokra vonatkozó eltérő értéket a Hivatal a honlapján közzéteszi;

## 6.31. QTárolói_ténykészlet: a betárolási időszak végi egyetemes szolgáltatási célú fizikai készlet;

## 6.31.1 QTárolói_célkészlet: a MEKH által rendeletben meghatározott betárolási időszak végére elérendő egyetemes szolgáltatási célú fizikai készlet;

## 6.32. QHidegre_elkülönített tárolói készlet (hidegre elkülönített tárolói készlet maradvány mennyisége): a betárolási időszak végi egyetemes szolgáltatási célú fizikai készlet (QTárolói_ténykészlet), és a felprofilozott tárolói készlet (QProfilozotttárolói összmennyiség) pozitív különbségéből az adott hónapig fel nem használt mennyiség;

## 6.32.1 QHidegre_elkülönített tároló_havi: A 6.32. szerinti QHidegre_elkülönített tárolói készletadott hónapban felhasznált mennyiség.

## 6.33. QTervezettimport (tervezett import mennyiség): a kitárolási hónapokban az egyetemes szolgáltatót ellátó földgázkereskedő által, az egyetemes szolgáltató ellátása céljából az adott tárgyhónapra a külön jogszabályban meghatározott földgáz mennyiségeken (QKedvezményesforrás) felül importálni tervezett, a kitárolási időszakot megelőzően meghatározandó mennyiség; értéke tárgyhónapban: QTervezettimport = QTerv - QHazaitermelés_tervezett - Qallokálttárolói fedezés – Qfedezett - QKedvezményesforrás, de legalább 0;

## 6.34. ΣQTárolóifedezés: a havi tárolói fedezett mennyiségek összege;

## 6.35. ELakosságicélú: A külön jogszabályban meghatározott, egyetemes szolgáltatót ellátó földgázkereskedő lakossági árak fenntarthatóságának céljából értékesített forrásainak eredménye, forintban kifejezve. A forrásokon realizált eredmény számítását az egyetemes szolgáltatót ellátó földgázkereskedő köteles transzparensen bemutatni a Hivatal részére ellenőrzés és szükség esetén felülvizsgálat céljára; [Ft]

## 6.36. QKedvezményesforrás: Külön jogszabályban meghatározott földgáz mennyiség, mely az egyetemes szolgáltatásban vételező felhasználók ellátása érdekében kerül az egyetemes szolgáltatót ellátó földgázkereskedő részére kedvezményes áron átadásra; [Ft/kWh]

## 6.37. PKedvezményesforrás ár: A külön jogszabályban meghatározott földgázmennyiség ára, melynek értékéről az egyetemes szolgáltatót ellátó földgázkereskedő tájékoztatja a Hivatalt. [Ft]

## 6.38. PLikvidimport ár(import likvid földgáz ára az adott hónapban, HUF/kWh-ban kifejezve): PLikvidimport ár= (fgL + spL) * EURHUFLikvid / 1000, ahol:

## 6.38.1. fgL: A szállítási hónapra vonatkozó az ICIS HEREN Report kiadvány „European Spot Gas Markets” részben publikált, az egyes napokat megelőző utolsó munkanapon közzétett „VTP Price Assessment - Day Ahead Bid” EUR/MWh napi árak számtani átlaga. Munkaszüneti nap esetén a munkaszüneti napot megelőző utolsó munkanapon publikált „VTP Price Assessment – Weekend Bid” EUR/MWh árakat kell figyelembe venni;

## 6.38.2. spL: eltérés (spread), értéke 0,0 EUR/MWh;

## 6.39. EURHUFLikvid: a szállítási hónapot követő hónap első 5 banki napjának a Bloomberg által közzétett BFIX EURHUF jegyzés budapesti idő szerint 14 óra 30 perckor érvényes értékeinek számtani átlaga. Banki napok alatt a magyarországi munkaszüneti napok és a magyarországi munkarend áthelyezés eredményeképpen áthelyezésre kerülő munkanapok figyelmen kívül hagyásával, a hétfőtől péntekig terjedő napok értendők beleértve a hétfői és pénteki napokat is.

## 6.40. QTöbblet: Az Allokált tárolói fedezés, a Fedezett import és a Kedvezményes árú forrás adott hónapra allokált részéből fogyasztásra fel nem használt mennyisége.

## 6.41. QTöbblet-1: Az Allokált tárolói fedezés, a Fedezett import és a Kedvezményes árú forrás a tárgyhónapot megelőző hónapra allokált részéből fogyasztásra fel nem használt mennyisége.

## 6.42. PTöbblet (HUF/kWh-ban kifejezve): a QTöbblet mennyiséggel súlyozott átlagára.

## 6.43. PTöbblet-1 (HUF/kWh-ban kifejezve): a QTöbblet-1 mennyiséggel súlyozott átlagára.”

4. melléklet a 21/2022. (IX. 30.) TIM rendelethez
