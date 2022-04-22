3. melléklet a 14/2020. (XII. 15.) NMHH rendelethez

Jelzéspont kódok felosztási terve és a kódokkal való gazdálkodás rendjére vonatkozó különös szabályok

A felosztási terv az ITU-T Q.708 Ajánlás alapján készült, figyelembe véve a Q.704 és Q.705 Ajánlásokban foglaltakat is.

A jelzéshálózatok közötti kapu szerepét betöltő jelzéspontok funkcionálisan egynél több jelzéshálózathoz tartoznak egyidejűleg. A 7-es jelzésrendszer címzési szabályai szerint egy kapu jelzéspontnak annyi jelzéspont kódjának kell lennie, ahány jelzéshálózathoz tartozik.

A hazai jelzéshálózat kétszintű, a nemzeti jelzéshálózatok egy nemzeti összekötő jelzéshálózaton át csatlakoznak egymáshoz.

A jelzéspont kódok számára egy 14 bit terjedelmű mező áll rendelkezésre. Ezt a mezőt az ITU-T a nemzetközi jelzéspont kódok esetében három részre osztotta, és meghatározta, hogy nemzetközi jelzéspont kódok esetében az egyes részek mit jelöljenek. A nemzeti jelzéspont kódok esetében a mező felosztására nincs ITU-T Ajánlás, a felosztás és a részek értelmezése szabadon választható. A 7-es jelzésrendszer a teljes mezőt együtt kezeli, a részekre osztás és értelmezés csak rendszerezési célokat szolgál. A részletes ismertetésben a bitmező részeit bittérkép helyett az átszámított decimális szám szemlélteti.

1. NEMZETKÖZI JELZÉSPONT KÓD

A nemzetközi jelzéshálózat NI (Network Indicator) bit kiosztása: 00

1.1. Leírás

A nemzetközi jelzéspont kód a nemzetközi jelzéshálózat jelzéspontjainak azonosítására szolgál.

1.2. A jelzéspont kód felépítése

A nemzetközi jelzéspont kód (ISPC, International Signalling Point Code) szerkezete:

ISPC (14 bit) = SANC (3+8 bit) + SPI (3 bit), ahol

SANC (Signalling Area/Network Code) = jelzéspont tartomány/hálózat kód, melynek első, 3 bites része földrajzi zónát, a második, 8 bites része területet/országot határoz meg,

SPI (Signalling Point Identification) = jelzéspont azonosító.

1.3. A gazdálkodás rendje

A jelzéspont tartomány/hálózat kódot (SANC) az ITU jelöli ki. A rendelet hatálybalépésének időpontjáig Magyarország részére kijelölt jelzéspont tartomány/hálózat kódok: 2+032, 2+212, 4+243, 5+218 és 6+251.

A jelzéspont azonosítót (SPI) a hatóság jelöli ki. Egy jelzéspont számára egy nemzetközi jelzéspont kód (jelzéspont azonosító) jelölhető ki. A jelzéspont azonosító kijelölését és visszavonását a hatóság az ITU részére bejelenti.

Nemzetközi jelzéspont kód (jelzéspont azonosító) jelölhető ki azon szolgáltatók számára, amelyeket a hatóság az elektronikus hírközlési szolgáltatókról vezetett nyilvántartásba bejegyzett.

2. NEMZETI ÖSSZEKÖTŐ JELZÉSHÁLÓZATI JELZÉSPONT KÓD

A nemzeti összekötő jelzéshálózat NI bit kiosztása: 11

2.1. Leírás

A nemzeti összekötő jelzéshálózat (NISN, National Interconnecting Signalling Network) kapcsolatot teremt az egyes szolgáltatók/hálózat üzemeltetők nemzeti jelzéshálózata között. Magyarországon egyetlen NISN van.

2.2. A jelzéspont kód felépítése

A nemzeti összekötő jelzéshálózati jelzéspont kód (NISPC, National Interconnecting Signalling Point Code) szerkezete:

NISPC (14 bit) = NIAA (5 bit) + NIBB (4 bit) + NICC (5 bit), ahol

NIAA + NIBB = a nemzeti jelzéshálózatot kijelölő kód,

NICC = a kapu jelzéspont kijelölő szám egy nemzeti jelzéshálózaton belül.

2.3. A gazdálkodás rendje

A nemzeti összekötő jelzéshálózati jelzéspont kódjának (NISPC) az NIAA + NIBB nemzeti jelzéshálózatot kijelölő kód részeit a hatóság határozza meg.

Egy adott NIAA + NIBB kódhoz tartozó NICC tartomány kijelölő számait a szolgáltató kérésére a hatóság jelöli ki a szolgáltató kapu jelzéspontjai számára.

Nemzeti összekötő jelzéshálózati jelzéspont kód jelölhető ki azon szolgáltatók számára, amelyeket a hatóság az elektronikus hírközlési szolgáltatókról vezetett nyilvántartásba bejegyzett.

3. NEMZETI JELZÉSHÁLÓZATI JELZÉSPONT KÓD

A nemzeti jelzéshálózatok NI bit kiosztása: 10

3.1. Leírás

Az egyes szolgáltatók/hálózat üzemeltetők a nemzeti jelzéshálózatukon belül a jelzések irányítására nemzeti jelzéshálózati jelzéspont kódokat alkalmaznak.

Magyarországon több, egymástól független nemzeti jelzéshálózat van.

3.2. A jelzéspont kód felépítése

A nemzeti jelzéshálózati jelzéspont kód, az NSPC (National Signalling Point Code) szerkezete:

NSPC (14 bit) = tetszőleges.

3.3. A gazdálkodás rendje

Nemzeti jelzéshálózat létesítésére a szolgáltató azzal kap felhatalmazást, ha számára a hatóság meghatározza az NISPC-hez tartozó NIAA + NIBB kódokat.

Az NSPC kiosztását a szolgáltató végzi.
