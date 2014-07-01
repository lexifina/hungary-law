## A közfeladatot ellátó szerveknél alkalmazható iratkezelési szoftverek által kezelendő küldemény

## és érkeztető könyvi metaadatok

## 1. KÜLDEMÉNY METAADATOK

|  | A | B | C | D |

|  | Megnevezés | Mező típusa | Mező felépítése, korlátozások | Megjegyzés |

| 1 | Beérkezés időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Elektronikus érkeztetés esetén a dátum és idő adat. Manuális érkeztetés esetén a beérkezés tényleges dátuma. |

| 2 | Érkeztetés időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Elektronikus érkeztetés esetén a dátum és idő adat. Manuális érkeztetés esetén a beérkezés tényleges dátuma. |

| 3 | Kézbesítés módja | Szövegmező | Maximum 25 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv által karbantartott és bővíthető listából választható, alapértékei: posta, futár, személyes benyújtás, e-mail/fax, e-ügyintézés, SZEÜSZ szolgáltatás. |

| 4 | Beérkezés módja | Szövegmező | Maximum 25 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv által karbantartott és bővíthető listából választható, alapértékei: elsőbbségi, ajánlott, tértivevény, értékküldemény, csomag vagy SZEÜSZ szolgáltatás. |

| 5 | Kézbesítés prioritása | Szövegmező | Maximum 15 karakter | A szerv által karbantartott és bővíthető listából választható, alapértékei: normál, sürgős, azonnal. |

| 6 | Érkeztető | Szövegmező | Maximum 50 karakter | A szerv által karbantartott címtárból választható természetes személyre vagy szervezeti egységre vonatkozó adat vagy automatizmus által rögzített adat. |

| 7 | Érkeztetési azonosító | Betűt és számot egyaránt tartalmazó mező | Maximum 30 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító vagy SZEÜSZ szolgáltatás esetén a szolgáltatás által alkalmazott azonosító. |

| 8 | Érkeztető munkaállomás / szerver azonosítója | Betűt és/vagy számot tartalmazó, illetve speciális karakter | Maximum 30 karakter | Hálózati név / IP cím / gép név / szerver azonosító |

| 9 | Postai azonosító | Betűt és számot egyaránt tartalmazó mező | Maximum 20 karakter | A könyvelt postai küldemény ragszáma. |

| 10 | Küldő / feladó neve | Szövegmező | Maximum 150 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | Természetes vagy jogi személy. A szerv által karbantartott címtárból választható adat, vagy egyedi adatbevitel, vagy SZEÜSZ szolgáltatás által biztosított adat. |

| 11 | Küldő / feladó címe | Betűt és számot egyaránt tartalmazó mező | Felépítése a polgárok személyi adatainak és lakcímének nyilvántartásáról szóló 1992. évi LXVI. törvény végrehajtásáról szóló 146/1993. (X. 26.) Korm. rendelet 15. § (5)–(6) bekezdése, vagy a cégbejegyzési eljárás és a cégnyilvántartás egyes kérdéseiről szóló 21/2006. (V. 18.) IM rendelet 1. számú mellékletében meghatározott formanyomtatvány adattartalma szerinti, vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv által karbantartott címtárból választható adat, vagy egyedi adatbevitel, vagy SZEÜSZ szolgáltatás által biztosított adat. |

| 12 | Küldő e-mail címe | Formátumnak megfelelő | Felhasználó_név@gépnév.domain_név.aldomain_név.országazonosító Maximum 50 karakter |  |

| 13 | Elektronikus aláírás érvényessége | Logikai mező | Választható értéke: Igen / Nem |  |

| 14 | Elektronikus aláírás lejárati dátuma | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Az az időpont, amíg az elektronikus aláírás ellenőrizhető és érvényes. |

| 15 | Elektronikus aláírás hitelesítés-szolgáltató neve | Betűt és számot egyaránt tartalmazó mező | Maximum 50 karakter | Elektronikus aláírást szolgáltató szervezet neve. |

| 16 | Címzett neve | Szövegmező | Maximum 150 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | Természetes vagy jogi személy. A szerv által karbantartott címtárból választható adat, vagy egyedi adatbevitel, vagy SZEÜSZ szolgáltatás által biztosított adat. |

| 17 | Címzett címe | Betűt és számot egyaránt tartalmazó mező | Felépítése a polgárok személyi adatainak és lakcímének nyilvántartásáról szóló 1992. évi LXVI. törvény végrehajtásáról szóló 146/1993. (X. 26.) Korm. rendelet 15. § (5)–(6) bekezdése, vagy a cégbejegyzési eljárás és a cégnyilvántartás egyes kérdéseiről szóló 21/2006. (V. 18.) IM rendelet 1. számú mellékletében meghatározott formanyomtatvány adattartalma szerinti, vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv által karbantartott címtárból választható adat, vagy egyedi adatbevitel, vagy SZEÜSZ szolgáltatás által biztosított adat. |

| 18 | Küldemény bontója | Szövegmező | Maximum 50 karakter vagy a SZEÜSZ szolgáltatás által rögzített adat. | A szerv által karbantartott címtárból választható természetes személyre vagy szervezeti egységre vonatkozó adat vagy a SZEÜSZ szolgáltatás által rögzített adat. |

| 19 | Címzés típusa | Szövegmező | Maximum 25 karakter | A szerv által karbantartott és bővíthető listából választható, alapértékei: névre szóló, saját kezű felbontásra. |

| 20 | Küldemény típusa | Szövegmező | Maximum 35 karakter vagy a SZEÜSZ szolgáltatás megnevezése. | A szerv által karbantartott és bővíthető listából választható, alapértékei: papír alapú, elektronikus formában benyújtott, SZEÜSZ szolgáltatás. |

| 21 | Küldemény elemeinek száma | Számmező (pozitív egész szám) | Maximum 3 karakter | Küldemény elkülöníthető elemeinek száma. |

| 22 | Mellékletek száma | Számmező (pozitív egész szám) | Maximum 3 karakter | Egy adott küldemény elemhez tartozó mellékletek száma. |

| 23 | Mellékletek (adathordozó) típusa | Szövegmező | Maximum 20 karakter | A szerv által karbantartott és bővíthető listából választható, alapértékei: papír alapú, elektronikus formában benyújtott. |

| 24 | Mellékletek (adathordozó) fajtája | Szövegmező | Maximum 30 karakter | A szerv által karbantartott és bővíthető listából választható, alapértékei: papír vagy elektronikus (CD, DVD, pendrive). |

| 25 | Bontás időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | A bontás időpontja megegyezhet az érkeztetés időpontjával. |

| 26 | Sérült küldemény | Logikai mező | Választható értéke: Igen / Nem |  |

| 27 | Téves címzés | Logikai mező | Választható értéke: Igen / Nem |  |

| 28 | Téves érkeztetés | Logikai mező | Választható értéke: Igen / Nem |  |

| 29 | Iktatást nem igényel | Logikai mező | Választható értéke: Igen / Nem |  |

| 30 | Hivatkozási szám | Betűt és számot egyaránt tartalmazó mező | Maximum 50 karakter vagy SZEÜSZ szolgáltatás esetén a szolgáltatás által alkalmazott azonosító. | A küldő által jelzett iktatószám vagy SZEÜSZ szolgáltatás esetén a szolgáltatás által alkalmazott azonosító. |

## 2. ÉRKEZTETŐ KÖNYVI METAADATOK

|  | A | B | C | D |

|  | Megnevezés | Mező típusa | Mező felépítése, korlátozások | Megjegyzés |

| 1 | Beérkezés időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Elektronikus érkeztetés esetén a dátum és idő adat. Manuális érkeztetés esetén a beérkezés tényleges dátuma. |

| 2 | Érkeztetési azonosító | Betűt és számot egyaránt tartalmazó mező | Maximum 30 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító vagy SZEÜSZ szolgáltatás esetén a szolgáltatás által alkalmazott azonosító. |

| 3 | Postai azonosító | Betűt és számot egyaránt tartalmazó mező | Maximum 20 karakter | A könyvelt postai küldemény ragszáma. |

| 4 | Küldő / feladó neve | Szövegmező | Maximum 150 karakter vagy a SZEÜSZ szolgáltatás által biztosított adat. | Természetes vagy jogi személy. A szerv által karbantartott címtárból választható adat, vagy egyedi adatbevitel, vagy SZEÜSZ szolgáltatás által biztosított adat. |

| 5 | Küldő / feladó címe | Betűt és számot egyaránt tartalmazó mező | Felépítése a polgárok személyi adatainak és lakcímének nyilvántartásáról szóló 1992. évi LXVI. törvény végrehajtásáról szóló 146/1993. (X. 26.) Korm. rendelet 15. § (5)–(6) bekezdése, vagy a cégbejegyzési eljárás és a cégnyilvántartás egyes kérdéseiről szóló 21/2006. (V. 18.) IM rendelet 1. számú mellékletében meghatározott formanyomtatvány adattartalma szerinti, vagy a SZEÜSZ szolgáltatás által biztosított adat. | A szerv által karbantartott címtárból választható adat, vagy egyedi adatbevitel, vagy SZEÜSZ szolgáltatás által biztosított adat. |

| 6 | Küldő e-mail címe | Formátumnak megfelelő | Felhasználó_név@gépnév.domain_név.aldomain_név.országazonosító Maximum 50 karakter |  |

| 7 | Érkeztető | Szövegmező | Maximum 50 karakter | A szerv által karbantartott címtárból választható természetes személyre vagy szervezeti egységre vonatkozó adat vagy automatizmus által rögzített adat. |

| 8 | Érkeztető hely egyedi azonosítója | Betűt és számot egyaránt tartalmazó mező | Maximum 100 karakter | A szerv iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító (pl.: központi érkeztető könyv, elektronikus küldemények érkeztető könyve). |

| 9 | Érkeztető hely munkaállomás / szerver azonosítója | Betűt és/vagy számot tartalmazó, illetve speciális karakter | Maximum 30 karakter | Hálózati név / IP cím / gép név / szerver azonosító |

| 10 | Érkeztető könyv megnevezése | Szövegmező | Maximum 100 karakter | Az érkeztető könyvhöz kötődő, a szerv iratkezelési szabályzata alapján meghatározott szöveges megnevezés. |

| 11 | Érkeztető könyv azonosítója | Betűt és számot egyaránt tartalmazó mező | Maximum 10 karakter | A szerv iratkezelési szabályzata alapján képzett, meghatározott formátumú azonosító. |

| 12 | Érkeztető könyv nyitásának dátuma | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Az adott érkeztető könyv elektronikus érkeztető nyilvántartásban történő létrehozásának, megnyitásának időpontja. |

| 13 | Érkeztető könyv lezárásának dátuma | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Az adott érkeztető könyv elektronikus érkeztető nyilvántartásban történő lezárásának időpontja. |

| 14 | Érkeztető könyv státusza | Logikai mező | Választható értéke: Aktív / inaktív |  |

2. melléklet a 27/2014. (IV. 18.) KIM rendelethez
