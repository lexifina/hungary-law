## A taxaméter funkciók és az adóügyi modul állapotának kapcsolatai (1)

|  | A | B | C | D | E | F | G | H | I | J | K |

| 1. | FUNKCIÓ | A VÉGREHAJTÁS |

| 2. | ÁLLAPOT-FELTÉTELEI | ÁLLAPOT VÁLTOZÁSAI |

| 3. | Adómemória indítási funkciók: | A | Á | K | I | B | A | Á | K | I | B |

| 4. | Dátum-, idő-állítás | - | - | - | - | - | - | - | - | - | - |

| 5. | „Azonosító rekord” írás | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 0 |

| 6. | „ÁFA rekord” írás | 1 | - | - | - | 0 | 1 | 1 | - | - | 0 |

| 7. | „Euró bevezetésének időpontja rekord” írás | 1 | - | - | - | 0 | 1 | - | 1 | - | 0 |

| 8. | Adómemória indítás | 1 | 1 | 1 | 0 | 0 | 1 | 1 | 1 | 1 | 0 |

## A taxaméter A=1&I=0&B=0 állapotban „gyakorló üzemmódban” működhet

8. melléklet az 49/2013. (XI. 15.) NGM rendelethez

## A taxaméter funkciók és az adóügyi modul állapotának kapcsolatai (2)

|  | A | B | C | D | E | F | G | H | I | J | K | L | M | N | O | P | Q | R | S |

| 1. | FUNKCIÓ | A VÉGREHAJTÁS |

| 2. | ÁLLAPOT-FELTÉTELEI | ÁLLAPOTVÁLTOZÁSAI |

| 3. | Napi, technikai, egyéb funkciók: | I | T | B | N | Y | Ö | M | K | E | I | T | B | N | Y | Ö | M | K | E |

| 4. | Napi nyitás | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | - | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | - |

| 5. | Nyugta / bizonylat nyitás | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | - | 1 | 0 | 0 | 1 | 1 | 0 | 0 | 1 | - |

| 6. | Tételsor nyomtatás | 1 | 0 | 0 | 1 | 1 | 0 | 0 | 1 | - | 1 | 0 | 0 | 1 | 1 | 0 | 0 | 1 | - |

| 7. | ÖSSZESEN sor nyomtatás | 1 | 0 | 0 | 1 | 1 | 0 | 0 | 1 | - | 1 | 0 | 0 | 1 | 1 | 1 | 0 | 1 | - |

| 8. | Megjegyzés sor nyomtatás | 1 | 0 | 0 | 1 | 1 | - | 0 | 1 | - | 1 | 0 | 0 | 1 | 1 | - | 0 | 1 | - |

| 9. | Nyugta / bizonylat megszakítás | 1 | 0 | 0 | 1 | 1 | - | - | 1 | - | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | - |

| 10. | Nyugta / bizonylat zárás | 1 | 0 | 0 | 1 | 1 | 1 | 0 | 1 | - | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | - |

| 11. | Adómemória adatai nyomtatás | 1 | - | - | 1 | 0 | 0 | 0 | 1 | - | 1 | - | - | 1 | 0 | 0 | 0 | 1 | - |

| 12. | Napi zárás | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | - | 1 | * | * | 0 | 0 | 0 | 0 | 1 | - |

| 13. | Dátum-, idő-állítás | - | - | - | 0 | 0 | 0 | 0 | - | - | - | - | - | 0 | 0 | 0 | 0 | - | - |

| 14. | „ÁFA rekord” írás | - | 0 | 0 | 0 | 0 | 0 | 0 | - | - | - | * | * | 0 | 0 | 0 | 0 | - | - |

| 15. | Fejléc beállítás | - | 0 | 0 | 0 | 0 | 0 | 0 | - | - | - | 0 | 0 | 0 | 0 | 0 | 0 | - | - |

| 16. | „RAM törlés rekord” írás | 1 | 0 | 1 | - | - | - | 0 | - | - | 1 | * | * | 0 | 0 | 0 | 0 | - | - |

| 17. | „Euró bevezetés Időpontja rekord” írás | - | 0 | 0 | 0 | 0 | 0 | 0 | - | 0 | - | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 |

| 18. | Euró üzemmód beállítása | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 1 |

* Az állapotjelző értéke 1-re változik, ha az adómemória megtelt, egyébként = 0.

1. A „bizonylat megszakítás” állapotjelzőt az adóügyi modul 1-re állítja, ha bizonylat nyomtatás közben:

a) hardver hiba történik,

b) nyugta, vagy ellenőrző papír kifogy,

c) a forgalmi adatok gyűjtése nem biztosított,

d) „Szinkronizálás” hiba esetén.

2. Betelt állapot esetén az egyéb állapotjelzők értékétől függetlenül biztosítani kell az adómemória adatainak kinyomtatását.
