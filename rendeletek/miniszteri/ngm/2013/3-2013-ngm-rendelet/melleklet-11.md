## A taxaméter napi funkcióinak leírása

|  | A | B | C |

| 1. | FUNKCIÓ | PARAMÉTER | TEVÉKENYSÉG |

| 2. | Napi nyitás | Dátum, Idő, Fejléc sorok | Dátum, idő, fejléc, ellenőrzése, idő szinkronizálása, Euró bevezetésének időpontja rekord ellenőrzése, napi nyitás elutasítása, vagy elvégzése és „Napi nyitás” nem adóügyi bizonylat nyomtatása. Az utolsó nap-zárás dátumánál korábbi dátummal a nap nem nyitható meg, szabad jelző világít, napi km számlálás (taxi üzemmódban). |

| 3. | Nyugta nyitás |  | Fejléc sorok nyomtatása, „NYUGTA” szöveg nyomtatása |

| 4. | Nyugta tételsor nyomtatás | Megnevezés, Érték, | Bizonylat szintű tarifák, forgalmi- és km gyűjtők tartalmának nyomtatása, a nyomtatás ellenőrzése. |

| 5. | ÖSSZESEN sor nyomtatás | Érték | Érték mező tartalmának összehasonlítása a bizonylat szintű forgalmi és km gyűjtők tartalmának összegével, kijelzőre írás, ÖSSZESEN sor nyomtatása (vagy visszautasítása, és a bizonylat megszakítása) |

| 6. | Megjegyzés sor nyomtatás | Megjegyzés sor | Megjegyzés sor nyomtatása. |

| 7. | Nyugta megszakítás |  | „MEGSZAKÍTÁS” szöveg, „ÖSSZESEN: 0 Ft” sor, bizonylat-sorszám, dátum, idő, AP sor nyomtatása, a megszakítás számláló és az érintett bizonylat-számláló növelése, a bizonylat automatikus újranyomtatása. |

| 8. | Nyugta zárás |  | Bizonylat-sorszám, dátum, idő, AP sor nyomtatása, a nyomtatás ellenőrzése, érintett napi szintű forgalmi – és km gyűjtők tartalmának növelése a bizonylat szintű forgalmi – és km gyűjtők tartalmával, bizonylat szintű forgalmi- és km gyűjtők tartalmának ürítése, érintett bizonylat számláló növelése, szabad jelzés engedélyezése. |

| 9. | Napi zárás |  | Fejléc sorok nyomtatása, GT érték növelése a napi szintű forgalmi gyűjtők összegével, „Napi forgalmi jelentés” nyomtatása, a nyomtatás ellenőrzése, „Napi forgalom rekord” adómemóriába írása, az írás ellenőrzése, napi szintű forgalmi- és km gyűjtők tartalmának ürítése, napi számlálók nullázása, zárás-számláló növelése. |

## A funkciókhoz tartozó általános ellenőrzési tevékenységek:

## • A funkció végrehajthatóságának ellenőrzése (lásd 13. és 14. melléklet),

## • A paraméterek szintaktikai és szemantikai ellenőrzése,

## • A perifériák (adómemória, nyomtató, vevőkijelző) működőképességének ellenőrzése

## A személyszállítás megkezdésekor a taxi vezetője köteles a taxamétert foglalt állapotba állítani, ezzel a taxaméter bizonylat szintű mérési funkcióit elindítani. A szolgáltatás teljesítéséig a taxaméter kijelzőjén folyamatosan meg kell jeleníteni az alkalmazott tarifa mértékét és az aktuálisan fizetendő értéket.

11. melléklet a 3/2003 . (II. 15.) NGM rendelethez
