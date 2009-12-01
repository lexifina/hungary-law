## I. rész

## Nemzeti Jövedéki Informatikai Rendszer alrendszerei és az abban rögzített adatállomány

## A Nemzeti Jövedéki Informatikai Rendszer az alábbi modulokból épül fel:

## – Jövedéki engedélyezési alrendszer,

## – Jövedéki adó alrendszer,

## – Jövedéki ellenőrzési alrendszer,

## – Adó- és Zárjegy alrendszer,

## – Üzemeltetési alrendszer,

## – Országos alrendszer.

## A gazdálkodók cégadatai és magánszemélyek személyes adatai, valamint a telephelyekre és székhelyekre vonatkozó adatok a Nemzeti Jövedéki Informatikai Rendszerben nem kerülnek rögzítésre, ezen adatok kezelése kizárólag a GTR rendszerben történik. A Nemzeti Jövedéki Informatikai Rendszer a fenti adatokra kizárólag a VPID számmal hivatkozik.

## Valamennyi alrendszer egy közös iktató modullal rendelkezik, melyben az alábbi adatok kerülnek tárolásra:

## – VPID szám (kapcsolata a GTR rendszerrel);

## – Ügyintéző adatai;

## – Ügyiratra vonatkozó adatok (iktatószám, iktatás napja, beérkezés napja, postára feladás napja, ügyirat kelte, ügydöntés jelölése);

## – Az egyes ügyiratokhoz kapcsolódó dátumok és időszakok (pl. adóbevallási, adó-visszaigénylési, nyilvántartás zárási időszaka).

## 1. Jövedéki engedélyezési alrendszer:

## Az engedélyhez kötött jövedéki tevékenységek végzéséhez benyújtott kérelmek feldolgozására szolgáló modul, melyben az alábbi adatok kerülnek rögzítésre:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – a kérelemhez benyújtott nyilatkozatok adatai;

## – jövedéki biztosítékra vonatkozó adatok;

## – az engedélyezett telephely(ek) adatai és a telephelyengedély típusára vonatkozó adatok;

## – tárolótartályok adatai;

## – a tevékenység során előállításra, tárolásra, felhasználásra kerülő jövedéki termék(ek) adatai;

## – szőlőültetvények adatai;

## – az egyes telephelyek első számú vezetőjének, felelős üzemvezetőjének, jövedéki ügyintézőjének, valamint TKO/EKO/BKO okmányok aláírására jogosult személyek személyes adatai.

## 2. SEED adatok:

## Az Európai Unió által meghatározott adóraktári és bejegyzett kereskedői engedélyesek adatait tartalmazó modul, melybe a Nemzeti Jövedéki Informatikai Rendszerben rögzített engedélyesek, valamint a tagállamok által megküldött engedélyes adatok kerülnek tárolásra.

## 3. Jövedéki adó alrendszer:

## Az adóbevallások, adókivetések és visszatérítések feldolgozására szolgáló programmodul, melyben az alábbi adatok kerülnek rögzítésre:

## Adóbevallások:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – a bevallásra vonatkozó különböző időszakok és dátumok (pl. beérkezés kelte, bevallási időszak, esedékesség kelte stb.);

## – adófizetésre vonatkozó adatok jövedéki fajtakódonként;

## – adó visszatérítésre vonatkozó adatok jövedéki fajtakódonként és visszaigénylési jogcímenként;

## – köztartozásokra vonatkozó adatok.

## Adókivetés:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – határozat adatok;

## – adókivetés jogcíme, indoklása;

## – engedélyszám;

## – adókivetés alapjául szolgáló termék vámtarifaszáma, mennyisége;

## – fajtakód;

## – időszaknak megfelelő adómérték;

## – kiszabásra kerülő jövedéki adó;

## – ÁFA.

## Visszatérítés:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – visszaigénylési alapadatok (a terület nagyság, a visszaigénylés jogcíme, a visszaigénylés éve, a visszaigénylés alapjául szolgáló termék mennyisége, fajtakód, adómérték, önellenőrzési pótlék);

## – beszerzési bizonylatok, számlák adatai (számlaszám, számlakibocsátó adószáma, beszerzés dátuma, számla kelte, fajtakód, számla összege);

## – belső-, felhasználási bizonylatok (felhasznált termék megnevezése, mennyisége, felhasználási időpontja, bizonylatszám);

## – köztartozásokra vonatkozó adatok;

## – csatolt igazolások, szakhatósági engedélyek száma.

## 4. Jövedéki ellenőrzési alrendszer:

## Nyilvántartások:

## Az engedélyes alanyok részére a nyilvántartásaikkal kapcsolatosan a törvényben meghatározott adatszolgáltatások adatainak feldolgozása szolgáló programrész, melyben az alábbi adatok kerülnek rögzítésre:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – az előállított, beszerzett, értékesített jövedéki termékek mennyiségére és a termékek mozgásának jogcímére vonatkozó adatok;

## – adófizetéssel járó mozgások esetén a fizetendő jövedéki adó és ÁFA összege.

## Készletfelvételi jegyzőkönyvek:

## Az adóraktáraknál, valamint az üzemanyagtöltő állomásokon végzett készletfelvételekről készült jegyzőkönyvek adatainak rögzítésére szolgáló programrész, melyben az alábbi adatok kerülnek tárolásra:

## – jegyzőkönyv iktatószáma;

## – a készletfelvétel időpontja;

## – az engedélyes adatai (a GTR rendszerből kerül átvételre);

## – vizsgált időszak;

## – adóraktárak esetében a tárgyidőszakban előállított, felhasznált, vásárolt és értékesített jövedéki termék mennyisége;

## – üzemanyagtöltő állomások esetében a tárgyidőszakban beszerzett és értékesített, valamint a készletezett üzemanyagok mennyiségi adatai.

## Szőlőbor elszámolás:

## Az egyszerűsített adóraktárak által benyújtott szőlőbor elszámolások rögzítésére szolgáló programrész, melyben az alábbi adatok kerülnek tárolásra:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – megtermelt, vásárolt és feldolgozott szőlő és must mennyisége;

## – az előállításra került szőlőbor mennyisége és a szőlőbor készlet csökkenésének mértéke jogcímenként;

## – a vásárolt és értékesített szőlő mennyiségének ellenőrzéséhez szükséges, a vevőre és eladóra vonatkozó adatok (bizonylatszám, adószám, adóazonosító, Sze. Ig./ út.szám, eladó neve, mennyiség);

## – melléktermékek adatai;

## – veszteség adatok.

## Szeszüzemi nyilvántartás és elszámolás:

## A bérfőzést és kereskedelmi főzést végző engedélyesek egyes adatai és az alanyoknál végzett elszámolások alábbi adatai kerülnek rögzítésre:

## – a telephelyen található szeszüzemi berendezések adatai, felelős üzemvezető személyes adatai (nem a GTR rendszerben kerül tárolásra);

## – az elszámolásokkal és váratlan ellenőrzésekkel és a szeszüzemi üzemakadályokkal kapcsolatos adatok (iktatószám, időszak, elszámolást végző személyek (név, nyilvántartási szám, rendfokozat);

## – feldolgozott alapanyag fajtája és mennyisége;

## – előállításra és a főzetőknek kiadásra került pálinka fajtája és mennyisége;

## – a fizetendő bérfőzési szeszadó összege;

## – befizetett bérfőzési szeszadó dátuma és összege;

## – a kiadásra került pálinka mennyiségének és a főzetők ellenőrzése érdekében a főzetők személyes adatai (nem a GTR rendszerben kerülnek tárolásra), származási igazolvány száma, kiadott pálinka mennyisége.

## Jogsértés – Fizetéskönnyítés – Végrehajtás

## A Vám- és Pénzügyőrség szervei által lefolytatott ellenőrzési jegyzőkönyvek és a feltárt jogsértések adatainak feldolgozására, valamint az ezekhez kapcsolódó bírság határozatok, jogorvoslati eljárások, fizetési könnyítések és végrehajtási eljárások adatainak rögzítésére szolgáló programrész, melyben az alábbi adatok kerülnek tárolásra:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – az ellenőrzés helyszínére és az ellenőrzést végző személyekre, valamint a feltárt jogsértésre vonatkozó adatok;

## – a jogsértést elbíráló határozat adatai (jogszabályi hivatkozás, bírság és adók összege, határidők);

## – esetleges fizetési könnyítést engedélyező határozat adatai;

## – a jogorvoslati eljárások során hozott II. fokú határozatok, valamint bírósági végzések adatai;

## – lefoglalásra és elkobzásra, valamint megsemmisítésre/értékesítésre került termékek adatai;

## – a végrehajtási eljárások során foganatosított inkasszó és APEH részére történő átadások adatai.

## Illeték:

## Az egyes eljárások során fizetendő illetékek kiszabására és kezelésére szolgáló programrész, melyben az alábbi adatok kerülnek rögzítésre:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – illeték összege.

## Kiskereskedők:

## A polgármesteri hivatalok jegyzői által megküldött működési engedélyek adatainak rögzítésére szolgáló programrész, melyben az alábbi adatok kerülnek tárolásra:

## – működési engedély száma;

## – adószám;

## – gazdálkodó neve, telephely címe;

## – engedélyező önkormányzat;

## – forgalmazott termékek;

## – érvényesség kezdete, vége.

## 5. Adó-, Zárjegy alrendszer:

## Az adó- és zárjegy megrendelések feldolgozására és azok teljesítésére vonatkozó adatok, valamint az adó- és zárjegy raktárkészlet kezelésére szolgáló modul, melyben az alábbi adatok kerülnek tárolásra:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – dátum adatok (a megrendelés és az átvétel időpontja);

## – folyószámla adatok;

## – nyilvántartási adatok (raktározási azonosító, táskaszám);

## – készlet mennyiségi adatok;

## – törzsadatok (fajtakód, cikktörzs);

## – szállítólevél és számla adatok.

## 6. Üzemeltetés alrendszer:

## A Nemzeti Jövedéki Informatikai Rendszert használó szervek törzsadatainak és az egyes szervek felhasználóinak jogosultsági adatainak rögzítésére és karbantartására szolgáló alrendszer, melyben az alábbi adatok kerülnek tárolásra:

## – a vámszervek név, cím, elérhetőségi és nyitvatartási adatai;

## – a rendszer használatára jogosult felhasználók neve, rendfokozata, beosztása és az egyes alrendszerekhez meghatározott jogosultsági szintjeik.

## Az üzemeltetés alrendszerben kerül továbbá a Közvetlen Elektronikus Adatkapcsolati rendszeren keresztül az engedélyes alanyok által elektronikusan teljesített adatszolgáltatások fogadása és feldolgozásra előkészítése.

## 7. Országos alrendszer:

## Kizárólag a Nemzeti Jövedéki Informatikai Rendszer egyes alrendszereiben rögzített adatok különböző szempontú lekérdezésére szolgáló alrendszer.

## Mindemellett a következő adatok rögzítésére is ez az alrendszer szolgál:

## – visszautalásokkal kapcsolatban a testület számára keletkezett késedelmi pótlék fizetési kötelezettségek rögzítése (VPID szám (GTR adataira hivatkozás), hivatkozott azonosító, fizetési határidő és mód);

## – kontrollszám hibás előírások feldolgozása.

## 8. Adóellenőrzés alrendszer

## Az alrendszer tartalmazza az adóellenőrzés lefolytatása során keletkező alábbi vizsgálati adatokat:

## – az iktatószámmal és VPID számmal hivatkozás az iktató modul és a GTR rendszer adataira;

## – a bevallásra vonatkozó különböző időszakok és dátumok (pl. beérkezés kelte, bevallási időszak, esedékesség kelte stb.);

## – adófizetésre vonatkozó adatok jövedéki fajtakódonként;

## – adó visszatérítésre vonatkozó adatok jövedéki fajtakódonként és visszaigénylési jogcímenként;

## – köztartozásokra vonatkozó adatok;

## – a gazdálkodó nyilvántartásaiból, illetve az ellenőrzés során az ellenőrzéshez felhasznált adatok.

## 9. E-Jövedék alrendszer

## Az elektronikus kormányzati rendszer keretében, az Ügyfélkapun megküldött ügyféli elektronikus bevallások, és egyéb adatszolgáltatásokkal kapcsolatos feldolgozáshoz szükséges adatokat.

## 10. Mobil Ellenőrzés alrendszer

## Az Adó- és Zárjegy alrendszer, valamint a Jövedéki ellenőrzési alrendszerben nyilvántartott adatok felhasználásával, a jövedéki helyszíni ellenőrzés során jegyzőkönyvben rögzített megállapításokat és az ahhoz kapcsolódó ellenőrzési adatokat, melyek megegyeznek a Jövedéki ellenőrzési alrendszer jogsértés részében rögzített adatokkal.

## II. rész

## A Nemzeti Jövedéki Informatikai rendszert kezelő szervek és a hozzáférési jogosultságok

| Szolgálati hely | Felhasználó beosztása | Adható hozzáférési jogosultságok |

| Rögzítés | Lekérdezés |

| Vám- és Pénzügyőrség Országos Parancsnoksága | Országos parancsnok |  | x |

| Országos parancsnok helyettes |  | x |

|  | Vámigazgatási tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének vezetője, vezetőjének helyettese |  | x |

|  | Jövedéki igazgatási tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének vezetője, vezetőjének helyettese |  | x |

|  | Bűnüldözési tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének vezetője, vezetőjének helyettese |  | x |

|  | Felderítés-felügyeleti és bűnmegelőzési tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének a vezetője, vezetőjének helyettese, osztályvezetője, és a vezetője által kijelölt tagjai |  | x |

|  | Ellenőrzési tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének valamennyi tagja |  | x |

|  | Vámigazgatási tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének vezetője által kijelölt tagjai |  | x |

|  | Jövedéki igazgatási tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének vezetője által kijelölt, illetőleg elemzéssel foglalkozó tagjai |  | x |

|  | Informatikai tevékenységet irányító, felügyelő, ellenőrző szervezeti egységének vezetője által kijelölt tagjai |  | x |

|  | Más szervezeti egység vezetője és az általa kijelölt illetőleg elemzéssel foglalkozó tagjai |  | x |

| Vám- és Pénzügyőrség Központi Bűnüldözési Parancsnoksága és a Vám- és Pénzügyőrség Regionális Nyomozó Hivatalai | Parancsnok és a parancsnok által kijelölt tagjai |  | x |

| Vám- és Pénzügyőrség Bűnügyi Ellátó Nyomozó Hivatala | Parancsnok és a parancsnok által kijelölt tagjai |  | x |

| Vám- és Pénzügyőrség Központi Járőrszolgálat Parancsnoksága | Parancsnok és a parancsnok által kijelölt tagjai | x | x |

| Vám- és Pénzügyőrség Központi Ellenőrzési Parancsnoksága | Parancsnok és a parancsnok által kijelölt, illetve elemzéssel foglalkozó tagjai | x | x |

| Vám- és Pénzügyőrség Számlavezető Parancsnoksága Parancsnok és a parancsnok által kijelölt tagjai | Parancsnok és a parancsnok által kijelölt tagjai | x | x |

| Vám- és Pénzügyőrség Regionális Parancsnokságai | Parancsnok és a parancsnok által kijelölt tagjai | x | x |

| Vám- és Pénzügyőri Hivatalok/Megyeszékhelyen működő Vám- és Pénzügyőri Hivatalok | Parancsnok és a parancsnok által kijelölt tagjai | x | x |

| Regionális Ellenőrzési Központok | Parancsnok és a parancsnok által kijelölt tagjai | x | x |

| Vám- és Pénzügyőrség rendszerfejlesztésért felelős szerve | Parancsnok és a parancsnok által kijelölt tagjai |  | x |

4. számú melléklet a 34/2004. (VI. 23.) PM rendelethez[^10]

[^10]: A 4. számú melléklet a 28/2009. (XI. 30.) PM rendelet 13. § (6) bekezdésével megállapított szöveg.
