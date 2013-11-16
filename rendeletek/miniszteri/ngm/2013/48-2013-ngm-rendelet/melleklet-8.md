## A tranzakciók, bizonylat szintű forgalmi és tranzakció-gyűjtő kapcsolatai

|  | A | B | C |

| 1. | TRANZAKCIÓ |

| 2. | TÍPUS | PARAMÉTER | HATÁS |

| 3. | ÉRTÉKESÍTÉS | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő növelése az Érték mező tartalmával |

| 4. | SZTORNÓ | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő csökkentése az Érték mező tartalmával SZTORNÓ tranzakció-gyűjtő növelése az Érték mező tartalmával |

| 5. | FELÁR | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő növelése az Érték mező tartalmával FELÁR tranzakció-gyűjtő növelése az Érték mező tartalmával |

| 6. | FELÁR SZTORNÓ | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő csökkentése az Érték mező tartalmával FELÁR tranzakció-gyűjtő csökkentése az Érték mező tartalmával |

| 7. | ENGEDMÉNY | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő csökkentése az Érték mező tartalmával ENGEDMÉNY tranzakció-gyűjtő növelése az Érték mező tartalmával |

| 8. | ENGEDMÉNY SZTORNÓ | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő növelése az Érték mező tartalmával ENGEDMÉNY tranzakció-gyűjtő csökkentése az Érték mező tartalmával |

| 9. | VISSZÁRU | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő csökkentése az Érték mező tartalmával VISSZÁRU tranzakció-gyűjtő növelése az Érték mező tartalmával |

| 10. | VISSZÁRU SZTORNÓ | Megnevezés, Érték, Áfa-jel | Áfa jel szerinti forgalmi gyűjtő növelése az Érték mező tartalmával VISSZÁRU tranzakció-gyűjtő csökkentése az Érték mező tartalmával |

| 11. | RÉSZÖSSZEG FELÁR | Megnevezés, Érték | Érték mező arányosítása a bizonylat forgalmi gyűjtőinek aktuális tartalma szerint Áfa jel szerinti forgalmi gyűjtők növelése az arányosított Értékekkel FELÁR tranzakció-gyűjtő növelése az Értékkel |

| 12. | RÉSZÖSSZEG FELÁR SZTORNÓ | Megnevezés, Érték | Érték ellenőrzése, Áfa jel szerinti forgalmi gyűjtők csökkentése az arányosított Értékekkel FELÁR tranzakció-gyűjtő csökkentése az Értékkel |

| 13. | RÉSZÖSSZEG ENGEDMÉNY | Megnevezés, Érték | Érték mező arányosítása a bizonylat forgalmi gyűjtőinek aktuális tartalma szerint Áfa jel szerinti forgalmi gyűjtők csökkentése az arányosított Értékekkel ENGEDMÉNY tranzakció-gyűjtő növelése az Értékkel |

| 14. | RÉSZÖSSZEG ENGEDMÉNY SZTORNÓ | Megnevezés, Érték | Érték ellenőrzése, Áfa jel szerinti forgalmi gyűjtők növelése az arányosított Értékekkel ENGEDMÉNY tranzakció-gyűjtő csökkentése az Értékkel |

8. melléklet a 48/2013. (XI. 15.) NGM rendelethez

## A pénztárgép napi funkcióinak leírása

|  | A | B | C |

| 1. | FUNKCIÓ | PARAMÉTER | TEVÉKENYSÉG |

| 2. | Napi nyitás |  | Dátum, idő, fejléc, Áfa értékek ellenőrzése, szinkronizálása, Euró bevezetésének időpontja rekord ellenőrzése, napi nyitás elutasítása, vagy elvégzése és „Napi nyitás” nem adóügyi bizonylat nyomtatása |

| 3. | Bizonylatnyitás | Bizonylattípus (NY / ESZ / NAB) | Fejléc nyomtatása, Bizonylatcím, vagy bizonylattípus nyomtatása |

| 4. | Tételsor nyomtatás | NY tételsor / ESZ tételsor | Bizonylat szintű forgalmi- és tranzakció-gyűjtők tartalmának növelése / csökkentése, tételsor nyomtatása, a nyomtatás ellenőrzése, vevőkijelzőre írás |

| 5. | Rész-összesen sor nyomtatás | Érték | Érték összehasonlítása a bizonylat szintű forgalmi gyűjtők tartalmának összegével, vevőkijelzőre írás, rész-összesen sor nyomtatása, vagy visszautasítása, és a bizonylat megszakítása |

| 6. | ÖSSZESEN sor nyomtatás | Érték | Érték összehasonlítása a bizonylat szintű forgalmi gyűjtők tartalmának összegével, vevőkijelzőre írás, ÖSSZESEN sor nyomtatása, vagy visszautasítása, és a bizonylat megszakítása |

| 7. | Megjegyzés sor nyomtatás | Megjegyzés sor | Megjegyzés sor nyomtatása, [vevőkijelzőre írás] |

| 8. | Bizonylat- megszakítás |  | NY és ESZ esetén: megszakítás szöveg, „ÖSSZESEN: 0 Ft” sor, bizonylat-sorszám, dátum, idő, AP sor nyomtatása, bizonylat szintű forgalmi- és tranzakciógyűjtők tartalmának ürítése, a megszakítás számláló és az érintett bizonylat-számláló növelése, [a következő bizonylat fejlécének nyomtatása, bizonylat-vágás] NAB esetén: megszakítás szöveg, dátum, idő, záró sor nyomtatása, [a következő bizonylat fejlécének nyomtatása, bizonylat-vágás] |

| 9. | Bizonylatzárás | NY / ESZ / NAB | NY és ESZ esetén: bizonylat-sorszám, dátum, idő, AP sor nyomtatása, a nyomtatás ellenőrzése, érintett napi szintű forgalmi- és tranzakció-gyűjtők tartalmának növelése a bizonylat szintű gyűjtők tartalmával, bizonylat szintű forgalmi- és tranzakció-gyűjtők tartalmának ürítése, érintett bizonylat számláló növelése, [a következő bizonylat fejlécének nyomtatása, bizonylat-vágás] NAB esetén: dátum, idő, záró sor nyomtatása, [a következő bizonylat fejlécének nyomtatása, bizonylatvágás] |

| 10. | Napi zárás |  | Fejléc sorok nyomtatása, GT érték növelése a napi szintű forgalmi gyűjtők összegével, „Napi forgalmi jelentés” nyomtatása, a nyomtatás ellenőrzése, Napi forgalom rekord Adóügyi Ellenőrző Egységbe írása, az írás ellenőrzése, napi szintű forgalmi- és tranzakció-gyűjtők tartalmának ürítése, napi számlálók nullázása, zárásszámláló növelése. |

|  | NY: Nyugta | ESZ: Egyszerűsített számla | NAB: Nem adóügyi bizonylat |

A funkciókhoz tartozó általános ellenőrzési tevékenységek:

1. a paraméterek szintaktikai és szemantikai ellenőrzése,

2. a perifériák (Adóügyi Ellenőrző Egység, nyomtató, vevőkijelző) működőképességének ellenőrzése.
