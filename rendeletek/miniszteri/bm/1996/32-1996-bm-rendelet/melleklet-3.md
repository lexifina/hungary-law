## Elektronikus adathordozón szolgáltatott adatok

| FILE név: NExxxx* INPUT rekordszerkezet |

| ssz. | mező neve | típusa | hossza | megjegyzés |

| 1. | Személyi azonosító | N | 11 |  |

| 2. | Házassági neve (családi név rész) | A | 50 |  |

| 3. | Házassági neve (első utónév része) | A | 20 |  |

| 4. | Házassági neve (második utónév része) | A | 20 |  |

| 5. | Születési családi neve | A | 50 |  |

| 6. | Születési első utóneve | A | 20 |  |

| 7. | Születési második utóneve | A | 20 |  |

| 8. | Választójogból kizárás oka | N | 1 | 2=Közügyektől eltiltva (KE) 3=Szabadságvesztés (BV) 4=Intézeti gyógykezelés (GY) |

| 9. | Választójogból kizárás kezdete | N | 8 | EEEEHHNN |

| 10. | Választójogból kizárás megszűnésének ideje | N | 8 | EEEEHHNN |

| 11. | Az okot elrendelő bíróság megnevezése | A | 67 |  |

| 12. | A határozat ügyiratszáma | A | 22 |  |

| 13. | A határozat kelte | N | 8 | EEEEHHNN |

| 14. | A határozat jogerőre emelkedésének ideje | N | 8 | EEEEHHNN |

| 15. | A szabadulás dátuma vagy az eltiltás megszűnésének ideje | N | 8 | EEEEHHNN |

| 16. | A küldő szerv(ezet) azonosítója | A | 5 | AAAAA=KEK KH BBBBB=Büntetés-végrehajtás OP. |

| 17. | Technikai mező | N | 2 | 99=rekord törlése |

## * A file névben az xxxx karakterek az adott évet és a hetet jelölik. Pl.: NE9602.txt; NE9651.txt

3. számú melléklet a 32/1996. (XII. 22.) BM rendelethez[^23]

Adatszerkezet

a választójoggal nem rendelkező

korlátozott belátási képességű személy adatairól

| Ssz. | Mező neve | Típusa | Hossza | Megjegyzés |

| ------------------------------------------------------------------------------------------------------------------------------------------ |

| 1. | A küldő járási gyámhivatal neve (településnév) | A | 23 |  |

| 2. | A küldő szerv(ezet) azonosítója | A | 6 | Pl. ASDFG |

| 3. | Személyi azonosító | N | 11 |  |

| 4. | Házassági neve (családi név rész) | A | 25 |  |

| 5. | Házassági neve (első utónév része) | A | 15 |  |

| 6. | Házassági neve (második utónév része) | A | 15 |  |

| 7. | Születési családi neve | A | 25 |  |

| 8. | Születési első utóneve | A | 15 |  |

| 9. | Születési második utóneve | A | 15 |  |

| 10. | Választójogból kizárás oka | A | 1 | 1= korlátozás esetén |

|  |  |  |  | üres = korlátozás törlése esetén |

| 11. | Választójogból kizárás kezdete | N | 8 | EEEEHHNN |

| 12. | A kizárást elrendelő bíróság neve | A | 67 | EEEEHHNN |

| 13. | A határozat ügyiratszáma | A | 22 |  |

| 14. | A határozat kelte | N | 8 | EEEHHNN |

| 15. | A határozat jogerőre emelkedésének dátuma | N | 8 | EEEEHHNN |

| 16. | A rögzítés dátuma | N | 8 | EEEEHHNN |

| 17. | Rögzítő neve, jele | A | 3 | balra igazított |

| 18. | Rögzítés hete | N | 4 | EEWW |

| 19. | Bizonylat száma | A | 10 |  |

[^23]: A 3. számú mellékletet az 50/2012. (XII. 4.) KIM rendelet 8. § (2) bekezdése iktatta be.
