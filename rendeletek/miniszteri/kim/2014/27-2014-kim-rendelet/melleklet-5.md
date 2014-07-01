## A közfeladatot ellátó szerveknél alkalmazható iratkezelési szoftverek által kezelendő, az irattári kezelésre, levéltárba adásra, selejtezésre vonatkozó metaadatok

## 1. IRATTÁRI TERVRE ÉS IRATTÁRRA VONATKOZÓ METAADATOK

|  | A | B | C | D |

|  | Megnevezés | Mező típusa | Mező felépítése, korlátozások | Megjegyzés |

| 1 | Irattári terv | Betűt és számot egyaránt tartalmazó értékkészlet | Maximum 100 karakter | A szerv elsődleges besorolási sémája. |

| 2 | Irattári tételszám | Betűt és számot egyaránt tartalmazó mező | Maximum 30 karakter | A szerv elsődleges besorolási sémája szerinti azonosítók. |

| 3 | Irattári tételszám megnevezése | Betűt és számot egyaránt tartalmazó mező | Maximum 300 karakter |  |

| 4 | Megőrzési mód | Szövegmező | Maximum 30 karakter | A szerv által karbantartott és bővíthető listából választható, alapértékei: selejtezés, levéltárba átadás, helyben őrzendő. |

| 5 | Őrzési idő | Számmező ( pozitív egész szám) | Maximum 3 karakter | Években megadandó egész szám. |

| 6 | Átmeneti irattár megnevezése | Szövegmező | Maximum 100 karakter | A szerv által karbantartott és bővíthető listából választható, a feladat ellátásában illetékes szervezeti egység. |

| 7 | Átmeneti irattári átvevő | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, az átmeneti irattár kezelésére jogosult természetes személy. |

| 8 | Átmeneti irattárba adás dátuma | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Papír alapú ügyirat és elektronikus ügyirat esetén. |

| 9 | Átmeneti irattári átvétel időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Papír alapú ügyirat és elektronikus ügyirat esetén. |

| 10 | Átmeneti irattár munkaállomás / szerver azonosítója | Betűt és/vagy számot tartalmazó, illetve speciális karakter | Maximum 30 karakter | Hálózati név / IP cím / gép név / szerver azonosító |

| 11 | Központi irattár megnevezése | Szövegmező | Maximum 100 karakter | A szerv által karbantartott és bővíthető listából választható, a feladat ellátásában illetékes szervezeti egység. |

| 12 | Központi irattári átvevő | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, a központi irattár kezelésére jogosult természetes személy. |

| 13 | Központi irattárba küldés dátuma | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Papír alapú ügyirat és elektronikus ügyirat esetén. |

| 14 | Központi irattári átvétel időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | Papír alapú ügyirat és elektronikus ügyirat esetén. |

| 15 | Központi irattár munkaállomás / szerver azonosítója | Betűt és/vagy számot tartalmazó, illetve speciális karakter | Maximum 30 karakter | Hálózati név / IP cím / gép név / szerver azonosító |

| 16 | Kölcsönzés időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. |  |

| 17 | Kölcsönző | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, kölcsönzésre jogosult természetes személy. |

| 18 | Kölcsönzést engedélyező | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, kölcsönzést engedélyező természetes személy. |

| 19 | Kölcsönzési határidő | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | A kikölcsönzött irat/ügyirat visszaadásának határideje. |

| 20 | Visszavétel időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. | A kikölcsönzött irat/ügyirat visszavételének ideje. |

| 21 | Visszavevő | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, visszavételre jogosult természetes személy. |

## 2. AZ ÜGYIRAT SELEJTEZÉSÉRE, LEVÉLTÁRBA ADÁSÁRA VONATKOZÓ METAADATOK

|  | A | B | C | D |

|  | Megnevezés | Mező típusa | Mező felépítése, korlátozások | Megjegyzés |

| 1 | Selejtezhetőség dátuma | Dátummező (év) | éééé |  |

| 2 | Levéltárba adhatóság dátuma | Dátummező (év) | éééé |  |

| 3 | Új őrzési idő | Számmező (pozitív egész szám) | Maximum 3 karakter | A selejtezésre előkészítéskor megállapított további (újabb) őrzési évek száma (egész számban megadva). |

| 4 | Selejtezés időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. |  |

| 5 | Selejtező | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, selejtezésre jogosult természetes személy. |

| 6 | Levéltárba adás dátuma | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. |  |

| 7 | Levéltárnak átadó | Szövegmező | Maximum 50 karakter | A szerv által karbantartott és bővíthető listából választható, levéltárba adásra jogosult természetes személy. |

5. melléklet a 27/2014. (IV. 18.) KIM rendelethez

A közfeladatot ellátó szerveknél alkalmazható iratkezelési szoftverek által kezelendő naplózásra vonatkozó metaadatok

1. NAPLÓZÁSRA VONATKOZÓ METAADATOK

|  | A | B | C | D |

|  | Megnevezés | Mező típusa | Mező felépítése, korlátozások | Megjegyzés |

| 1 | Műveletet végrehajtó felhasználó neve, szervezeti egysége | Szövegmező | Maximum 100 karakter |  |

| 2 | Műveletet végrehajtó felhasználó azonosítója | Szövegmező | Maximum 30 karakter |  |

| 3 | Műveletet végrehajtó munkaállomásának azonosítója | Betűt és/vagy számot tartalmazó, illetve speciális karakter | Maximum 50 karakter | Hálózati név / IP cím / gép név. Az esemény keletkezési helye, a belépési pontok azonosítói. |

| 4 | Műveleti mező | Szövegmező | Maximum 30 karakter | A változtatott adatbázis mező felületen megjelenő címkéje. |

| 5 | Művelet végrehajtásának időpontja | Dátummező (év, hónap, nap, óra, perc) | éééé.hh.nn.óó.pp. |  |

| 6 | Művelet megnevezése | Betűt és számot egyaránt tartalmazó mező | Maximum 35 karakter | Az ISZ-szel végrehajtott művelet, alapértékei: módosítás, törlés, hozzáférés. |

| 7 | Művelet kimenetele | Szövegmező | Választható érték: sikeres / hibás |  |

| 8 | Változtatás előtti állapot | Betűt és számot egyaránt tartalmazó mező | Maximum 500 karakter | Az adat változtatás előtti értéke. |

| 9 | Megváltozott állapot | Betűt és számot egyaránt tartalmazó mező | Maximum 500 karakter | Az adat változtatását követő értéke. |
