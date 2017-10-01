## Az adathálózatok számozási terve

## Az adathálózatok számozási terve az adathálózatok elérésére alkalmazott azonosítók felépítését, terjedelmét és a kijelölhető azonosítókat határozza meg. A számozási terv nem foglalkozik a hálózatokhoz tartozó előfizetők [elektronikus hírközlő végberendezések (a továbbiakban: végberendezés): adat-, illetőleg adatáramköri végberendezések] azonosítóival, ezeket a hálózatokat üzemeltető szolgáltatók osztják ki.

## A felosztási terv az ITU-T X.121 Ajánlása alapján készült. Az ITU-T E.164 alapú és X.121 alapú számozási tervek együttműködését az ITU-T E.166/X.122 Ajánlás szabályozza.

## 1. Adatátviteli nemzetközi szám

## 1.1. Leírás

## Az adatátviteli nemzetközi szám egy másik országbeli előfizető (adat-végberendezés, illetőleg adatáramköri végberendezés) elérése érdekében választandó szám, amely tartalmazza az adott ország azonosítására szolgáló számot, és a hívott előfizetői/adat-végberendezés adatátviteli belföldi számát.

## 1.2. A számok felépítése

## Az adatátviteli nemzetközi szám felépítése:

|  |  | DCC + NN |

| ahol: | DCC | (Data Country Code) adatátviteli országhívó szám, amelynek hossza három számjegy, egy országot határoz meg az adathálózati számozási tervben. A DCC-ben alkalmazható számjegyeket az ITU-T X.121 Ajánlás adja meg. Az adatátviteli országhívó számot az ITU jelöli ki. Magyarország adatátviteli országhívó száma: 216. |

|  | NN | (National Number) adatátviteli belföldi szám, amely legfeljebb tizenegy számjegyből áll. |

## 2. Adathálózati azonosító kód

## 2.1. Leírás

## Az adathálózati azonosító kód az adott országot és ezen belül valamely adathálózatot azonosítja.

## 2.2. A kódok felépítése

## Az adathálózati azonosító kód felépítése:

|  |  | DNIC = DCC + ND |

| ahol: | DNIC | (Data Network Identification Code) adathálózati azonosító kód |

|  | ND | (Network Digit) adatátviteli hálózatkijelölő szám, amely az országon belül egy adathálózatot határoz meg, és amely egyetlen számjegyből áll. |

## Az adathálózati azonosító kód maximális hossza négy számjegy lehet.

## 3. Adatátviteli belföldi szám

## 3.1. Leírás

## Az adatátviteli belföldi szám egy előfizetőt (adat-, illetve adatáramköri végberendezést) azonosít valamely országon belül.

## 3.2. A számok felépítése

## Az adatátviteli belföldi szám, NN (National Number) felépítése:

|  |  | NN = ND + NTN |

| ahol: | NTN | (Network Terminal Number) adatátviteli előfizetői szám, amely legfeljebb tíz számjegyből áll, és az adott hálózatban lévő előfizetők (adat-végberendezések, illetőleg adatáramköri végberendezések) azonosítására szolgál. |

4. melléklet a 3/2011. (IX. 26.) NMHH rendelethez[^20]

Jelzéspont kódok felosztási terve

A felosztási terv az ITU-T Q.708 Ajánlása alapján készült, figyelembe véve a Q.704 és Q.705 Ajánlásokban foglaltakat is.

A jelzéshálózatok közötti kapu szerepét betöltő jelzéspontok funkcionálisan egynél több jelzéshálózathoz tartoznak egyidejűleg. A 7-es jelzésrendszer címzési szabályai szerint egy kapu jelzéspontnak annyi jelzéspont kódjának kell lennie, ahány jelzéshálózathoz tartozik.

A hazai jelzéshálózat kétszintű, a nemzeti jelzéshálózatok egy nemzeti összekötő jelzéshálózaton át csatlakoznak egymáshoz.

A jelzéspont kódok számára egy 14 bit terjedelmű mező áll rendelkezésre. Ezt a mezőt az ITU-T a nemzetközi jelzéspont kódok esetében három részre osztotta, és meghatározta, hogy nemzetközi jelzéspont kódok esetében az egyes részek mit jelöljenek. A nemzeti jelzéspont kódok esetében a mező felosztására nincs ITU-T Ajánlás, a felosztás és a részek értelmezése szabadon választható. A 7-es jelzésrendszer a teljes mezőt együtt kezeli, a részekre osztás és értelmezés csak rendszerezési célokat szolgál. A részletes ismertetésben a bitmező részeit bittérkép helyett az átszámított decimális szám szemlélteti.

1. Nemzetközi jelzéspont kód

A nemzetközi jelzéshálózat NI (Network Indicator) bit kiosztása: 00

1.1. Leírás

A nemzetközi jelzéspont kód a nemzetközi jelzéshálózat jelzéspontjainak azonosítására szolgál.

1.2. A jelzéspont kód felépítése

A nemzetközi jelzéspont kód (ISPC, International Signalling Point Code) szerkezete:

|  |  | ISPC (14 bit) = SANC (3+8 bit) + SPI (3 bit) |

| ahol: | SANC | (Signalling Area/Network Code) jelzéspont tartomány/hálózat kód, melynek első, 3 bites része földrajzi zónát, a második, 8 bites része területet/országot határoz meg. A kódot az ITU jelöli ki. A rendelet hatálybalépésének időpontjáig Magyarország részére kijelölt jelzéspont tartomány/hálózat kódok: 2+032, 2+212, 4+243 és 6+251. |

|  | SPI | (Signalling Point Identification) jelzéspont azonosító. |

2. Nemzeti összekötő jelzéshálózati jelzéspont kód

A nemzeti összekötő jelzéshálózat NI bit kiosztása: 11

2.1. Leírás

A nemzeti összekötő jelzéshálózat (NISN, National Interconnecting Signalling Network) kapcsolatot teremt az egyes szolgáltatók/hálózat üzemeltetők nemzeti jelzéshálózata között.

Magyarországon egyetlen NISN van.

2.2. A jelzéspont kód felépítése

A nemzeti összekötő jelzéshálózati jelzéspont kód, a NISPC (National Interconnecting Signalling Point Code) szerkezete:

|  |  | NISPC (14 bit) = NIAA (5 bit) + NIBB (4 bit) + NICC (5 bit) |

| ahol: | NIAA + NIBB NICC | a nemzeti jelzéshálózatot kijelölő kód, a kapu jelzéspont kijelölő szám egy nemzeti jelzéshálózaton belül. |

3. Nemzeti jelzéshálózati jelzéspont kód

A nemzeti jelzéshálózatok NI bit kiosztása: 10

3.1. Leírás

Az egyes szolgáltatók/hálózat üzemeltetők a nemzeti jelzéshálózatukon belül a jelzések irányítására nemzeti jelzéshálózati jelzéspont kódokat alkalmaznak.

Magyarországon több, egymástól független nemzeti jelzéshálózat van.

3.2. A jelzéspont kód felépítése

A nemzeti jelzéshálózati jelzéspont kód, az NSPC (National Signalling Point Code) szerkezete:

| NSPC (14 bit) = tetszőleges. |

[^20]: A 4. melléklet az 1/2012. (I. 3.) NMHH rendelet 8. § (5) bekezdésével megállapított szöveg.
