7. § (1) A központi szerver és a helyhez kötött szerver alapú pénznyerő automata, illetve a nem helyhez kötött szerver alapú pénznyerő rendszer közötti biztonságos kommunikáció érdekében a használt protokollnak titkosítással, hibaérzékelő és helyreállító mechanizmusokkal kell rendelkeznie, ami a manipulálás elleni kellő védettséget biztosít. A kapcsolat megszakadása és újrafelvétele nem járhat adatvesztéssel.

(2) A központi szerver és a helyhez kötött szerver alapú pénznyerő automata, illetve a nem helyhez kötött szerver alapú pénznyerő rendszer közötti hálózati kapcsolat bármilyen okból (pl. áramszünet miatt) történő megszakadását követően a helyhez kötött szerver alapú pénznyerő automatának, illetve a nem helyhez kötött szerver alapú pénznyerő rendszernek biztosítania kell a játékos és a szerencsejáték szervező közötti elszámolás lehetőségét.

(3) A kommunikációs hálózatnak biztonságosan össze kell kapcsolnia a központi szervert és a helyhez kötött szerver alapú pénznyerő automatát, illetve a nem helyhez kötött szerver alapú pénznyerő rendszert úgy, hogy a központi szerver által biztosított játékprogramot csak engedélyezett helyhez kötött szerver alapú pénznyerő automata, illetve a nem helyhez kötött szerver alapú pénznyerő rendszer használhassa. A központi szerver és a helyhez kötött szerver alapú pénznyerő automata, illetve a nem helyhez kötött szerver alapú pénznyerő rendszer közötti kommunikációba nem építhető be semmilyen a játéklogika befolyásolására képes entitás (különösen lokális szerver és proxy szerver).

(4) A központi szerverhez való minden csatlakozásnak megfelelő tűzfalat kell tartalmaznia. A tűzfal alkalmazásnak eseménynaplót kell vezetnie és az eseménynapló megtelése esetén le kell tiltania minden kommunikációt, és hibaeseményt kell generálnia.

(5) Az állami adóhatóság kivételével távoli hozzáférés kizárólag a központi szerver játékszerver részével valósítható meg olyan módszerrel, amely biztonságos, minősített hardver egységben tárolt kulcs segítségével, zárt csatornán összekapcsolja a rendszert és a hozzáférést kérőt. Ennek a biztonságos kapcsolatnak egyedileg be kell azonosítania a hozzáférést kérő távoli felhasználót és annak munkaállomását. A távoli hozzáférés számára egyetlen rendszeradminisztrátori funkció sem engedélyezett, így különösen távoli hozzáféréssel nem adható jogosultság az alábbiakra:

a) új felhasználó hozzáadása,

b) műszaki egység csatlakoztatása, vagy leválasztása,

c) hozzáférési jogosultságok megváltoztatása,

d) rendszerprogramok telepítése, módosítása, törlése,

e) fájlok törlése vagy felülírása, a vírusvédelmi frissítések kivételével.

(6) A távoli hozzáférésről a szervernek automatikus, megváltoztathatatlan eseménynaplót kell vezetnie, amely leírja az összes távoli hozzáférési információt, így különösen a belépési azonosítót, dátumot és időpontot, a végzett tevékenységet és a kapcsolat időtartamát. Ha jogosulatlan hozzáférési kísérlet érkezik, a szerver működtetőjét értesítenie kell a rendszernek.

(7) Az 1. mellékletben megjelölt adatokat a központi szerver üzemeltetőjének átlátható, elemezhető, a változásokat nyomon követhető formátumban kell biztosítania.
