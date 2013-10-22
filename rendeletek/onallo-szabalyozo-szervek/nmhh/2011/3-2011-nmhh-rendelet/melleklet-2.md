## A beszédcélú elektronikus hírközlő hálózatok számozási terve

## Ez a számozási terv meghatározza a beszédcélú elektronikus hírközlő hálózatokban használatos számok típusát, a különböző típusú számok felépítését, terjedelmét, a számhasználat feltételeit, az előtéteket és a tárcsázási eljárásokat.

## A számozási terv a Nemzetközi Távközlési Egyesület (International Telecommunication Union, a továbbiakban: ITU) ITU-T E.164 és E.213 Ajánlása és az MSZ ETS 300 927 szabványa alapján készült.

## 1. NEMZETKÖZI SZÁMOK FELOSZTÁSA

## 1.1. Leírás

## A nemzetközi szám egy másik ország, globális szolgáltatás vagy nemzetközileg azonosított hálózat (a továbbiakban: Hálózat) előfizetőjének elérése érdekében tárcsázandó, az ITU-T E.164. Ajánlásban meghatározott felépítésű szám, amely tartalmazza az országkódot és a hívott előfizető belföldi számát, de nem tartalmazza a nemzetközi előtétet, sem az adott ország belföldi előtétjét.

## 1.2. A számok felépítése

## A nemzetközi szám formátumai:

## a) A földrajzi területek nemzetközi száma:

|  |  | OS + Belföldi szám |

| ahol: | OS | a földrajzi terület országkódja. |

## Az OS egy, kettő vagy három számjegyből áll. Magyarország országkódja: 36.

## b) A globális szolgáltatások nemzetközi száma:

|  |  | OS + GES |

| ahol: | OS | a globális szolgáltatás országkódja, |

|  | GES | globális előfizetői szám, amely a globális szolgáltatás egy előfizetőjét határozza meg. |

## Az OS három számjegyből áll. A GES legfeljebb tizenkét számjegyű lehet.

## c) A Hálózatok nemzetközi száma:

|  |  | OS + AK + ES |

| ahol: | OS | a Hálózat országkódja, |

|  | AK | Hálózat azonosító kód, |

|  | ES | előfizetői szám, amely a Hálózat egy előfizetőjét határozza meg. |

## Az OS három számjegyből áll és a Hálózatok egy csoportját azonosítja. Az AK egy, kettő, három vagy négy számjegyből áll. Az adott Hálózatot az OS és AK együtt azonosítják.

## 1.3. A számok használatának adminisztrációja

## Az országkódot minden esetben az ITU határozza meg.

## A globális előfizetői számot a szolgáltató kérésére az ITU jelöli ki.

## A Hálózat azonosító kódot az ITU, a Hálózat előfizetői számait a Hálózat szolgáltatója jelöli ki.

## 1.4. A használat feltételei

## Az 1.2 pont b) és c) pontjában meghatározott globális szolgáltatások és Hálózatok nemzetközi számainak kijelölési és használati feltételeit ITU-T Ajánlások határozzák meg.

## Az ITU-T E.152 Ajánlásban meghatározott OS=800 egyetemes nemzetközi díjmentes szolgáltatás (Universal International Freephone Service) számainak elérését a hívó részére díjmentesen kell biztosítani, feltéve, hogy a hívó fél a hívást honos hálózatából, barangolás igénybevétele nélkül kezdeményezi. A hívás és üzenetküldés díját a hívott fél fizeti. A barangolásból adódó többletköltségeket a hívó fél viseli.

## A nemzetközi hívás lehetőségét a szolgáltató az előfizetője kérésére köteles letiltani.

## 2. BELFÖLDI SZÁMOK FELOSZTÁSA ÉS MEGHATÁROZÁSA

## 2.1. A belföldi számok felosztása

## 2.1.1. Leírás

## A belföldi szám egy magyarországi előfizetői hozzáférési pont vagy szolgáltatás elérése érdekében tárcsázandó szám, amely tartalmazza a belföldi rendeltetési számot és az előfizetői számot, de nem tartalmazza a belföldi előtétet.

## 2.1.2. A számok felépítése

## A belföldi szám két részből áll:

|  |  | BRS + ES |

| ahol: | BRS | belföldi rendeltetési szám, amely egy földrajzilag vagy más módon elkülönülten kezelt hálózathoz vagy szolgáltatáshoz tartozó számozási tartományt határoz meg, |

|  | ES | előfizetői szám, amely egy BRS által meghatározott számozási tartományban egy előfizetői hozzáférési pont vagy egy szolgáltatás hívására vagy elérésére szolgál. |

## A belföldi szám hossza 8, 9 vagy 12 számjegy. Egy számozási tartományban a belföldi szám hossza azonos.

## A belföldi rendeltetési szám típusai:

|  | KS | körzetszám, amely az ország egy földrajzilag elkülönített területéhez (a továbbiakban: földrajzi számozási terület) tartozó, helyhez kötött felhasználású számozási tartományt határoz meg, |

|  | SHS | szolgáltatás- vagy hálózatkijelölő szám, amely nem földrajzi alapon elkülönülten kezelt szolgáltatáshoz vagy hálózathoz tartozó számozási tartományt határoz meg. |

## A belföldi szám típusa KS esetén földrajzi szám, SHS esetén nem-földrajzi szám.

## 2.1.3. A körzetszámok felosztása

## A körzetszám egy- vagy kétjegyű szám.

## A körzetszámok és a földrajzi számozási területek összerendelését az alábbi táblázat tartalmazza:

|  |  | A | B |

|  | 1 | KS | Földrajzi számozási terület |

|  | 2 | 1 | Budapest |

|  | 3 | 22 | Székesfehérvár |

|  | 4 | 23 | Biatorbágy |

|  | 5 | 24 | Szigetszentmiklós |

|  | 6 | 25 | Dunaújváros |

|  | 7 | 26 | Szentendre |

|  | 8 | 27 | Vác |

|  | 9 | 28 | Gödöllő |

|  | 10 | 29 | Monor |

|  | 11 | 32 | Salgótarján |

|  | 12 | 33 | Esztergom |

|  | 13 | 34 | Tatabánya |

|  | 14 | 35 | Balassagyarmat |

|  | 15 | 36 | Eger |

|  | 16 | 37 | Gyöngyös |

|  | 17 | 42 | Nyíregyháza |

|  | 18 | 44 | Mátészalka |

|  | 19 | 45 | Kisvárda |

|  | 20 | 46 | Miskolc |

|  | 21 | 47 | Szerencs |

|  | 22 | 48 | Ózd |

|  | 23 | 49 | Mezőkövesd |

|  | 24 | 52 | Debrecen |

|  | 25 | 53 | Cegléd |

|  | 26 | 54 | Berettyóújfalu |

|  | 27 | 55 | teszt-körzet |

|  | 28 | 56 | Szolnok |

|  | 29 | 57 | Jászberény |

|  | 30 | 59 | Karcag |

|  | 31 | 62 | Szeged |

|  | 32 | 63 | Szentes |

|  | 33 | 66 | Békéscsaba |

|  | 34 | 68 | Orosháza |

|  | 35 | 69 | Mohács |

|  | 36 | 72 | Pécs |

|  | 37 | 73 | Szigetvár |

|  | 38 | 74 | Szekszárd |

|  | 39 | 75 | Paks |

|  | 40 | 76 | Kecskemét |

|  | 41 | 77 | Kiskunhalas |

|  | 42 | 78 | Kiskőrös |

|  | 43 | 79 | Baja |

|  | 44 | 82 | Kaposvár |

|  | 45 | 83 | Keszthely |

|  | 46 | 84 | Siófok |

|  | 47 | 85 | Marcali |

|  | 48 | 87 | Tapolca |

|  | 49 | 88 | Veszprém |

|  | 50 | 89 | Pápa |

|  | 51 | 92 | Zalaegerszeg |

|  | 52 | 93 | Nagykanizsa |

|  | 53 | 94 | Szombathely |

|  | 54 | 95 | Sárvár |

|  | 55 | 96 | Győr |

|  | 56 | 99 | Sopron |

## Az egyes földrajzi számozási területekhez tartozó települések felsorolását, az érintett szolgáltatókkal történt egyeztetés után, a hatóság a honlapján teszi közzé.

## 2.1.4. A szolgáltatás- vagy hálózatkijelölő számok felosztása

## A szolgáltatás- vagy hálózatkijelölő szám kétjegyű.

## Az SHS-ek és a szolgáltatások, vagy hálózatok összerendelését az alábbi táblázat tartalmazza:

|  |  | A | B |

|  | 1 | SHS | Szolgáltatás vagy hálózat |

|  | 2 | 20 | Mobil rádiótelefon szolgáltatás |

|  | 3 | 21 | Nomadikus telefonszolgáltatás |

|  | 4 | 30 | Mobil rádiótelefon szolgáltatás |

|  | 5 | 31 | Mobil rádiótelefon szolgáltatás |

|  | 6 | 38 | Üzleti hálózatok |

|  | 7 | 40 | Kedvezményes díjazású szolgáltatás |

|  | 8 | 50 | Mobil rádiótelefon szolgáltatás |

|  | 9 | 51 | Internet-hozzáférési szolgáltatás |

|  | 10 | 60 | Mobil rádiótelefon szolgáltatás |

|  | 11 | 70 | Mobil rádiótelefon szolgáltatás |

|  | 12 | 71 | Gépek közötti kommunikáció |

|  | 13 | 80 | Díjmentes szolgáltatás |

|  | 14 | 90 | Emelt díjas, díjkorlátmentes szolgáltatás és emelt díjas felnőtt szolgáltatás |

|  | 15 | 91 | Emelt díjas, díjkorlátos szolgáltatás |

## 2.1.5. Hívószám azonosítás

## Az egyes szolgáltatások igénybevétele során, a szolgáltatás igénybevételét kezdeményező azonosítására szolgáló, a hívott, elért végződtetési ponton megjeleníthető azonosító („A” szám) csak az ANFT-ben meghatározott módon és formában jeleníthető meg.

## Ennek megfelelően, a beszédcélú elektronikus hírközlő hálózatokban hívás és üzenetküldés kezdeményezésekor a hívó azonosítójaként a számjegyeken és a + karakteren kívül más karakter nem használható.

## 2.2. Földrajzi számok

## 2.2.1. Leírás

## A földrajzi számok helyhez kötött telefonhálózathoz csatlakozó előfizetők azonosítását és elérését teszik lehetővé.

## A földrajzi szám körzetszám része az előfizetői hozzáférési pont helye szerinti földrajzi számozási területet jelöli ki.

## 2.2.2. A számok felépítése

## A földrajzi szám körzetszámból és előfizetői számból áll.

## A szám felépítése egyjegyű körzetszám esetén:

|  |  | A abc defg |

| ahol: | A | körzetszám |

|  | abc defg | előfizetői szám 200 0000-999 9999 között. |

## Kétjegyű körzetszám esetén: AB abc def

| ahol: | AB | körzetszám |

|  | abc def | előfizetői szám 200 000-999 999 között. |

## A körzetszám a földrajzi számozási területet jelöli ki a 2.1.3. pont táblázata szerint.

## 2.2.3. A használat feltételei

## A földrajzi szám csak a körzetszámhoz tartozó földrajzi számozási területen elhelyezett előfizetői hozzáférési ponthoz rendelhető.

## Földrajzi számon különleges díjazású (a díjmentes, a kedvezményes díjazású, az emelt díjas) szolgáltatás, valamint nomadikus telefonszolgáltatás nem nyújtható.

## 2.3. Mobil számok (SHS = 20, 30, 31, 50, 60, 70)

## 2.3.1. Leírás

## A mobil számok a mobil rádiótelefon hálózathoz csatlakozó előfizetők azonosítását és elérését teszik lehetővé mobil rádiótelefon illetőleg mobil internet hozzáférési szolgáltatás igénybevételéhez.

## 2.3.2. A számok felépítése

## A mobil szám szolgáltatáskijelölő számból és előfizetői számból áll:

|  |  | AB abc defg |

| ahol: | AB | mobil rádiótelefon szolgáltatást jelölő SHS, |

|  | abc defg | előfizetői szám 000 0000-999 9999 között. |

## 2.3.3. A használat feltételei

## A mobil számon kedvezményes díjazású és emelt díjas szolgáltatás, nomadikus telefonszolgáltatás, valamint – amennyiben az Európai Unió általános hatályú, közvetlenül alkalmazandó kötelező jogi aktusa eltérően nem rendelkezik – díjmentes szolgáltatás nem nyújtható.

## 2.4. Nomadikus telefonszolgáltatás számai (SHS = 21)

## 2.4.1. Leírás

## A nomadikus számok a nyilvános elektronikus hírközlő hálózathoz – általában helyhez kötött vagy mobil internet hozzáférésen – csatlakozó nomadikus telefonszolgáltatás előfizetők azonosítását és elérését teszik lehetővé.

## 2.4.2. A számok felépítése

|  |  | 21 abc defg |

| ahol: | 21 | nomadikus telefonszolgáltatást jelölő SHS, |

|  | abc defg | előfizetői szám 200 0000-999 9999 között. |

## 2.4.3. A használat feltételei

## Az előfizetői számokon helyhez kötött telefonszolgáltatás, mobil rádiótelefon szolgáltatás, különleges díjazású (a díjmentes, a kedvezményes díjazású, az emelt díjas) szolgáltatás nem nyújtható.

## 2.5. Kedvezményes díjazású szolgáltatás számai (ún. kék számok) (SHS = 40)

## 2.5.1. Leírás

## Lehetővé teszi a telefonhálózatból a 2. § 2. pontban meghatározott kedvezményes díjazású szolgáltatások elérését.

## 2.5.2. A számok felépítése

## A kedvezményes díjazású szolgáltatás száma szolgáltatás kijelölő számból és előfizetői számból áll:

|  |  | 40 abc def |

| ahol: | 40 | a kedvezményes díjazású szolgáltatást jelölő SHS, |

|  | abc def | előfizetői szám 100 000-999 999 között. |

## 2.5.3. A használat feltételei

## A szolgáltatónak kötelessége, hogy a hálózatából kedvezményes díjazású szolgáltatások elérésére kezdeményezett hívások hívó által fizetendő, az általános forgalmi adót (a továbbiakban: áfa) tartalmazó hívásdíját az általános szerződési feltételeiben közzétegye. A szolgáltató a hívó fél által fizetendő díjat úgy köteles meghatározni, hogy az ne haladja meg a hatóság által az érintett szolgáltatókkal történő egyeztetést követően – évente január 31-ig – a hatóság internetes honlapján közzétett díjat.

## A számhasználó kérésére – kereskedelmi okból – a szolgáltatónak korlátoznia kell a kedvezményes díjazású szolgáltatás nemzetközi hálózatból, valamint meghatározott belföldi KS-sel, illetve SHS-sel azonosított számtartományokból való elérését.

## A kedvezményes díjazású szolgáltatás szám számhasználója által kezdeményezett hívásoknál a kedvezményes díjazású szolgáltatás szám a hívottnál hívószám kijelzés szolgáltatással a hívó telefonszámaként nem jeleníthető meg.

## 2.6. Internet-hozzáférési szolgáltatás számai (SHS = 51)

## 2.6.1. Leírás

## Lehetővé teszi internetszolgáltatók telefonhálózaton keresztül történő elérését.

## 2.6.2. A számok felépítése

|  |  | 51 abc def |

| ahol: | 51 | internet-hozzáférési szolgáltatást jelölő SHS, |

|  | abc | a közreműködő szolgáltatót határozza meg, amely az internetszolgáltatóval a hívások eljuttatása tárgyában hálózati szerződéses jogviszonyban áll, |

|  | def | a közreműködő szolgáltató hálózatán keresztül elérhető internetszolgáltatót és annak szolgáltatását azonosítja. A közreműködő szolgáltató saját azonosító tartományából jelöli ki. |

## Egy közreműködő szolgáltatóhoz több „abc”, és egy internetszolgáltatóhoz több „def” azonosító tartozhat.

## 2.6.3. A használat feltételei

## Az internetszolgáltatás hívószáma nem tehető közzé a hívó által fizetendő díj és a díjazási feltételek ismertetése nélkül.

## A közreműködő szolgáltató feladatát az internetszolgáltató is elláthatja.

## 2.7. Díjmentes szolgáltatás számai (ún. zöld számok) (SHS = 80)

## 2.7.1. Leírás

## A számhasználónak vagy az általa nyújtott szolgáltatásnak a hívó fél részére díjmentes elérését teszi lehetővé, feltéve, hogy a hívó fél a hívást a részére előfizetői szolgáltatást nyújtó szolgáltató hálózatából (honos hálózat) kezdeményezi.

## 2.7.2. A számok felépítése

## A díjmentes szolgáltatás száma szolgáltatás kijelölő számból és előfizetői számból áll:

|  |  | 80 abc def |

| ahol: | 80 | a díjmentes szolgáltatást jelölő SHS, |

|  | abc def | előfizetői szám, amelynek értéke: 000 000-099 999, ha belföldi formában tárcsázható nemzetközi hívószám, ahol a hívás nemzetközi hívószámon, illetve más országban végződik 100 000-999 999, ha belföldi hívószám, ahol a hívás belföldi hívószámon, illetve belföldön végződik. |

## 2.7.3. A használat feltételei

## A hívás és üzenetküldés díját a számhasználó fizeti. A hívás és üzenetküldés a hívó fél részére díjmentes, feltéve, hogy a hívó fél a hívást honos hálózatából, barangolás igénybevétele nélkül kezdeményezi. A barangolásból adódó többletköltségeket a hívó fél viseli.

## A számhasználó kérésére – kereskedelmi okból – a szolgáltatónak korlátoznia kell a díjmentes szolgáltatás nemzetközi hálózatból, valamint meghatározott belföldi KS-sel, illetve SHS-sel azonosított számtartományokból való elérését.

## A díjmentes szolgáltatás szám számhasználója által kezdeményezett hívásoknál a díjmentes szolgáltatás szám a hívottnál hívószám kijelzés szolgáltatással a hívó telefonszámaként nem jeleníthető meg.

## 2.8. Emelt díjas szolgáltatás számai (SHS = 90, 91)

## 2.8.1. Leírás

## Lehetővé teszi a telefonhálózatból információt, tartalmat nyújtó, emelt díjas szolgáltatások elérését.

## 2.8.2. A számok felépítése

|  |  | 90 abc def 91 abc def |

| ahol: | 90 91 | az emelt díjas, díjkorlátmentes és emelt díjas felnőtt szolgáltatást jelölő SHS, az emelt díjas, díjkorlátos szolgáltatást jelölő SHS |

|  | abc def | előfizetői szám 100 000-999 999 között. |

## 2.8.3. A szolgáltatás kategóriák használati feltételei

## Az SHS=90 számtartomány számain a szolgáltatónak megfelelő intézkedésekkel biztosítania kell, hogy kiskorú előfizető ne érhessen el olyan szolgáltatást, amelyen keresztül felnőtt tartalom hozzáférhető. Ez a korlátozás a kiskorú előfizető esetében törvényes képviselőjének kérésére sem oldható fel.

## Az SHS=91 számtartomány számain nem nyújtható felnőtt tartalom. A szolgáltató a hívó fél által fizetendő legmagasabb díjat úgy köteles meghatározni, hogy az ne haladja meg a hatóság által az érintett szolgáltatókkal történő egyeztetést követően – évente január 31-ig – a hatóság internetes honlapján közzétett díjat.

## 2.8.4. A számhasználat általános feltételei

## A szolgáltatás tartalmára vonatkozó feltételek betartásáért a számhasználó felel.

## A számhasználó minden esetben köteles az emelt díjas szolgáltatás hívószámának közzétételével együtt a hívó fél által fizetendő, áfát tartalmazó díj mértékét is (hívásonkénti vagy percenkénti díj, vagy az üzenetküldés díja) nyilvánosságra hozni. A szolgáltatás díja mellett fel kell tüntetni, hogy annak megfizetése indított emelt díjas hívással, vagy üzenetküldéssel történik, valamint fogadott emelt díjas szolgáltatás esetén azt, hogy maximálisan hány üzenet küldésére kerül sor a szolgáltatás igénybevétele során. Ugyancsak fel kell tüntetni a számhasználó megnevezését, valamint a szolgáltatáshoz kapcsolódó ügyfélszolgálat elérhetőségét telefonon, postai és elektronikus úton.

## Az emelt díjas szolgáltatások elérését az előfizetője kérésére a szolgáltató köteles díjmentesen letiltani. Ennek lehetőségéről a szolgáltató az előfizetőket honlapján, illetve ügyfélszolgálatán megfelelően tájékoztatni köteles.

## A fogadott emelt díjas szolgáltatás nyújtására használható számokra vonatkozóan a szolgáltató minden előfizetőjénél díjmentesen alapértelmezett tiltást köteles berendezni. A tiltás csak az előfizető megfelelő azonosítását követően tett kifejezett és egyértelmű nyilatkozatára oldható fel. A szolgáltatónak biztosítania kell, hogy az emelt díjas szolgáltatás nyújtására használható számok hívásának, illetve az ilyen számokra küldött, vagy onnan fogadott üzeneteknek tiltására, illetve feloldásra vonatkozó nyilatkozatát az előfizető bármikor ingyenesen megtehesse, illetve visszavonhassa. Az emelt díjas szolgáltatás nyújtására használható számok hívására, illetve az ilyen számokra küldött, vagy onnan fogadott üzenetekre vonatkozó tiltás, illetve feloldás a szolgáltatás rendelkezésre állásának állapotát jelenti, ezért tiltás feloldására vonatkozó nyilatkozat megtétele, továbbá a tiltás újbóli beállítására vonatkozó nyilatkozat megtétele nem minősül az előfizetői szerződés módosításának. Ennek részletes feltételeit a szolgáltató Általános Szerződési Feltételeiben határozza meg, de a nyilatkozat megtételének és visszavonásának lehetőségét legalább telefonos ügyfélszolgálatán biztosítania kell.

## Amennyiben az emelt díjas szolgáltatás elérhetőségével, igénybevehetőségével, vagy a szolgáltató által kiszámlázott díjával kapcsolatban az igénybevevő a számára előfizetői szolgáltatást nyújtó elektronikus hírközlési szolgáltatónál reklamációt terjeszt elő, az elektronikus hírközlési szolgáltató köteles gondoskodni a reklamáció hatályos jogszabályoknak megfelelő kivizsgálásáról. Az ilyen vitatott díj meg nem fizetése miatt az igénybevevő számára elektronikus hírközlési szolgáltatást nyújtó szolgáltató az elektronikus hírközlési szolgáltatás nyújtását nem korlátozhatja, nem szüneteltetheti, és az előfizetői szerződést erre hivatkozva rendkívüli felmondással nem szüntetheti meg.

## Az emelt díjas szolgáltatás szám használatára feljogosított számhasználó által kezdeményezett hívásoknál az emelt díjas szolgáltatás szám a hívottnál hívószám kijelzés szolgáltatással a hívó telefonszámaként nem jeleníthető meg.

## 2.9. Üzleti hálózatok számai (SHS=38)

## 2.9.1. Leírás

## Az előfizetők egy meghatározott csoportját – jellemzően egy céget, vagy egyéb szervezetet – kiszolgáló hálózat, azaz üzleti hálózat (Corporate Network) tagjainak elérését biztosítja a telefonhálózatból. Az üzleti hálózat összekapcsolja az adott szervezet magánhálózati és/vagy virtuális magánhálózati elemeit, ezen kívül lehetőséget biztosít az elektronikus hírközlő hálózat elérésére. Egy üzleti hálózat egyaránt tartalmazhat elektronikus hírközlési szolgáltatói és saját hálózati elemeket.

## 2.9.2. A számok felépítése

|  |  | 38 abc defg |

| ahol: | 38 | az üzleti hálózatot jelölő SHS |

|  | abc defg | előfizetői szám 200 0000-999 9999 között. |

## 2.9.3. A használat feltételei

## Az SHS=38 számtartomány számain nyilvánosan elérhető elektronikus hírközlési szolgáltatást üzleti hálózaton kívüli előfizetők részére nem nyújtható.

## 2.10. Gépek közötti kommunikáció számai (ún. M2M számok) (SHS=71)

## 2.10.1. Leírás

## Az elektronikus hírközlő hálózaton olyan kommunikációt tesz lehetővé a végberendezések vagy alkalmazások között, ahol az információt legfeljebb csekély emberi beavatkozással továbbítják.

## 2.10.2. A számok felépítése

|  |  | 71 abc def ghij |

| ahol: | 71 | a gépek közötti kommunikációt jelölő SHS |

|  | abc def ghij | előfizetői szám 200 000 0000-999 999 9999 között. |

## 2.10.3. A használat feltételei

## A számok használatának egyes alkalmazásokra vonatkozó feltételeit a hatóság a kijelölési engedélyben határozza meg. A számokon adat- vagy hangkommunikáció, illetve üzenetküldés kizárólag a hatóság számmező kijelölési határozatában megadott jelleggel illetve módon, az alkalmazáshoz tartozó végberendezések és alkalmazások között létesíthető.

## Az SHS=71 számtartomány számain helyhez kötött telefonszolgáltatás, mobil rádiótelefon szolgáltatás és nomadikus telefonszolgáltatás nem nyújtható.

## 3. RÖVID KÓDOK FELOSZTÁSA ÉS MEGHATÁROZÁSA

## 3.1. A rövid kódok felosztása

## 3.1.1. Leírás

## A rövid kód legfeljebb hatjegyű szám, amelynek struktúrája eltér az ITU-T E.164 Ajánlásban meghatározott nemzetközi és belföldi számok struktúrájától. Rövid kódok kizárólag számjegyeket tartalmazhatnak.

## A rövid kódoknak kétféle típusa van: előtét és rövid szám.

## Előtét: legfeljebb négyjegyű szám, amelyet a nemzetközi vagy belföldi szám előtt kell tárcsázni, és amely jelöli a tárcsázott számformátumot (nemzetközi vagy belföldi), vagy a választott közvetítő szolgáltatót, vagy egy kiegészítő szolgáltatást. Egy hívásban több különböző előtét is alkalmazható.

## Rövid szám: legalább három-, legfeljebb hatjegyű nem-földrajzi szám, amelynek hívásával egy szolgáltatás érhető el. A rövid szám nemzetközi hálózatból nem elérhető.

## 3.1.2. A rövid kódok felosztása

## A rövid kód első számjegye 0 vagy 1.

## A rövid kódok és rövid kód tartományok felosztása:

|  |  | A | B |

|  | 1 | 00 | nemzetközi előtét (NE) |

|  | 2 | 06 | belföldi előtét (BE) |

|  | 3 | 104 105 107 112 | segélyhívó számok |

|  | 4 | 116* | harmonizált közérdekű szolgáltatások harmonizált számai |

|  | 5 | 118* | telefontudakozó számok |

|  | 6 | 12* | elektronikus hírközlési szolgáltatók ügyfélszolgálati számai |

|  | 7 | 130 131 | kiegészítő szolgáltatás előtétek |

|  | 8 | 135* 136* | adománygyűjtő számok |

|  | 9 | 137* | lelki segítő és támogató szolgáltatás számok |

|  | 10 | 14* | különös díjazású országos számok |

|  | 11 | 15* | közvetítő választó előtétek (KVE) |

|  | 12 | 16* | emelt díjas szolgáltatás rövid számok |

|  | 13 | 17* | elektronikus hírközlési szolgáltató hálózatához rendelt számok |

|  | 14 | 18* | közérdekű tájékoztató és támogató szolgáltatások számai |

|  | 15 | 192 193 | telefonos kezelői szolgáltatások számai |

## A * a számtartományokat jelöli.

## 3.2. Nemzetközi és belföldi előtét

## 3.2.1. Leírás

## A nemzetközi előtét tárcsázása nemzetközi számformátumú, a belföldi előtét tárcsázása belföldi számformátumú szám tárcsázását jelzi.

## 3.2.2. A használat feltételei

## Az előtétek használatát a 4. pont (Tárcsázási eljárások) írja le.

## 3.3. Segélyhívó számok

## 3.3.1. Leírás

## Háromjegyű rövid számok, amelyek segélyhívó szolgálatok (mentők, tűzoltóság, rendőrség) elérését teszik lehetővé. A segélyhívó számok hívása a hívó fél részére díjmentes.

## 3.3.2. Hívószámok

| 104 | mentők |

| 105 | tűzoltóság |

| 107 | rendőrség |

| 112 | egységes európai segélyhívószám |

## 3.3.3. A használat feltételei

## A telefonszolgáltató köteles ingyenesen biztosítani, hogy előfizetője vagy a szolgáltatás igénybe vevője elérhesse a segélyhívó szolgálatokat.

## A segélyhívások földrajzi irányítása tekintetében a telefonszolgáltató köteles egyeztetni a segélyhívó szolgálatokkal.

## 3.4. Harmonizált közérdekű szolgáltatások harmonizált számai

## 3.4.1. Leírás

## Az Európai Unió által, minden tagállam területén azonos hívószámmal bevezetésre javasolt szolgáltatások, úgynevezett harmonizált közérdekű szolgáltatások hívószámai, amelyek valamely konkrét közérdekű – az állampolgárok vagy állampolgári csoportok jólétét és biztonságát szolgáló, vagy a bajba jutott állampolgárokon segítő – szolgáltatás díjmentes elérését hivatottak lehetővé tenni.

## 3.4.2. A számok felépítése

|  |  | 116def |

| ahol: | 116 | a harmonizált közérdekű szolgáltatás elérési kódja |

|  | def | harmonizált közérdekű szolgáltatás azonosítója. |

## 3.4.3. A használat feltételei

## A harmonizált közérdekű szolgáltatások harmonizált számai használatának feltétele, hogy a szolgáltatás előzetes regisztráció nélkül bárki számára – az ország területén belül bárhonnan – elérhető legyen. A szolgáltatás időhatárokhoz nem kötött, a szolgáltatás igénybevételének nem előfeltétele fizetési kötelezettség vagy kötelezettségvállalás, a hívás díját a számhasználó fizeti. A szolgáltatás a tájékoztatás vagy segítségnyújtás, vagy az állampolgári bejelentés eszköze, vagy ezek tetszőleges kombinációja. A számon nyújtott szolgáltatás keretében reklám, szórakoztatás, továbbá áru, szolgáltatás értékesítését célzó üzletszerzési vagy tájékoztatási tevékenység nem folytatható.

## Az egyes harmonizált közérdekű szolgáltatások harmonizált számaihoz kapcsolódó – jogszabályon és az Európai Unió általános hatályú, közvetlenül alkalmazandó kötelező jogi aktusán alapuló – használati feltételeket a hatóság a honlapján teszi közzé.

## A harmonizált közérdekű szolgáltatások elérhetőségének biztosítása érdekében a 116 kezdetű számhoz rendelt szervezet felkérése esetén az elektronikus hírközlési szolgáltatót a felkéréstől számított 30 napon belül szerződéskötési kötelezettség terheli.

## Az elektronikus hírközlési szolgáltatók a hívások, illetve üzenetek költségére a rövid számhoz kijelölt szervezet részére legfeljebb az érintett szolgáltatókkal történő egyeztetést követően a hatóság által megállapított és a hatóság honlapján közzétett összeget számíthatják fel.

## 3.5. Telefontudakozó számok

## 3.5.1. Leírás

## Rövid számok, amelyek előfizetők meghatározott adatairól – az előfizető hozzájárulásától függően – felvilágosítást nyújtó tudakozó szolgáltatások elérését teszik lehetővé.

## 3.5.2. A számok felépítése

|  |  | 118de |

| ahol: | 118 | a tudakozó szolgáltatás elérési kódja |

|  | de | a tudakozó szolgáltatóját és szolgáltatását azonosítja. |

## Az egyetemes tudakozó szolgáltatások hívószámai: 11800-11809.

## 3.5.3. A használat feltételei

## Az egyetemes tudakozó szolgáltatás nyújtására egyetemes szolgáltató jogosult a 11800-11809 hívószámokon, amelyek elérhetőségét minden telefonhálózatból biztosítani kell. Az egyetemes tudakozó szolgáltatás nyújtásának feltételeit az egyetemes elektronikus hírközlési szolgáltatás nyújtásával kapcsolatos részletes szabályokról szóló NMHH rendelet tartalmazza.

## Az elektronikus hírközlési szolgáltató, illetve a számhasználó minden esetben köteles a szolgáltatás hívószámának közzétételével együtt a hívó fél által fizetendő, áfát tartalmazó díj mértékét (hívásonkénti vagy percenkénti díj, vagy az üzenetküldés díja), valamint az igénybe vehető kiegészítő szolgáltatások díját is nyilvánosságra hozni. Emellett közzé kell tenni, hogy a tudakozó mely előfizetők adataira terjed ki, terület, számtípus, illetve szolgáltatók szerint.

## 3.6. Elektronikus hírközlési szolgáltatók ügyfélszolgálati számai

## 3.6.1. Leírás

## Rövid számok, amelyek az elektronikus hírközlési szolgáltatók ügyfélszolgálatainak országos elérését teszik lehetővé.

## 3.6.2. A számok felépítése

|  |  | 12cd |

| ahol: | 12 | az elektronikus hírközlési szolgáltatók ügyfélszolgálatainak elérési kódja |

|  | cd | az elektronikus hírközlési szolgáltatót azonosítja. |

## 3.6.3. A használat feltételei

## A rövid szám olyan szolgáltató részére jelölhető ki, amelyet a hatóság elektronikus hírközlési szolgáltatás nyújtására vett nyilvántartásba.

## Az elektronikus hírközlési szolgáltató a rövid számot kizárólag az előfizetői és felhasználói bejelentések intézésére, panaszok kivizsgálására és orvoslására, az előfizetők és felhasználók tájékoztatására, az ügyfélszolgálat körébe tartozó információ nyújtására használhatja.

## 3.7. Kiegészítő szolgáltatás előtétek

## 3.7.1. Leírás

## Előtét, amely jogszabályban előírt kiegészítő szolgáltatások igénybevételét teszi lehetővé tárcsás, impulzusos nyomógombos és hangfrekvenciás hívóműves készülékről egyaránt, olyan rendszerekben, amelyekben más szabványos megoldás nem alkalmazható.

## A hívószámkijelzés hívásonkénti engedélyezése előtét alkalmazása esetén az előfizető az adott hívásra vonatkozóan feloldhatja az egyébként letiltott hívószámkijelzést. A hívószámkijelzés hívásonkénti letiltása előtét alkalmazása esetén az előfizető az adott hívásra vonatkozóan letilthatja az egyébként engedélyezett hívószámkijelzést.

## 3.7.2. Előtétek

|  | 130 | hívószám kijelzés hívásonkénti engedélyezése (KEE) |

|  | 131 | hívószám kijelzés hívásonkénti letiltása (KTE) |

## 3.7.3. A használat feltételei

## Az előtétek használatát azokban a hívószám kijelzésre kötelezett hálózatokban kell lehetővé tenni, amelyekben más szabványos megoldás nem alkalmazható.

## 3.8. Adománygyűjtő számok

## 3.8.1. Leírás

## Rövid számok, amelyek elérése a hívás, illetve üzenetküldés díjából közcélú adományok eljuttatását teszi lehetővé.

## 3.8.2. A számok felépítése

## Kiemelt adománygyűjtő számok:

|  |  | 135d, melynek értéke: |

|  | 1357 | Nemzeti Összefogás Vonala hívószáma |

|  | 135d, d ≠ 7 | kiemelt adománygyűjtő vonal hívószáma. |

## Közcélú adománygyűjtő számok:

|  |  | 136de, melynek értéke: |

|  | 13600-13609 | adománygyűjtést közvetítő szervezet hívószáma |

|  | 13610-13699 | közhasznú adománygyűjtő szervezet hívószáma. |

## 3.8.3. A használat feltételei

## A 135d kiemelt adománygyűjtő számokon közcélú adománygyűjtésre a Karitatív Tanács tagszervezetei jogosultak. A 135d rövid számok elérhetőségének biztosítása érdekében a rövid számhoz rendelt szervezet felkérése esetén az elektronikus hírközlési szolgáltatót a felkéréstől számított 30 napon belül szerződéskötési kötelezettség terheli.

## A 1357 rövid szám a „Nemzeti Összefogás Vonala”, egy kormányrendeletben kihirdetett veszélyhelyzet esetén elinduló adományvonal.

## A 13600-13609 számokon az a szervezet jogosult adományok közvetítésére közhasznú, vagy kiemelten közhasznú szervezetek felé, amellyel a hatóság által kijelölt előfizetői számok 60%-ával együttesen rendelkező hírközlési szolgáltatók megállapodást kötöttek a hívószámok elérhetőségének biztosításáról.

## A 13610-13699 számokon az a közhasznú, vagy kiemelten közhasznú szervezet jogosult adománygyűjtésre, amely legalább egy elektronikus hírközlési szolgáltatóval az adománygyűjtésről megállapodást kötött.

## A hatóság internetes honlapján közzéteszi az adománygyűjtő számokat, a számokhoz tartozó adománygyűjtő, illetve közvetítő szervezet adatait és honlapjának elérhetőségét.

## Az adománygyűjtő szervezet köteles honlapján az alábbi adatokat közzétenni:

## 1. a beérkezett hívásokból és üzenetekből származó adomány teljes összege (a)

## 2. ebből a telefonszolgáltatók részére átadott díj (b)

## 3. az adománygyűjtő szervezet által saját működési költségre felhasznált keret (a következő részletezettséggel: raktározási költség, karbantartási költség, hirdetési költség, bérköltség, bérjárulékok) (c)

## 4. a szervezet által a rászorulók megsegítésére felhasználható összeg (d) [d=a-b-c)]

## 5. adományban részesítettek száma (fő)

## 6. a gyűjtésből befolyt adomány felhasználása, a tevékenység részletes bemutatása

## Az adománygyűjtést közvetítő szervezet a honlapján köteles közzétenni az adománygyűjtő számokon belül az egyes kódokhoz tartozó adománygyűjtő szervezet adatait és honlapjának elérhetőségét, valamint köteles gondoskodni az általa közvetített adományok fenti adatainak az adománygyűjtő szervezet általi közzétételéről.

## Az elektronikus hírközlési szolgáltatók az adománygyűjtés hívásonkénti, illetve üzenetenkénti költségére legfeljebb az érintett szolgáltatókkal történő egyeztetést követően a hatóság által a 135d, illetve 136de számtartományokra megállapított és a hatóság honlapján közzétett összeget számíthatják fel. A 135d és 136de számokra az emelt díjas, díjkorlátos szolgáltatásra előírt, 2. § 3a. pont és az 1. melléklet 2.8.3. és 2.8.4. pont szerinti feltételeket kell alkalmazni. Amennyiben az előfizető az adománygyűjtő számok elérhetőségének letiltását kérte, a szolgáltatónak a letiltást díjmentesen biztosítania kell a 135d és 136de rövidszámokra.

## 3.9. Különös díjazású országos számok

## 3.9.1. Leírás

## Rövid számok, amelyek díjmentes vagy kedvezményes díjazású szolgáltatások országos elérését teszik lehetővé.

## 3.9.2. A számok felépítése

| Négyjegyű számok: | 140d, 141d, 142d, 143d, 144d |

| Ötjegyű számok: | 145de, 146de, 147de, 148de, 149de |

## 3.9.3. A használat feltételei

## A számhasználó a szolgáltatás hívószámával együtt köteles közzétenni, hogy a szám elérése a hívó számára díjmentes vagy kedvezményes díjazású.

## A kedvezményes díjazású szolgáltatások hívásdíjára az 1. melléklet 2.5.3. pontjában leírt feltételeket kell alkalmazni.

## 3.10. Közvetítő választó előtét

## 3.10.1. Leírás

## Előtét, amellyel a hívó megválaszthatja az adott híváshoz a közvetítő szolgáltatót. A közvetítő szolgáltatót azonosító előtétet hívásonkénti közvetítő választás esetén a hívó tárcsázza a hívás során, közvetítő előválasztás esetén a közvetítő szolgáltatót azonosító kódot az előfizetői hozzáférést nyújtó szolgáltató illeszti be a hívásfelépítést kezdeményező jelzésüzenetbe.

## 3.10.2. A számok felépítése

|  |  | 15cd |

| ahol: | 15 | a közvetítő választás elérési kódja, |

|  | cd | a közvetítő szolgáltatót azonosítja. |

## 3.10.3. A használat feltételei

## A közvetítő választó előtét használatának feltételeit az elektronikus hírközlési szolgáltatás igénybevétele során alkalmazható közvetítőválasztásról szóló külön jogszabály rögzíti.

## 3.11. Elektronikus hírközlési szolgáltató hálózatához rendelt számok

## 3.11.1. Leírás

## A szolgáltató hálózatán belül elérhető szolgáltatások hívószámai.

## A hívószámok nem harmonizáltak, az egyes szolgáltatóknál eltérő szolgáltatásokra alkalmazhatók.

## 3.11.2. A számok felépítése

| Három-, négy- vagy ötjegyű számok: | 17c |

|  | 17cd |

|  | 17cde |

## 3.11.3. A használat feltételei

## A 17c(d)(e) formátumú számokon a szolgáltató saját hálózatában saját előfizetői részére nyújtott szolgáltatásai érhetők el. A szolgáltatás más szolgáltató hálózatából csak abban az esetben érhető el, ha az adott szolgáltató jogosult ugyanazon rövid szám használatára ugyanannak a szolgáltatásnak az eléréséhez.

## A számokon emelt díjas szolgáltatás nem nyújtható. Kedvezményes díjazású szolgáltatás csak a 2. § 2. pontjában és az 1. melléklet 2.5.3. pontjában előírt feltételek szerint nyújtható.

## 3.12. Közérdekű tájékoztató és támogató szolgáltatások számai

## 3.12.1. Leírás

## Közérdekű szolgáltatások országos elérését lehetővé tevő rövid számok.

## 3.12.2. A számok felépítése

## Az egyes szolgáltatásokat három- vagy négyjegyű számok azonosítják:

| Háromjegyű számok: | 180, 185, 186, 187, 188, 189 |

| Négyjegyű számok: | 181d, 182d, 183d, 184d |

## 3.12.3. A használat feltételei

## A számokon valamely nagyobb közösség, vagy az egész társadalom érdekét szolgáló támogató vagy tájékoztató jellegű szolgáltatások nyújthatók.

## A hatóság internetes honlapján folyamatosan közzéteszi a kijelölhető számokat és a számokon elérhető szolgáltatásokat. Az országosan harmonizált számokhoz rendelt közérdekű támogató és tájékoztató szolgáltatások bevezetése nem kötelező, de alkalmazásuk esetén a közzétett számok csak a megadott szolgáltatáshoz használhatók.

## A számokon emelt díjas szolgáltatás nem nyújtható. A szolgáltató minden esetben köteles a szolgáltatás hívószámának közzétételével együtt a hívó fél által fizetendő, áfát tartalmazó díj mértékét is (hívásonkénti vagy percenkénti díj, vagy az üzenetküldés díja) nyilvánosságra hozni.

## 3.13. Telefonos kezelői szolgáltatások számai

## 3.13.1. Leírás

## A hagyományos kezelői szolgáltatásoknak a szolgáltató hálózatából történő elérését lehetővé tevő harmonizált rövid számok.

## 3.13.2. Számok

| 192 | táviratfeladás |

| 193 | kezelői ébresztés |

## 3.13.3. A használat feltételei

## A 19c formátumú számokon nyújtott szolgáltatások kizárólag a szolgáltató hálózatában, saját előfizetői által érhetők el. A szolgáltatás más szolgáltató hálózatából csak abban az esetben érhető el, ha az adott szolgáltató jogosult ugyanazon rövid szám használatára.

## A 19c formátumú országosan harmonizált számhoz rendelt szolgáltatás bevezetése nem kötelező, de alkalmazása esetén a fent felsorolt számok csak a megadott szolgáltatásokhoz használhatók.

## A hívó fél által fizetendő díj mértékét (áfát is tartalmazó hívásonkénti vagy percenkénti díj) a szolgáltatónak minden esetben a szolgáltatás számának közzétételével együtt nyilvánosságra kell hoznia.

## 3.14. Lelki segítő és támogató szolgáltatás számok

## 3.14.1. Leírás

## Rövid számok, amelyek telefonos lelki segítséget és támogatást nyújtó szervezetek díjmentes elérését teszik lehetővé.

## 3.14.2. A számok felépítése

|  |  | 137de |

| ahol: | 137 | a lelki segítő és támogató szolgáltatások elérési kódja |

|  | de | a támogató szervezetet és szolgáltatást azonosítja. |

## 3.14.3. A használat feltételei

## A 137de formátumú számokon a számhoz hozzárendelt, a hatóság honlapján, valamint az egyesülési jogról, a közhasznú jogállásról, valamint a civil szervezetek működéséről és támogatásáról szóló törvény által létrehozott Civil Információs Portálon közzétett, működő státuszú lelki segítő és támogató szolgáltatást nyújtó szervezetek nyújtanak telefonos támogatást, biztosítva a hívók névtelenségét. A szolgáltatás igénybevétele a hívók részére díjmentes, a szolgáltatás díját a hívott szervezet fizeti.

## Az elektronikus hírközlési szolgáltatók a hívások, illetve üzenetek költségére a rövid számhoz hozzárendelt szervezet részére legfeljebb – az érintett szolgáltatókkal történő egyeztetést követően – a hatóság által megállapított és a hatóság honlapján közzétett összeget számíthatják fel.

## 3.15. Emelt díjas szolgáltatás rövid számok

## 3.15.1. Leírás

## Rövid számok, melyek a beszédcélú elektronikus hírközlő hálózatból adott számhasználó meghatározott emelt díjas szolgáltatásának elérését teszik lehetővé. A szolgáltatás igénybevételi díja és tartalma szerint a számokon emelt díjas, díjkorlátos szolgáltatás vagy emelt díjas, díjkorlátmentes szolgáltatás vagy emelt díjas felnőtt szolgáltatás nyújtható.

## 3.15.2. A számok felépítése

| Emelt díjas, díjkorlátos szolgáltatás: | 160de, 161def |

| Emelt díjas, díjkorlátmentes szolgáltatás: | 164de, 165def |

| Emelt díjas felnőtt szolgáltatás: | 168de, 169def |

## 3.15.3. A használat feltételei

## A 16cde(f) számok az 1. melléklet 2.8.4. pontjában meghatározott általános számhasználati feltételekkel használhatók.

## A 160de és 161def számokon a szolgáltató a hívó fél által fizetendő legmagasabb díjat úgy köteles meghatározni, hogy az ne haladja meg a hatóság által az érintett szolgáltatókkal történő egyeztetést követően – évente január 31-ig – a hatóság internetes honlapján közzétett díjat.

## A 160de, 161def, 164de és 165def számokon nem nyújtható felnőtt tartalom.

## A 168de és 169def számokra vonatkozóan a szolgáltató minden kiskorú előfizetőjénél díjmentesen alapértelmezett tiltást köteles berendezni. Ez a korlátozás kiskorú előfizető esetében még törvényes képviselőjének kérésére sem oldható fel.

## A szolgáltatás tartalmára vonatkozó feltételek betartásáért a számhasználó felel.

## 4. TÁRCSÁZÁSI ELJÁRÁSOK

## A tárcsázási eljárások meghatározzák, hogy a beszédcélú elektronikus hírközlő hálózatok számozási tervében, azaz e melléklet 1–3. pontjában meghatározott azonosítók milyen sorrendben, milyen eljárással alkalmazhatók hívásfelépítés és üzenetküldés kezdeményezésére a számozási tervben meghatározott előfizetők és szolgáltatások felé.

## A tárcsázási eljárásokban a belföldi előtét (BE) és a nemzetközi előtét (NE) a belföldi és a nemzetközi számformátumot jelzik, a közvetítő választó előtét (KVE) az adott híváshoz tartozó közvetítő szolgáltató választását jelzi.

## A hívószám kijelzést hívásonként engedélyező előtét (KEE) és a hívószám kijelzést hívásonként letiltó előtét (KTE) használatával az adott hívásra megváltoztatható a hívószám kijelzési beállítás.

## Az előtét nem része a hívószámnak. Egy híváson belül több előtét is alkalmazható.

## Mobil rádiótelefon hálózatokban a nemzetközi előtét (NE) helyett megengedett a + karakter használata is.

## A beszédcélú elektronikus hírközlő hálózatokban hívás és üzenetküldés kezdeményezésére a számjegyeken és a + karakteren kívül más karakter nem használható.

## 4.1. Nemzetközi számok hívása

## A tárcsázási folyamat:

## (KVE) – NE – nemzetközi szám

## 4.2. Belföldi számok hívása

## A tárcsázási folyamat:

## (KVE)–BE-belföldi szám

## vagy

## (KVE)–NE-36-belföldi szám

## Megengedett a földrajzi számozási területen belüli, azonos körzetszámmal rendelkező előfizetői hozzáférési pontok közötti hívás esetén az előfizetői szám formátumú tárcsázás is:

## (KVE) – ES

## 4.3. Rövid számok hívása

## A rövid számok (RS) csak közvetlen formában hívhatók, előtét (BE, NE), vagy belföldi rendeltetési szám (KS vagy SHS) után nem:

## RS

## 4.4. Hívószám kijelzés előtétek

## A KEE vagy a KTE előtétet a tárcsázási folyamat elején kell tárcsázni.

2. melléklet a 3/2011. (IX. 26.) NMHH rendelethez[^16]

[^16]: A 2. melléklet az 1/2012. (I. 3.) NMHH rendelet 8. § (5) bekezdésével megállapított szöveg.
