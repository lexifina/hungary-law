5. melléklet az 49/2013. (XI. 15.) NGM rendelethez

## A taxaméter funkciók listája (adómemória indítási, technikai és egyéb funkciók)

|  | A | B | C |

| 1. | FUNKCIÓ | PARAMÉTER | TEVÉKENYSÉG |

| 2. | Dátum-, időállítás | ÉÉÉÉ, HH, NN, ÓÓ, PP, MM | A dátum paraméter összehasonlítása az adómemória utolsó „Napi forgalmi rekordjában” levő dátum értékével. Ha az utóbbi nagyobb, akkor a funkció visszautasítása, egyébként végrehajtása. |

| 3. | Azonosító rekord írása* | Sorszám | „Azonosító rekord” beírása az adómemóriába. |

| 4. | ÁFA rekord írása* | ÁFA XX%, vagy AAM | „ÁFA rekord” beírása az adómemóriába. |

| 5. | Fejléc beállítás* | Fejléc sorok | Fejléc sorok RAM, vagy EPROM területre írása |

| 6. | Adómemória indítás* |  | Adómemória indítása. |

| 7. | RAM törlés rekord írása* |  | RAM törlés számláló növelése, ellenőrzése, ha = 25, akkor a taxaméter „blokkolása”, egyébként „RAM törlés rekord” beírása az adómemóriába, napi számlálók, bizonylat és napi szintű gyűjtők tartalmának módosítása nélkül. A funkció csak a működtető program helyreállítására szolgál. |

| 8. | Euró bevezetésének időpontja rekord írása* | ÉÉÉÉ, HH, NN | „Euró bevezetésének időpontja” rekord beírása az adómemóriába |

| 9. | Euró üzemmód beállítása** | ÉÉÉÉ, HH, NN | Euró üzemmód beállítása |

| 10. | Adómemória adatai lista nyomtatása | Dátum (1), (2) Sorszám (1), (2) | „Adómemória adatai” lista nyomtatása. |

| 11. | Időszakos forgalmi jelentés |  | Napi szintű forgalmi és km gyűjtők, számlálók (napi, globális) értékének kinyomtatása adóügyi bizonylatként. |

| 12. | Információs lista |  | „Információs lista” kinyomtatása nem adóügyi bizonylatként. |

A funkciókhoz tartozó általános ellenőrzési tevékenységek

1. A funkció végrehajthatóságának ellenőrzése (lásd 8. melléklet).

2. A paraméterek szintaktikai, szemantikai ellenőrzése.

3. A perifériák (adómemória, nyomtató, kijelző) működőképességének ellenőrzése.

* Kizárólag regisztrált szerviz által elvégezhető funkciók.

** Az adóügyi modul által végrehajtható funkció.
