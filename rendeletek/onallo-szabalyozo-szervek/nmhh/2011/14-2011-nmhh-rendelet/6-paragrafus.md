6. § (1) Ez a rendelet a kihirdetését követő negyvenötödik napon lép hatályba.

(2) Ez a rendelet 2015. december 31-én hatályát veszti.

Melléklet a 14/2011. (XII. 27.) NMHH rendelethez

Alkalmassági követelmények

Az az eszköz tekinthető alkalmasnak a magyarországi földfelszíni, szabad hozzáférésű digitális televíziós műsorszórás vételére, amely teljesíti az alábbi követelményeket:

a) Általános követelmények

Az eszköznek képesnek kell lennie az összes elérhető, az ETSI EN 300 744 szabvány szerinti DVB-T átviteli rendszer által továbbított, ISO/IEC 13818–1 szabvány szerinti „MPEG–2 Transport Stream” multiplex(ek) vételére és az ezen multiplexekben átvitt digitális szolgáltatások feldolgozására, amely magában foglalja az összes elérhető szabad hozzáférésű HD és SD televíziós és rádiós szolgáltatás dekódolását és megjelenítését/kiadását, valamint a kiegészítő szolgáltatások (pl. több kísérőhang, feliratok, EPG, szülői zár, teletext) elérhetővé tételét, az alábbi pontokban definiált további követelmények szerint.

b) RF követelmények

A VHF III sávban a CH5-CH12 csatornákban 7 MHz-es, valamint az UHF sávban a CH21-CH69 csatornákban 8 MHz-es csatorna sávszélességgel kell működnie.

c) Videokomponensek és képoldalarány jelzések dekódolása

Az eszköznek képesnek kell lennie a beérkező H.264/AVC (ITU-T H.264, illetve ISO/IEC 14496–10) video kódolási szabvány szerinti video adatfolyamok dekódolására.

SD minőségű jel esetén szükséges a „Main”, illetve a „High” profil támogatása „Level 3” szintig, a következő felbontások esetén: 720x576/50i, 704x576/50i, 544x576/50i, 480x576/50i, 352x576/50i, illetve 352x288/50i.

HD minőségű jel esetén szükséges a „High” profil támogatása „Level 4” szintig, a következő felbontások esetén: 1920x1080/50i, 1440x1080/50i, 1280x1080/50i, illetve 1280x720/50p.

Az eszköznek képesnek kell lennie a video adatfolyamban jelenlévő képoldalarányt meghatározó jelzésrendszerek folyamatos feldolgozására:

ca) H.264/AVC „aspect_ratio_idc” mező, mely a képkeret (frame) oldalarányát határozza meg.

cb) ETSI TS 101 154 – Annex B szerinti AFD (Active Format Description), mely a képkeretben átvitt ténylegesen „hasznos területeket” határozza meg. Amennyiben AFD jelzés nem kerül átvitelre, akkor a teljes frame tartalma hasznos területnek tekintendő.

d) Videojelek megjelenítése

Az eszköznek, a számítógépes vevőegység kivételével, a következő két (vagy a csatlakozott kijelző felületén ezekkel ekvivalens képernyőképet létrehozó) megjelenítési módot kell támogatnia: „4:3 letterbox” és „16:9 pillarbox”.

HD átvitelre alkalmas video kimenetek esetén, illetve a 16:9-es beépített kijelzőt tartalmazó készülékek esetén elégséges a „16:9 pillarbox” mód támogatása. RCA aljzaton biztosított összetett videojel kimenet esetén elégséges a „4:3”-as módok támogatása.

Ezen megjelenítési módok kiválasztása esetén az eszköznek mindig olyan videotartalmat és ehhez kapcsolódó képoldalarány jelzéseket kell kiadnia, melyek hatására a csatlakozott kijelző legalább két párhuzamos éléig, geometriai torzításoktól és „csonkolásoktól” mentesen, hasznos képtartalom tölti ki a kijelző felületét. Szükség esetén az eszköznek képesnek kell lennie a dekódolt videotartalom átskálázására (akár fekete kitöltősávok beillesztésével is a torzításmentes megjelenítés érdekében, valamint azokban az esetekben, amikor a megjelenítésre előkészített videotartalom és egy adott video kimenet felbontása különböző (SD – HD, illetve HD – SD konverziók).

da) „4:3 letterbox”: 4:3-as kijelzőt feltételez, ennek felületét a 4:3-as hasznos videotartalom teljes egészében ki kell, hogy töltse, míg egyéb esetekben megfelelő kitöltő sávokkal kell a hasznos tartalomnak kiegészülnie a torzításmentes megjelenítés érdekében.

db) „16:9 pillarbox”: 16:9-es kijelzőt feltételez, ennek felületét a 16:9-es hasznos videotartalom teljes egészében ki kell, hogy töltse, míg egyéb esetekben megfelelő kitöltő sávokkal kell a hasznos tartalomnak kiegészülnie a torzításmentes megjelenítés érdekében.

e) Audiokomponensek dekódolása

Az eszköznek képesnek kell lennie:

ea) ISO/IEC 11172–3 szabvány szerinti MPEG–1 Layer II szerint kódolt hangjelek dekódolására,

eb) ISO/IEC 14496–3 szabvány szerinti MPEG–4 HE-AAC szerint kódolt hangjelek dekódolására,

ec) ETSI TS 102 366 szabvány szerinti Dolby AC–3 szerint kódolt hangjelek dekódolására és sztereóra való lekeverésére. Az eszköznek képesnek kell lennie a dekódolt hangjelek kiadására televíziókészülék esetén a hangszórón keresztül, illetve vevődekóder esetén a jelenlévő sztereó kimeneteken (SCART és/vagy HDMI) keresztül.

f) Audiokomponensek kezelése

Az eszköznek képesnek kell lennie a televíziós szolgáltatások valamennyi elérhető kísérőhangja és a rádiós szolgáltatások hangjának vételére.

Az eszköznek folyamatosan frissítenie kell az aktuálisan kiválasztott szolgáltatáshoz tartozó audiokomponensek listáját.

Az eszköznek az ISO–639 nyelvi leíró alapján képesnek kell lennie szolgáltatásonként kijelezni az elérhető audio komponensek nyelvét, és felkínálni a felhasználó számára a választás lehetőségét.

g) A feliratozásra vonatkozó követelmények

Az eszköznek folyamatosan frissítenie kell az aktuálisan kiválasztott szolgáltatáshoz tartozó ETSI EN 300 743 szerinti DVB felirat komponensek listáját.

Az eszköznek az ISO–639 nyelvi leíró alapján képesnek kell lennie szolgáltatásonként kijelezni az elérhető feliratok nyelvét, és felkínálni a felhasználó számára a választás lehetőségét.

h) EPG (Electronic Programme Guide – elektronikus műsorújság) funkciók

Az eszköznek az ETSI EN 300 468 szerint definiált esemény-információs táblában (EIT) átvitt adatok felhasználásával támogatnia kell az EPG-t.

Az eszköznek képesnek kell lennie az EIT szövegmezők elejére opcionálisan beszúrt karaktertábla választó vezérlőbyte-ok kezelésére, és legalább a Latin–2 (ISO/IEC 8859–2) karaktertábla szerinti ékezethelyes megjelenítést támogatnia kell.

Az EPG-nek ki kell jeleznie az aktuálisan elérhető információk alapján:

– a program címét (a short_Event_descriptor Event_name mezője),

– a kezdési időt (az EIT start_time mezője),

– a program hosszát és/vagy végének időpontját (az EIT start_time + duration mezője),

– a program rövid leírását (short_event_descriptor), valamint

– a program hosszú leírását (extended_event_descriptor-ok összefűzése).

i) EIT alapú szülői zár funkció

Az eszköznek képesnek kell lennie az EIT-ben opcionálisan átvitt parental_rating_descriptor alapján az aktuálisan megtekintett műsorszám médiaszolgáltató általi korhatárbesorolása és a felhasználó által védett módon beállított szülői korhatár folyamatos összevetésére, szükség esetén az adott műsorszám video és audio komponenseinek elérését blokkolnia kell, mely blokkolás feloldása csak a felhasználó által korábban védett módon megadott PIN kód bevitelével lehetséges.

Az eszköznek legalább a következő korhatárok beállítását szükséges támogatnia: 6, 12, 16 és 18.

j) A teletextre (TXT) vonatkozó követelmények

Az eszköznek minden szolgáltatás esetében kezelnie kell a bejövő transzport adatfolyamba az ETSI EN 300 472 szerint opcionálisan beillesztett teletext (ETSI EN 300 706) komponenseket.

Az eszköznek rendelkeznie kell beépített OSD alapú teletext böngészővel. Az aktuális szolgáltatás teletextjét ezen keresztül – az ETSI EN 300 706 level 1.5-től definiált, X/26-on alapuló nyelvi kiterjesztés szerint kódolt ékezethelyes magyar karakterekkel – kell megjelenítenie. A beépített teletext böngészőnek támogatnia kell a teletext szolgáltatáson keresztüli felirat oldalak megjelenítését.

k) Az eszköznek (a televíziókészülék és számítógépes vevőegység kivételével) legalább az alábbi csatlakozófelületek egyikével rendelkeznie kell:

ka) EuroScart (legalább CVBS (WSS opcionális) szabványú alapsávi PAL video átvitelét kell támogatnia, emellett támogatnia kell a pin–8 alapú képarányjelzést, és a pin–16 alapú bemenetválasztást, valamint a sztereo hang kiadását),

kb) HDMI 1.3 (automatikus megjelenítő raszter méret felismeréssel és sztereo hang átvitelének lehetőségével).

l) Felhasználói kezelhetőség

Az eszköznek magyar nyelvű menüvel is rendelkeznie kell.
