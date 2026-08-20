## I. Általános rendelkezések

## 1. A bányavállalkozó a II–V. pont szerinti adatszolgáltatásokhoz

## 1.1. a vízszintméréseket az ME-10-231-24, ME-10-231-25, ME-10-231-26 szabványban,

## 1.2. a termálvizek minőségi vizsgálatát – akkreditált vízmintavétel alkalmazásával – az ISO 5667-11:2012 nemzetközi szabványban

## foglaltak szerint vagy azokkal egyenértékű műszaki megoldással végzi.

## A rendszeres mintavételekből származó vízminták elemzését a bányavállalkozó az ISO/IEC 17025:2005 szabvány előírásai szerint akkreditált laboratóriumban végezteti el

## II. A 15/E. § (4) bekezdés a) pontja alapján teljesítendő adatszolgáltatás tartalma és formája

## 1. A bányavállalkozó az adatszolgáltatás során a mérési adatsort ékezet nélküli karakterekkel elnevezett CSV formátumú állományban szolgáltatja. A CSV fájl elnevezése a következő:

## <kútazonosító>_<mért paraméter>_<mérési gyakoriság>_<küldési időpont>

## ahol:

## 1.1. kútazonosító: a bányavállalkozó adatszolgáltatása teljesítéséhez szükséges, a bányafelügyelet által megadott, a létesítmény megjelölésére szolgáló azonosító szám,

## 1.2. mért paraméter: a mért paraméter 3–5. pont szerinti jellemző kódja, amelyre a mérési adatsor vonatkozik,

## 1.3. mérési gyakoriság: óránkénti mérési adatok esetén: „ora”, napi összegzett adatok esetén: „napi”,

## 1.4. küldési időpont: az állomány elküldésének dátuma, ahol az év négy számjeggyel, a hónap két arab számjeggyel, a nap két számjeggyel szerepel, elválasztójel nélkül (így például: 20240906).

## 2. A bányavállalkozó valamennyi mért adatsort paraméterenként külön CSV állományban szolgáltatja; a CSV állomány tartalmazza:

## 2.1. az első sorban a mért paramétert és a mértékegységet pontosvesszővel elválasztva,

## 2.2. a második sorban a „time”, illetve „data” szavakat pontosvesszővel elválasztva,

## 2.3. a harmadik sortól soronként a mérési időpontokat (év-hó-nap óra:perc:másodperc) és a mért adatokat pontosvesszővel elválasztva.

## 3. A termelőkútban folyamatosan, legalább óránként mérendő paraméterek és paraméterkódjaik:

## 3.1. P01 termelt pillanatnyi vízhozam (l/perc),

## 3.2. P02 a víztermelés leállásának és újraindulásának időpontja,

## 3.3. P03 pillanatnyi vízszint (dinamikus kútfejnyomás vízoszlop magasságban) (mBf), termelés alatt és a leállás időszakában is,

## 3.4. P04 szivattyú pillanatnyi teljesítménye (kW),

## 3.5. P05 pillanatnyi vízhőmérséklet (°C),

## 3.6. P06 pillanatnyi fajlagos elektromos vezetőképesség (µS/cm 25 °C-ra megadva).

## 4. A visszasajtoló kútban folyamatosan, óránként mérendő paraméterek és paraméterkódjaik:

## 4.1. P07 visszasajtolt víz pillanatnyi vízhozama (l/perc),

## 4.2. P08 visszasajtolási nyomás (MPa),

## 4.3. P09 pillanatnyi, a kútban kialakult vízszint (mBf)/nyomás (MPa),

## 4.4. P10 pillanatnyi vízhőmérséklet (°C),

## 4.5. P11 a nem üzemelő visszasajtoló kútban a nyugalmi vízszint (mBf)/nyomás (MPa) a visszasajtolás leállítási idejének megjelölésével,

## 4.6. P12 fajlagos elektromos vezetőképesség (µS/cm 25 °C-ra megadva),

## 4.7. P13 szivattyú pillanatnyi teljesítménye (kW).

## 5. A napi összegzett paraméterek és paraméterkódjaik a termelő és a visszasajtoló kútra:

## 5.1. P14 napi összegzett termelt és visszasajtolt vízmennyiség (m3),

## 5.2. P15 napi üzemidő (óra),

## 5.3. P16 napi állásidő (óra).

## III. A 15/E. § (4) bekezdés b) pontja alapján teljesítendő adatszolgáltatás tartalma

## 1. A mérési dokumentáció adattartalma:

## 1.1. vízmintavétel/vízelemzés ideje,

## 1.2. vízmintavevő szervezet és a mintavevő neve,

## 1.3. vízmintavétel során mért vízhozam,

## 1.4. vízmintavételt megelőző kitermelt vízmennyiség (m3),

## 1.5. vizsgáló laboratórium neve, címe,

## 1.6. vizsgáló laboratórium akkreditálási száma,

## 1.7. vizsgáló laboratórium iktatószáma.

## 2. A helyszíni mérések adattartalma a vízmintavétel idején:

## 2.1. kifolyóvíz hőmérséklete a mintavételkor (°C),

## 2.2. helyszíni elektromos vezetőképesség (µS/cm 25 °C-ra megadva),

## 2.3. helyszíni pH.

## 3. A vízelemzés során végzett laboratóriumi vizsgálatok adattartalma:

## 3.1. elektromos vezetőképesség (µS/cm 25 °C-ra megadva),

## 3.2. összes oldottanyag tartalom (mg/l),

## 3.3. pH érték,

## 3.4. általános vízkémiai vizsgálat, főkomponensek: Na, Ca, K, Mg, Li, Fe, Mn, NH4+, Cl–, S2–, SO42–, HCO3–, CO32–, NO3–, NO2–, I–, Br–, meta-bórsav B-ban kifejezve, meta-kovasav, összes keménység, lúgosság, KOI, szabad szénsav,

## 3.5. izotóp vizsgálatok δ18O, δD, trícium vagy δ13C, 14C,

## 3.6. nyomelemek: Al, As, B, Cd, Cu, Hg, Mo, Ni, Pb, Sb, Se, Sr, Zn.

## IV. A 15/E. § (4) bekezdés c) pontja szerinti időszakos vizsgálat

## 1. Az időszakos vizsgálat tartalma:

## 1.1. talpmélység ellenőrzése,

## 1.2. egyéb, a kútszerkezetre vonatkozó ellenőrző mérés (lyukátmérő, szűrővizsgálat), amennyiben hiányosak, vagy a rendszeres üzemi mérések alapján feltételezhető a kútszerkezet változása (betétcsövezés, kúthiba, vízkőlerakódás),

## 1.3. kapacitásmérés (három hozamlépcső beállítása, vízhozammérés, üzemi kútfejnyomás- vagy vízszintmérés, nyugalminyomás-, illetve vízszintmérés a felszínen és a megnyitott szakasz felett),

## 1.4. a homokolás vizsgálata hozamlépcsőnként a felszínen vagy szükség esetén mélységi méréssel:

## 1.4.1. áramlásmérés,

## 1.4.2. folyamatos áramlásmérés a megnyitott szakaszokon és a tömszelencéknél,

## 1.4.3. folyamatos hőmérsékletmérés,

## 1.4.4. nyomásemelkedés-mérés a felszínen és a megnyitott szakasz felett,

## 1.4.5. nyomásgradiens-mérés a gázos kutaknál,

## 1.4.6. kifolyó víz hőmérsékletének mérése hozamlépcsőnként,

## 1.4.7. mélységi folyamatos hőmérsékletmérés,

## 1.4.8. felszíni és mélységi vízmintavétel, valamint -elemzés,

## 1.4.9. gáztartalmú kutaknál a termelt és szolgáltatott vizek gázmentesítéséről szóló miniszteri rendelet szerinti gázkapacitás-mérés és gázmintavétel-elemzés.

## V. A vízkémiai adatszolgáltatás formája:

## 1. Az adatszolgáltatás során eltérő helyszíni mérési vagy vízmintavételi időpont vagy eltérő laboratórium esetén a 2., illetve a 3. pontban szereplő táblázat szerinti jegyzőkönyvet mérési időpontonként, vízmintavételenként, laboratóriumonként külön kell kitölteni.

## 2. Helyszíni mérési jegyzőkönyv

|  | A | B | C |

| 1. | Helyszíni mérések |

| 2. | Kútazonosító |  |

| 3. | Helyszíni mérés vagy vízmintavétel időpontja | (ÉÉÉÉ.HH.NN.) |

| 4. | Mintaazonosító |  |

| 5. | Mintavevő vagy mérést végző szervezet neve |  |

| 6. | Akkreditációs száma |  |

| 7. | Mért paraméter | Érték | Mértékegység |

| 8. | pH |  |  |

| 9. | Fajlagos elektromos vezetőképesség |  | µS/cm 25 °C-ra megadva |

| 10. | Kifolyóvíz hőmérséklet |  | °C |

| 11. | Hozam |  | l/perc |

## 3. Laboratóriumi mérések adatai

|  | A | B | C |

| 1. | Kútazonosító |

| 2. | Laboratóriumi vizsgálati jegyzőkönyv kiállításának időpontja |  |

| 3. | Laboratórium neve |  |

| 4. | Akkreditációs száma |  |

| 5. | Mintaazonosító |  |

| 6. | Mért paraméter | Érték | Mértékegység |

| 7. | pH |  |  |

| 8. | Fajlagos elektromos vezetőképesség |  | µS/cm 25 °C-ra megadva |

| 9. | Kifolyóvíz hőmérséklet |  | °C |

| 10. | Kationok |

| 11. | Na |  | mg/l |

| 12. | K |  | mg/l |

| 13. | Ca |  | mg/l |

| 14. | Mg |  | mg/l |

| 15. | Li |  | mg/l |

| 16. | Fe |  | mg/l |

| 17. | Mn |  | mg/l |

| 18. | NH4+ |  | mg/l |

| 19. | Egyéb alkotók |

| 20. | B (HBO2) |  | B mg/l |

| 21. | Si (H2SiO3) |  | mg/l |

| 22. | m-lúgosság |  | mmol/l |

| 23. | p-lúgosság |  | mmol/l |

| 24. | Összes keménység |  | CaO mg/l |

| 25. | Karbonát keménység |  | CaO mg/l |

| 26. | KOI |  | O2 mg/l |

| 27. | TOC |  | mg/l |

| 28. | szabad szénsav |  | mg/l |

| 29. | Bepárlási maradék 180 °C |  | mg/l |

| 30. | Összes oldottanyag-tartalom |  | mg/l |

| 31. | Nyomelemek |

| 32. | Al |  | µg/l |

| 33. | As |  | µg/l |

| 34. | B |  | µg/l |

| 35. | Ba |  | µg/l |

| 36. | Cd |  | µg/l |

| 37. | Cr |  | µg/l |

| 38. | Cu |  | µg/l |

| 39. | Hg |  | µg/l |

| 40. | Mo |  | µg/l |

| 41. | Ni |  | µg/l |

| 42. | Pb |  | µg/l |

| 43. | Sb |  | µg/l |

| 44. | Se |  | µg/l |

| 45. | Sr |  | µg/l |

| 46. | Zn |  | µg/l |

| 47. | Anionok |

| 48. | Cl– |  | mg/l |

| 49. | SO42– |  | mg/l |

| 50. | S2– |  | mg/l |

| 51. | HCO3– |  | mg/l |

| 52. | CO32– |  | mg/l |

| 53. | NO3– |  | mg/l |

| 54. | NO2– |  | mg/l |

| 55. | PO43– |  | mg/l |

| 56. | I– |  | mg/l |

| 57. | Br– |  | mg/l |

| 58. | F– |  | mg/l |

| 59. | Izotóp vizsgálatok |

| 60. | δ18O |  | ‰ |

| 61. | δD |  | ‰ |

| 62. | trícium |  | Bq/l |

| 63. | δ 13C |  | ‰ |

| 64. | 14C |  | ‰ |

| 65. | Gáz vizsgálatok |

| 66. | Vízhozam |  | l/perc |

| 67. | Gázhozam |  | l/perc |

| 68. | Szeparált gáz |

| 69. | Oxigén |  | térfogat% |

| 70. | Nitrogén |  | térfogat% |

| 71. | Metán |  | térfogat% |

| 72. | Szén-dioxid |  | térfogat% |

| 73. | GVVsz |  | l/m3 |

| 74. | MVVsz |  | l/m3 |

| 75. | Oldott gáz |

| 76. | Oxigén |  | térfogat% |

| 77. | Nitrogén |  | térfogat% |

| 78. | Metán |  | térfogat% |

| 79. | Szén-dioxid |  | térfogat% |

| 80. | GVVo |  | l/m3 |

| 81. | MVVo |  | l/m3 |

| 82. | GVV (Fajlagos ö. gáztartalom) |  | l/m3 |

| 83. | MVV (Fajlagos ö. metán tartalom) |  | l/m3 |

6. melléklet a 20/2022. (I. 31.) SZTFH rendelethez[^226]

A földgáz, illetve hidrogén tárolására javasolt földtani szerkezet alkalmasságának bemutatása

1. A tárolókőzetre vonatkozó feltételek:

1.1. Annak igazolása, hogy a tárolásra kiválasztott földtani szerkezet petrofizikai és földtani tulajdonságai alkalmasak a maximális betárolási és kitermelési ütemhez.

1.2. A tárolásra kiválasztott földtani szerkezetből vagy földtanilag analóg mintából származó kőzetanyag-minta felhasználásával annak igazolása, hogy a tárolókőzet anyagával és a tárolókőzet pórusaiban található pórusfluidummal vagy jelenlevő egyéb gázokkal, a tárolásra jellemző nyomás- és hőmérsékleti értékek mellett, nem lépnek fel olyan kölcsönhatások, amelyek a tároló, vagy a tárolót elérő fúrások integritását veszélyeztetnék.

1.3. Kőzetmechanikai laboratóriumi mérésekkel és modellezéssel vagy termeléstörténeti adatokkal annak igazolása, hogy a betárolás és kitermelés során fellépő mechanikai hatásokra nem következnek be olyan mechanikai folyamatok, amelyek a tároló, vagy a tárolót elérő fúrások integritását veszélyeztetnék.

2. A fedőkőzetre vonatkozó feltételek:

2.1. A tárolásra kiválasztott földtani szerkezetből vagy földtanilag analóg környezetből származó kőzetanyag-minta felhasználásával annak igazolása, hogy a fedőkőzetek petrofizikai és földtani szempontból alkalmasak a tárolt földgáz, illetve hidrogén szivárgásmentes tárolására.

2.2. A tárolásra kiválasztott szerkezetből vagy földtanilag analóg környezetből származó kőzetanyag-minta felhasználásával annak igazolása, hogy a fedőkőzet anyagával és a fedőkőzet pórusaiban található pórusfluidummal, a tárolásra jellemző nyomás- és hőmérsékleti értékek mellett nem lépnek fel olyan kölcsönhatások, amelyek a zárást veszélyeztetnék.

2.3. Kőzetmechanikai laboratóriumi mérésekkel és modellezéssel vagy termeléstörténeti adatokkal annak igazolása, hogy a betárolás és kitermelés során fellépő mechanikai hatásokra nem következnek be olyan mechanikai folyamatok, amelyek a zárást veszélyeztetnék.

3. A kiválasztott tárolót vagy tárolórészt elérő, illetve harántoló kutakra vonatkozó feltételek:

3.1. A kiválasztott tárolót vagy tárolórészt elérő, vagy harántoló fúrások esetén anyagvizsgálati jelentésekkel, kútvizsgálati vagy termeléstörténeti dokumentációval igazolni szükséges, hogy azok jó állapotúak, a cementezés, dugózás, illetve béléscsövezés hibájából adódó szivárgás nem következik be.

3.2. Igazolni kell, hogy a tárolás időtartama alatt a cementezés, dugózás, illetve béléscsövezés anyaga és a pórusfluidum között, a tárolásra jellemző nyomás- és hőmérsékleti értékek mellett nem lépnek fel olyan kölcsönhatások, amelyek szivárgáshoz vezetnek.

[^226]: A 6. mellékletet a 14/2025. (XII. 22.) SZTFH rendelet 27. §-a iktatta be.
