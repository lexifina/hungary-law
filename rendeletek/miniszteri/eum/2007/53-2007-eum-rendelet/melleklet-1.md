1. számú melléklet az 53/2007. (XII. 7.) EüM rendelethez[^46]

## Az extra vonalkód adattartalma és műszaki leírása

1. Az „extra vonalkód” adattartalma:

a) a vény felírás dátuma,

b) a TAJ szám,

c) a BNO kód,

d) a vény felírás jogcíme,

e) a helyettesíthetőség,

f) a felírt gyógyszer TTT kódja,

g) a felírt gyógyszer mennyisége,

h) a külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslatot adó orvos pecsétszáma,

i) a külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslat keletkezésének ideje a vény felírás időpontjához viszonyítva,

j) a szoftver minősítésének azonosító kódja,

k) a program által a vénynyomtatás során használt gyógyszertörzs érvényességi idejének kezdő dátuma.

2. Az „extra vonalkód” adattartalmának kódolása:

a) A vény felírás dátuma: 1-től 366-ig terjedő, három számjegyből álló szám, amely azt jelzi, hogy a vényfelírás az év hányadik napján történt.

b) A TAJ szám 9 számjegye.

c) A BNO-kód: a nyomtatott vényen szereplő BNO-kód numerikus formában, mely úgy áll elő, hogy a BNO-kód első karaktere helyett minden esetben az adott karakter ASCII kódja szerepel, 2 számjegy hosszúságban. Ha az eredeti BNO-kód negyedik karaktere „H”, akkor helyette a vonalkódban „0” érték szerepel, továbbá az ma) pont szerinti bináris szám értéke „1”. Ha az eredeti BNO-kód negyedik karaktere nem „H”, akkor az ma) pont szerinti bináris szám értéke „0”.

d) A vény felírás jogcíme:

| Általános jogcím | 1 |

| HM jogcímen | 2 |

| Közgyógyellátási jogcím | 3 |

| Üzemi baleset | 4 |

| Eü. rend. jogcím | 5 |

| Eü. tér. köt. jogcím | 6 |

| Teljes ár | 7 |

| Eü. rend. és közgyógyellátási jogcím együtt | 8 |

| Eü. tér. köt. és közgyógyellátási jogcím együtt | 9 |

e) A helyettesíthetőség: értéke a „0” (nulla) vagy az „1” (egy) lehet. Az „1” jelentése, hogy a gyógyszer helyettesíthető, a „0” jelentése, hogy a gyógyszer nem helyettesíthető. A helyettesíthetőség értékét az mb) pont szerinti bináris számban kell feltüntetni.

f) A felírt gyógyszer TTT kódja, 9 számjegy hosszúságban. Többkomponensű magisztrális gyógyszer esetén TTT kódként 9 db „0” karakter írandó.

g) A felírt gyógyszer mennyisége: jobbra igazított, vezető nullákkal feltöltött, 3 karakter hosszúságú numerikus adat, bontott mennyiség esetén „000”.

h) A külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslatot adó orvos pecsétszáma, 5-nél kevesebb számjegyből álló pecsétszám esetén vezető nullával feltöltve. Ha az orvosi pecsétszám 6 számjegyből áll és az első számjegye „1”, azaz a pecsétszám értéke 100 000–199 999 közötti, akkor az mc) pont szerinti bináris szám értéke „1”, különben „0”. Amennyiben a gyógyszer rendelése szakorvosi javaslathoz nem kötött, akkor 5 karakter hosszúságban nullával feltöltve.

i) A külön jogszabály szerint szakorvosi javaslatra rendelhető készítmények esetén a szakorvosi javaslat időpontja és a vényfelírás időpontja között eltelt idő hónapban kifejezve, egész hónapra lefelé kerekítve, 2 számjegy hosszúságban. Amennyiben olyan gyógyszerről van szó, amely esetében a szakorvosi javaslat alapján határozatlan ideig lehet gyógyszert felírni és a javaslat 96 hónapnál régebbi, minden esetben a „99” számjegyeket kell használni. Amennyiben a gyógyszer rendelése szakorvosi javaslathoz nem kötött, akkor 2 karakter hosszúságban nullával feltöltve.

j) Az OEP által a szoftver minősítésekor adott 3 számjegyből álló szám.

k) A program által a vénynyomtatás során használt gyógyszertörzs érvényességi ideje kezdő dátumának hónapja és a vényfelírás dátumának hónapja között eltelt hónapok száma, egész hónapban számítva, lefelé kerekítve, 1 számjegy hosszúságban. Ha a két dátumban a hónapok megegyeznek, akkor a karakter értéke „0”; ha a gyógyszertörzs érvényességi ideje kezdő dátumából a hónap egy hónappal korábbi, mint a vényfelírás dátuma, akkor a karakter értéke „1” és így tovább.

l) Az ma), mb) és mc) alpontok értéke alapján képzett bináris szám decimális megfelelője, 1 számjegy hosszúságban. A képzett decimális szám bináris összetevői sorrendben az alábbiak:

ma) Ha a vényen szereplő BNO-kód negyedik karaktere „H”, akkor értéke „1”, különben „0”.

mb) Ha a gyógyszer az e) pont szerint helyettesíthető, értéke „1”, különben „0”.

mc) Amennyiben a h) pont szerinti orvos pecsétszáma hat számjegyű és első számjegye „1”, akkor értéke „1”, különben „0”.

3. Példa „extra vonalkód” adattartalmára és annak kódolására:

| Pozíció | Karakter tartalma | Hossz | Példa | Kódolt érték |

| 1–3 | a vény felírás dátuma | 3 | 2007. 02. 02 | 033 |

| 4–12 | a TAJ szám | 9 | 238338038 | 238338038 |

| 13–18 | a BNO kód | 6 | I10H0 | 731000 |

| – |  | – | +,,H” | → binA = 1 |

| 19–19 | a vény felírás jogcíme | 1 | Általános | 1 |

| – | a helyettesíthetőség | – | Helyettesíthető | → binB = 1 |

| 20–28 | a felírt gyógyszer TTT kódja | 9 | 210002737 | 210002737 |

| 29–31 | a felírt gyógyszer mennyisége | 3 | 99 | 099 |

| 32–36 | orvos pecsétszáma | 5 | 112345 | 12345 |

| – |  | – | + „1” | → binC = 1 |

| 37–38 | szakorvosi javaslat dátuma (relatív módon) | 2 | 2006.01.30 | 12 |

| 39–41 | az OEP által minősítéskor adott szám | 3 | 020 | 020 |

| 42–42 | törzs érvényességének kezdő hónapja (relatív módon) | 1 | 2006.12.01 | 2 |

| – | binA: BNO-kód 4. karaktere „H” | – | 1xx |  |

| – | binB: helyettesíthető | – | x1x |  |

| – | binC: pecsétszám 6 számjegyű, első karaktere „1” | – | xx1 |  |

| 43–43 | → binA, binB, binC decimális megfelelője | 1 | 111 | 7 |

4. Az „extra vonalkód” műszaki leírása: Code–128 jelkép MSZ EN 799:2001 számú szabvány 4.6 pontja alapján a jelkép méreteit és tűréseit az adott alkalmazási környezet határozza meg. A megfelelő leolvashatóság érdekében – figyelembe véve az olvashatóságot és a dekódolhatóságot – az X=0,33–0,495 mm közötti modulméret javasolt. Ugyancsak az alkalmazási környezet alapján a javasolt minimális vonalmagasság 12 mm (MSZ EN 799:2001 számú szabvány 4.6 pontja alapján). A jelkép előtt és mögött megjelenő világos nyugalmi mező X=0,33 mm esetén minimum 3,4 mm (MSZ EN 799:2001 számú szabvány 4.6.3.1 pontja alapján). A vonalkódba bekódolt adatok szemmel olvasható módon történő feltüntetése az adott alkalmazási környezetben tiltott.

[^46]: Az eredeti melléklet megjelölését 1. számú mellékletre változatta és szövegét megállapította a 46/2008. (XII. 3.) EüM rendelet 5. § (1) bekezdése. Az 1. számú melléklet a 9/2009. (IV. 8.) EüM rendelet 4. § (3) bekezdése, a 38/2009. (XI. 6.) EüM rendelet 6. § (7) bekezdése, a 4/2010. (VIII. 12.) NEFMI rendelet 3. § (3) bekezdés a)–b) pontja szerint módosított szöveg.
