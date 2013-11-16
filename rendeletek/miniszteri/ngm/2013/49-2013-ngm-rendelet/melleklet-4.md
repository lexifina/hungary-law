## 1. Plombával való lezárhatóság ellenőrzése (a plombasérülés mutassa a készüléken történt illetéktelen beavatkozást, illetve a gépjárműből történő eltávolítást).

## 2. Hibakezelés ellenőrzése (blokkolt állapot biztosítása).

## Nyomtató

## 1. Bizonylat olvashatóságának ellenőrzése.

## 2. Megjelenített karakterek méretének ellenőrzése.

## 3. Nyomtatás indítási lehetőségek ellenőrzése.

## 4. Nyomtató hibajelzés ellenőrzése.

## 5. Taxaméter és nyomtató kapcsolatának ellenőrzése.

## Adómemória

## 1. Hozzáférhetetlenség ellenőrzése.

## 2. Módosítás elleni védelem ellenőrzés.

## 3. Adómemória eltávolítása és megtelte esetén a működésképtelenség biztosításnak ellenőrzése.

## 4. Göngyölt forgalomképzési képesség.

## 5. Indítási és egyéb technikai funkciók (pl. dátum-, időállítás, azonosító rekord, áfa rekord, adómemória indítás, adómemória adat nyomtatás, fejléc, váltópénzkezelés, fölözés).

## 6. Elektronikus kártya kötelező részegységeinek ellenőrzése.

## B) Informatikai vizsgálat

## 1. Tarifa tárolási képesség ellenőrzése.

## 2. Gépen futó programok vizsgálata (pl. forgalmi adatgyűjtés biztosítási lehetőség, napi szintű számlálók ellenőrzése, globális számlálók ellenőrzése, több vállalkozó adata kezelésének biztosítása, napi zárások megkülönböztetése vállalkozónként, nyomtatási kényszer kezelése sorszám folytonosság, sorszám formátum).

## 3. Napi feladatok ellenőrzése (pl. napi nyitás, foglalt állás, fizetett állás).

## 4. Kötelező adattartalom ellenőrzése a különböző adóügyi bizonylatokon.

## 5. Adóügyi bizonylat nyomtatott elemei elrendezésének vizsgálata (pl. megnevezés, formátum, reklámszöveg).

## 6. Nyomtatás megszakítás lehetőségének vizsgálata.

## 7. Értékhatár ellenőrzés (tételsorszám: 99 999, bizonylat szintű forgalmi gyűjtőszám: 999 999, napi forgalmi gyűjtők, sztornó gyűjtői: 9 999 999, göngyölített forgalom: 999 999 999).

## 8. A „gyakorló üzemmód” kezelésének ellenőrzése.

## C) Dokumentáció vizsgálata

## 1. A típusvizsgálathoz előírt és benyújtott valamennyi dokumentum vizsgálata.

## 2. A dokumentáció és a mintadarab azonosságának vizsgálata.

## 3. E jogszabályban előírtakat, továbbá a vonatkozó uniós irányelveket átültető tagállami jogszabályokban előírtakat igazoló tanúsítványok meglétének ellenőrzése.

4. melléklet az 49/2013. (XI. 15.) NGM rendelethez

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

A funkciókhoz tartozó általános ellenőrzési tevékenységek

1. A funkció végrehajthatóságának ellenőrzése (lásd 7-8. melléklet).

2. A paraméterek szintaktikai és szemantikai ellenőrzése.

3. A perifériák (adómemória, nyomtató, vevőkijelző) működőképességének ellenőrzése.

A személyszállítás megkezdésekor a taxi vezetője köteles a taxamétert foglalt állapotba állítani, ezzel a taxaméter bizonylat szintű mérési funkcióit elindítani. A szolgáltatás teljesítéséig a taxaméter kijelzőjén folyamatosan meg kell jeleníteni az alkalmazott tarifa mértékét és az aktuálisan fizetendő értéket.
