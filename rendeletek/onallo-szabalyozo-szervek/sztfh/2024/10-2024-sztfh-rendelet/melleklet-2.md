2. melléklet a 10/2024. (VIII. 8.) SZTFH rendelethez

Követelményrendszer

1. A biztonsági követelményrendszer tekintetében az 1. melléklet 1. pontja szerinti IoT-eszköz azonosító dokumentumban meghatározott eszköz által – megbízhatósági szintenként – teljesítendő követelményeket a C–E oszlop rögzíti.

2. A követelményrendszer a következő európai, illetve nemzeti szabványokra figyelemmel került kialakításra:

a) ETSI EN 303 645 V2.1.1,

b) NIST Special Publication 800-213A és

c) NIST Special Publication 800-53 Revision 5.

3. Bármely oszlopban

a) „–”-lel jelölt sorok a kontrollcsaládok elnevezését jelzik;

b) „X” jelzi, hogy az adott sorban szereplő biztonsági követelmény teljesítése a C–E oszlop szerinti megbízhatósági szinten kötelező;

c) „0” jelzi, hogy az adott sorban szereplő biztonsági követelmény teljesítése a C–E oszlop szerinti megbízhatósági szinten nem kötelező.

|  | A | B | C | D | E |

| 1. | Azonosító | Leírás | alap | jelentős | magas |

| 2. |  | ESZKÖZ AZONOSÍTÁSA | – | – | – |

| 3. |  | Eszközazonosítás | – | – | – |

| 4. | DEVID-1 | Az IoT-eszköz modelljelölése egyértelműen felismerhető, akár az eszközön található címkén, akár egy fizikai interfészen keresztül. | X | X | X |

| 5. | DEVID-2 | Az IoT-eszköz egyedi, az eszközön található címkén vagy interfészen keresztül lekérdezhető logikai azonosítóval rendelkezik. | X | X | X |

| 6. | DEVID-3 | Távolról vezérelhető IoT-eszköz egyedi azonosítója és modelljelölése megállapítható. | X | X | X |

| 7. | DEVID-4 | Az IoT-eszköz lehetőséget biztosít egyedi fizikai azonosító hozzáadására, amelyhez az arra jogosult entitások hozzáférnek. | 0 | X | X |

| 8. |  | Műveletvégzés | – | – | – |

| 9. | DEVOP-1 | Az IoT-eszköz képes olyan műveletek végrehajtására, amelyek az eszköz azonosítása alapján vagy a felhasználásával előfordulhatnak. | X | X | X |

| 10. | DEVOP-2 | Az IoT-eszköz képes különbséget tenni azonosított és nem azonosított felhasználók között. | X | X | X |

| 11. | DEVOP-3 | Nem jogosult felhasználó által az egyedi logikai IoT-eszközazonosító nem megismerhető. | 0 | X | X |

| 12. | DEVOP-4 | Az IoT-eszköz azonosító ismeretében az aktuális szoftververzió ellenőrizhető. | 0 | X | X |

| 13. | DEVOP-5 | A hálózati eszközök azonosítása és kezelése céljából az eszközazonosító felhasználható az IoT-eszköz felderítésére. | 0 | 0 | X |

| 14. |  | Eszközazonosítás támogatása | – | – | – |

| 15. | IDSUPP-1 | Az IoT-eszköz képes arra, hogy más eszközök számára előzetesen azonosított entitásként hirdesse magát. | 0 | X | X |

| 16. | IDSUPP-2 | Más IoT-eszközök hitelességének ellenőrzése biztosított. | 0 | X | X |

| 17. | IDSUPP-3 | Az IoT-eszköz hálózati és távoli hálózati kapcsolat esetén az azonosított kapcsolat felépítése előtt kriptográfiai alapú, kétirányú azonosítást végez. | 0 | 0 | X |

| 18. | IDSUPP-4 | Az IoT-eszköz tanúsítványalapú azonosítást és hitelesítést támogat. | 0 | 0 | X |

| 19. |  | ESZKÖZ KONFIGURÁCIÓJA | – | – | – |

| 20. | DEVCONF-1 | A logikai hozzáférési jogosultságok beállítására, az IoT-eszköz konfigurációjára – Külső kapcsolatok, interfész-kontroll követelményeknek megfelelően – csak privilegizált felhasználókon keresztül nyílik lehetőség. | X | X | X |

| 21. | DEVCONF-2 | Csak arra jogosult felhasználók konfigurálhatják az IoT-eszköz azonosítási házirendjét és a hozzáférési korlátozási listákat a Külső kapcsolatok, interfész-kontroll követelményekkel összhangban. | X | X | X |

| 22. | DEVCONF-3 | Csak arra jogosult felhasználók konfigurálhatják az IoT-eszköz logikai és fizikai interfészeit a Külső kapcsolatok, interfész-kontroll követelményekkel összhangban. | X | X | X |

| 23. | DEVCONF-4 | Feljogosított felhasználók konfigurálhatják az IoT-eszköz szoftverbeállításait. | X | X | X |

| 24. | DEVCONF-5 | Feljogosított felhasználók az IoT-eszközt gyári állapotára visszaállíthatják. | X | X | X |

| 25. | DEVCONF-6 | Feljogosított felhasználók az IoT-eszközt valamely korábbi – a gyáritól eltérő – biztonságos állapotára visszaállíthatják. | 0 | 0 | X |

| 26. | DEVCONF-7 | Az IoT-eszköz szervizelése, javítása alatt vagy után a korábbi konfigurációs állapot biztosított. | 0 | X | X |

| 27. |  | ADATVÉDELEM | – | – | – |

| 28. |  | Kriptográfiai támogatás | – | – | – |

| 29. | CRYPT-1 | Az IoT-eszköz megfelelő erősségű és hatékonyságú kriptográfiai algoritmust biztosít az adatok védelme érdekében. | X | X | X |

| 30. | CRYPT-2 | Az IoT-eszköz képes egyedi tanúsítványok érvényesítésére. | 0 | X | X |

| 31. | CRYPT-3 | Digitális aláírások ellenőrzése biztosított. | 0 | X | X |

| 32. | CRYPT-4 | Az IoT-eszköz képes Hash algoritmusok futtatására. | X | X | X |

| 33. | CRYPT-5 | A kriptográfiai algoritmusoknak és primitíveknek ajánlott verziókra frissíthetőek. | 0 | X | X |

| 34. | CRYPT-6 | Az eszköz forráskódja nem tartalmaz hard-coded kritikus biztonsági paramétereket. | 0 | X | X |

| 35. | CRYPT-7 | A szoftverfrissítések integritásának és hitelességének ellenőrzésére, valamint az eszközszoftverben a kapcsolódó szolgáltatásokkal folytatott kommunikáció védelmére használt kritikus biztonsági paraméterek eszközönként egyediek, és azokat olyan mechanizmussal állítják elő, amely csökkenti az automatizált támadások kockázatát. | X | X | X |

| 36. |  | Kriptográfiai kulcsok támogatása | – | – | – |

| 37. | CRYKEY-1 | Az IoT-eszköz a kriptográfiai kulcsokat biztonságosan kezeli. | X | X | X |

| 38. | CRYKEY-2 | Az IoT-eszköz képes kulcspárok generálására. | X | X | X |

| 39. | CRYKEY-3 | Az IoT-eszköz a kriptográfiai kulcsokat biztonságosan tárolja. | X | X | X |

| 40. | CRYKEY-4 | Az IoT-eszköz a kriptográfiai kulcsok változtatását biztonságosan végzi. | X | X | X |

| 41. | CRYKEY-5 | Az IoT-eszköz a külső rendszerek által generált kriptográfiai kulcsokat ellenőrzi. | 0 | X | X |

| 42. |  | Biztonságos tárolás | – | – | – |

| 43. | SECSTR-1 | Az IoT-eszköz a jelszavakat nem tárolja – ide nem értve az irreverzibilis kriptográfiai hasító függvénnyel a jelszóból képzett hash érték tárolást – és nem továbbítja. | X | X | X |

| 44. | SECSTR-2 | Biztonságos tárolás engedélyezhető az IoT-eszközön vagy annak interfészén keresztül. | X | X | X |

| 45. | SECSTR-3 | Gyári állapotban az adatok biztonságos, titkosított tárolása engedélyezett. | X | X | X |

| 46. | SECSTR-4 | A személyes adatok védelme a természetes személyeknek a személyes adatok kezelése tekintetében történő védelméről és az ilyen adatok szabad áramlásáról, valamint a 95/46/EK irányelv hatályon kívül helyezéséről szóló, 2016. április 27-i (EU) 2016/679 európai parlamenti és tanácsi rendelettel (általános adatvédelmi rendelet) összhangban biztosított. | X | X | X |

| 47. | SECSTR-5 | Az IoT-eszköz – ideértve az adatok elérését biztosító felhőinfrastruktúrát is – csak az üzemszerű működéséhez szükséges mennyiségű adatot tárolja. | X | X | X |

| 48. | SECSTR-6 | Az IoT-eszköz az adatokat képes lokálisan titkosítottan tárolni. | X | X | X |

| 49. | SECSTR-7 | Az IoT-eszközhöz kapcsolódó távoli rendszerelemek (pl. felhő) az adatokat titkosítottan tárolják. | 0 | X | X |

| 50. | SECSTR-8 | Érzékeny biztonsági paraméterek perzisztens tárolóban tárolódnak. | 0 | X | X |

| 51. | SECSTR-9 | A rendszer- és felhasználói adatok külön partíciókon helyezkednek el. | 0 | X | X |

| 52. | SECSTR-10 | Az adatok biztonságos mentése biztosított. | 0 | X | X |

| 53. | SECSTR-11 | Az IoT-eszközön lokálisan tárolt felhasználói adatok egyszerűen, visszaállíthatatlanul törölhetőek. | X | X | X |

| 54. | SECSTR-12 | Az IoT-eszközhöz kapcsolódó távoli rendszerelemek által tárolt felhasználói adatok egyszerűen törölhetőek. | 0 | X | X |

| 55. |  | Biztonságos adatátvitel | – | – | – |

| 56. | SECDT-1 | Az IoT-eszköz be- és kimeneti interfészein az adatáramlás biztonságos. | X | X | X |

| 57. | SECDT-2 | A biztonságos adatátvitel kriptográfiai algoritmusa konfigurálható. | 0 | X | X |

| 58. | SECDT-3 | Az IoT-eszköz rendelkezik a jogosulatlan hozzáférés és módosítás elleni védelemmel az adatkapcsolati közegben. | X | X | X |

| 59. | SECDT-4 | Az IoT-eszköz a továbbított és fogadott adatok integritását kriptográfiai megoldással ellenőrzi. | 0 | X | X |

| 60. |  | LOGIKAI HOZZÁFÉRÉS AZ INTERFÉSZEKHEZ | – | – | – |

| 61. |  | Azonosítás támogatása | – | – | – |

| 62. | AUTH-1 | Az IoT-eszköz támogat authentikációs metódusokat. | X | X | X |

| 63. | AUTH-2 | Az IoT-eszköz a kapcsolatok felépítéséhez – kiemelten a távoli kapcsolatok esetén – authentikációs metódus megkövetelésére képes. | X | X | X |

| 64. | AUTH-3 | Az IoT-eszköz többfaktoros hitelesítési metódust támogat meghatározott felhasználói kör esetén. | 0 | X | X |

| 65. | AUTH-4 | Ha az IoT-eszköz gyári alapértelmezett jelszavakat használ, azok eszközönként egyediek. | 0 | X | X |

| 66. | AUTH-5 | Az IoT-eszköz a gyári alapértelmezett jelszavak generálása során olyan generálási algoritmust alkalmaz, amely csökkenti az automata támadások kockázatát. | 0 | X | X |

| 67. | AUTH-6 | A használatban lévő hitelesítési mechanizmusnak megfelelő hitelesítő azonosító megváltoztatása egyszerűen biztosított a felhasználó számára. | X | X | X |

| 68. | AUTH-7 | Az IoT-eszköz a hitelesítési folyamat során az adatokat elrejti. | X | X | X |

| 69. | AUTH-8 | Az IoT-eszköz standardizált, egységes authentikációs metódust támogat (pl. SAML, OAuth2). | 0 | X | X |

| 70. | AUTH-9 | Az IoT-eszköz távoli elérés esetén az authentikációs adatokat műveletenként ellenőrzi. | 0 | 0 | X |

| 71. | AUTH-10 | Az IoT-eszköz a hitelesítési metódus feedbackjében található információk rejtett visszacsatolásával biztosítja, hogy a hitelesítési azonosítók illetéktelenek számára megismerhetővé, újrafelhasználhatóvá váljanak. | X | X | X |

| 72. |  | Azonosítás konfigurációja | – | – | – |

| 73. | IDENT-1 | Az IoT-eszköz életciklusa során az authentikációs metódusok, szabályok és korlátozások beállíthatóak és változtathatóak. | 0 | X | X |

| 74. | IDENT-2 | Az IoT-eszköz a fiókkezelést automatizált módon támogatja. | 0 | 0 | X |

| 75. | IDENT-3 | A sikertelen azonosítási kísérletek száma konfigurálható, amely után az IoT-eszköz az adott felhasználót tiltja meghatározott, beállítható időtartam erejéig. | 0 | X | X |

| 76. | IDENT-4 | Az IoT-eszköz a sikertelen azonosítási kísérletek miatt tiltott felhasználói fiók visszaállítását alternatív azonosítási metódussal támogatja. | 0 | 0 | X |

| 77. | IDENT-5 | Az IoT-eszköz visszajelzést ad a legutolsó sikeres authentikáció időpontjáról. | 0 | X | X |

| 78. | IDENT-6 | Az IoT-eszköz az inaktív fiókok kijelentkeztetését támogatja, amelynek időtartama konfigurálható. | X | X | X |

| 79. | IDENT-7 | Az IoT-eszköz az ideiglenes felhasználói fiókokat konfigurálható módon, automatikusan tiltja. | 0 | X | X |

| 80. | IDENT-8 | Az IoT-eszköz a sikertelen belépési kísérleteket naplózza, amelyekről riport készíthető. | X | X | X |

| 81. | IDENT-9 | Az IoT-eszköz a sikertelen belépési kísérletek számát a következő sikeres bejelentkezés során jelzi a felhasználó számára. | 0 | X | X |

| 82. | IDENT-10 | Az IoT-eszköz a külső felhasználók és rendszerek authentikációját támogatja. | X | X | X |

| 83. | IDENT-11 | A felhasználói fiókok, külső felhasználók és rendszerek hozzáférése visszavonható, amely esetében az IoT-eszköz a fennálló kapcsolatot bontja. | 0 | X | X |

| 84. | IDENT-12 | Az IoT-eszköz támogatja fiókok lejárati dátumának beállítását, amely lejárati dátumon túl az érintett fiók tiltásáról gondoskodik. | 0 | X | X |

| 85. |  | Felhasználók értesítése | – | – | – |

| 86. | NOTIF-1 | Az IoT-eszköz állapota ránézésre megállapítható státuszállapot-jelzők segítségével. | X | X | X |

| 87. | NOTIF-2 | Az IoT-eszköz kijelzőjén megjelenő információk konfigurálhatóak. | 0 | X | X |

| 88. | NOTIF-3 | Az IoT-eszköz képes a felhasználók számára (konfigurált módon) értesítéseket küldeni. | X | X | X |

| 89. | NOTIF-4 | Személyes adatokat tartalmazó, továbbá biztonsági értesítések teljes tartalma csak azonosítás után megismerhető, érzékeny adatok a figyelmeztető üzenetben nem jelennek meg. | 0 | X | X |

| 90. | NOTIF-5 | Az IoT-eszköz által kijelzett, küldött üzenetek tartalma konfigurálható. | 0 | X | X |

| 91. | NOTIF-6 | Ha a figyelmeztető üzenet az IoT-eszköz kijelzőjén jelenik meg, az IoT-eszköz biztosítja, hogy az üzenet felhasználói interakcióig a kijelzőn maradjon. | 0 | X | X |

| 92. |  | Hozzáférés-kezelés támogatása | – | – | – |

| 93. | ACCESS-1 | Az IoT-eszköz a jogosulatlan műveleteknek ellenáll. | X | X | X |

| 94. | ACCESS-2 | Az IoT-eszköz képes a felhatalmazott felhasználók és folyamatok (pl. csatlakozó rendszerek) azonosítására. | X | X | X |

| 95. | ACCESS-3 | Az IoT-eszköz különbséget tesz a feljogosított és nem feljogosított felhasználók között. | X | X | X |

| 96. | ACCESS-4 | Bizonyos, az üzemeltető által meghatározható funkciók azonosítás nélkül elérhetőek. | X | X | X |

| 97. |  | Szerepkörtámogatás és -kezelés | – | – | – |

| 98. | ROLE-1 | Az IoT-eszköz több típusú felhasználói fiók kezelésére képes. | X | X | X |

| 99. | ROLE-2 | Az IoT-eszköz elkülöníti legalább a következő típusú felhasználói fiókokat: személyhez kötött fiókok (általános és privilegizált), osztott privilegizált fiókok. | 0 | X | X |

| 100. | ROLE-3 | Az IoT-eszköz támogatja a felhasználói fiókok hozzáadását. | 0 | X | X |

| 101. | ROLE-4 | A felhasználói fiókokhoz szerepkörök rendelhetőek. | 0 | X | X |

| 102. | ROLE-5 | A felhasználói fiókok egyedi azonosítóval vannak ellátva. | 0 | X | X |

| 103. | ROLE-6 | Az IoT-eszköz szerepköralapú logikai hozzáférés-vezérlést végez. | 0 | X | X |

| 104. | ROLE-7 | Adminisztrátor felhasználó által a szerepkörökkel elérhető funkciók, folyamatok konfigurálhatóak. | 0 | X | X |

| 105. | ROLE-8 | A szerepkörök standardizált, egységes authorizációs metódusokkal kompatibilisek, a megfeleltetés konfigurálható (pl. LDAPS). | 0 | X | X |

| 106. | ROLE-9 | Adminisztrátor felhasználó által új szerepkör konfigurálható. | 0 | 0 | X |

| 107. | ROLE-10 | Alapértelmezetten a szerepkörök a legkisebb jogosultság elve mentén kerülnek kialakításra. | X | X | X |

| 108. | ROLE-11 | Az audit naplókhoz és biztonsági beállításokhoz való hozzáférés-kezelés konfigurációja támogatott. | 0 | X | X |

| 109. | ROLE-12 | Az IoT-eszköz az egyes felhasználótípusokhoz korlátozó feltételek megadására biztosít lehetőséget (pl. időalapú korlátozás, IP-korlát). | 0 | 0 | X |

| 110. | ROLE-13 | A szerepkörökhöz rendelt feljogosítók ellenőrzése a privilegizált funkciók és folyamatok elérésére irányuló felhasználói interakció esetén megtörténik. | 0 | 0 | X |

| 111. | ROLE-14 | Az egyes felhasználói fiókok esetén használt authentikációs metódusok konfigurálhatóak. | 0 | 0 | X |

| 112. | ROLE-15 | Osztott fiókok esetén konfigurálható fiókonként az egyidejű bejelentkezés engedélyezése (gyári állapotban tiltott). | 0 | X | X |

| 113. | ROLE-16 | Az IoT-eszköz képes előre beállított korlátozások érvényesítésére az eszköz használata során. | 0 | X | X |

| 114. |  | Külső kapcsolatok, interfész-kontroll | – | – | – |

| 115. | INTCTRL-1 | Az IoT-eszköz külső, 3rd party rendszerekkel való kapcsolatát biztonságos metódussal biztosítja. | X | X | X |

| 116. | INTCTRL-2 | Az IoT-eszköz komponenseinek használata korlátozható (portok, funkciók, be- és kimeneti eszközök). | X | X | X |

| 117. | INTCTRL-3 | Azok a fizikai vagy logikai interfészek, amelyek nem szükségesek az IoT-eszköz működéséhez, tilthatóak. | X | X | X |

| 118. | INTCTRL-4 | Gyári alapértelmezett állapotban csak a telepítéshez, beüzemeléshez minimálisan szükséges logikai és fizikai interfészek engedélyezettek. | X | X | X |

| 119. | INTCTRL-5 | Gyári alapértelmezett állapotban az IoT-eszköz védelmet biztosít a biztonsági információk azonosítás nélküli kinyerése ellen. | X | X | X |

| 120. | INTCTRL-6 | A fizikai interfészeket a hardver szükségtelen kockázatnak nem teszi ki. | 0 | X | X |

| 121. | INTCTRL-7 | Az IoT-eszköz szolgáltatásainak használata korlátozható. | 0 | X | X |

| 122. | INTCTRL-8 | A menedzsment felület elérésének külső hozzáférése tiltható. | 0 | X | X |

| 123. | INTCTRL-9 | Az IoT-eszköz logikai interfészeinek elérése szabályozható. | X | X | X |

| 124. | INTCTRL-10 | Az IoT-eszköz vezeték nélküli kapcsolatot támogat, amelynek biztonságos és engedélyezett authentikációs protokollja konfigurálható. | X | X | X |

| 125. | INTCTRL-11 | Ha az IoT-eszköz rendelkezik debug interfésszel, az szoftveresen tiltott. | 0 | X | X |

| 126. |  | SZOFTVERFRISSÍTÉS | – | – | – |

| 127. |  | Frissítési képességek | – | – | – |

| 128. | UPD-1 | Az IoT-eszköz szoftvere biztonságosan frissíthető a szoftver által biztosított módon vagy interfészen keresztül. | X | X | X |

| 129. | UPD-2 | A szoftverfrissítés azonosított, arra feljogosítással rendelkező felhasználói fiókkal végezhető el, biztonságos és konfigurálható mechanizmussal támogatva. | 0 | X | X |

| 130. | UPD-3 | Az IoT-eszköz szoftverének aktuális verziója lekérdezhető. | X | X | X |

| 131. | UPD-4 | Feljogosított fiókok a szoftvert korábbi szoftververzióra visszaállíthatják. | 0 | X | X |

| 132. | UPD-5 | A szoftverfrissítések hiteles forrásból származnak, és ennek a feltételnek a teljesülését az IoT-eszköz ellenőrzi. | X | X | X |

| 133. | UPD-6 | A szoftverfrissítések nem okozzák az IoT-eszköz kiberbiztonsági felkészültségének csökkenését, és ennek a követelménynek az ellenőrzésére az IoT-eszköz beépített metódussal rendelkezik. | 0 | X | X |

| 134. |  | Frissítések kezelése alkalmazástámogatás által | 0 | 0 | 0 |

| 135. | UPDCTRL-1 | Az IoT-eszköz a frissítések hitelességét és integritását ellenőrzi. | X | X | X |

| 136. | UPDCTRL-2 | Az IoT-eszköz automatikus frissítése kikapcsolható. | X | X | X |

| 137. | UPDCTRL-3 | Manuális és automatikus frissítési metódus támogatott. | X | X | X |

| 138. | UPDCTRL-4 | A frissítési metódus megválasztható. | X | X | X |

| 139. | UPDCTRL-5 | A szoftver állítható időközönként ellenőrzi új frissítés rendelkezésre állását. | X | X | X |

| 140. | UPDCTRL-6 | Újonnan megjelenő szoftververziókról az IoT-eszköz értesítést küld, amely funkció kikapcsolható. | X | X | X |

| 141. | UPDCTRL-7 | Újonnan megjelenő szoftververziókról az IoT-eszköz értesítést küld, az értesítendők köre konfigurálható. | 0 | 0 | X |

| 142. | UPDCTRL-8 | Az IoT-eszköz tájékoztatja a felhasználót arról, ha a frissítés az IoT-eszköz alapvető működésére kockázatot jelent. | 0 | X | X |

| 143. |  | ESEMÉNYKEZELÉS TÁMOGATÁSA | – | – | – |

| 144. |  | Naplózás | – | – | – |

| 145. | LOG-1 | Az IoT-eszköz képes események naplózására. | X | X | X |

| 146. | LOG-2 | Az IoT-eszköz külső naplózó rendszer kapcsolatot támogat. | 0 | X | X |

| 147. | LOG-3 | A naplóbejegyzések minimális tartalma a következő: az IoT-eszköz egyedi azonosítója, időjelzés, esemény forrása, esemény típusa, esemény besorolása, felhasználóazonosító vagy folyamatazonosító, esemény leírása. | 0 | X | X |

| 148. | LOG-4 | Az IoT-eszköz képes a hálózati kommunikáció naplózására. | 0 | X | X |

| 149. | LOG-5 | Az IoT-eszköz képes az eszközkonfiguráció változásainak naplózására. | 0 | X | X |

| 150. | LOG-6 | Az IoT-eszköz képes a sikeres és sikertelen hozzáférési kísérletek naplózására. | X | X | X |

| 151. | LOG-7 | Az IoT-eszköz képes a saját és szenzorai állapotának naplózására. | 0 | X | X |

| 152. | LOG-8 | A naplózható események listája alapján a naplózandó események konfigurálhatóak. | 0 | 0 | X |

| 153. | LOG-9 | Az IoT-eszköz állapota interfészen lekérdezhető. | 0 | X | X |

| 154. | LOG-10 | Az események maximális megőrzési ideje, a tárolt naplóesemények száma, illetve a naplóállomány maximális mérete beállítható. | 0 | X | X |

| 155. | LOG-11 | Az IoT-eszközön a megőrzési kritériumokon túli naplóállomány maradéktalan törlése biztosított. | 0 | X | X |

| 156. |  | Időjelzés kezelése | – | – | – |

| 157. | TIMESTP-1 | Az IoT-eszköz által naplózott események időjelzése legalább másodperc pontosságú. | 0 | X | X |

| 158. | TIMESTP-2 | Az IoT-eszköz NTP hálózati protokollt támogat. | 0 | X | X |

| 159. | TIMESTP-3 | Megbízható időforrás konfigurálható. | 0 | X | X |

| 160. | TIMESTP-4 | Az IoT-eszköz szabványos, UTC-re visszavezethető időjelzést használ. | 0 | X | X |

| 161. |  | Eseménykezelés támogatása | – | – | – |

| 162. | INC-1 | Az IoT-eszköz figyelmeztetést küld a biztonsági eseménynek tekintendő, konfigurált eseményekről. | 0 | X | X |

| 163. | INC-2 | Az IoT-eszköz figyelmeztetést küld a biztonsági eseménynek tekintendő, konfigurált eseményekről a kapcsolódó információs rendszerek felé. | 0 | 0 | X |

| 164. | INC-3 | A figyelmeztetés módja konfigurálható. | 0 | 0 | X |

| 165. | INC-4 | Az IoT-eszköz alternatív naplózási megoldást támogat az elsődleges naplózási mechanizmus kiesése esetére. | 0 | 0 | X |

| 166. |  | ESZKÖZBIZTONSÁG | – | – | – |

| 167. |  | Biztonságos kommunikáció | – | – | – |

| 168. | SECCOM-1 | Más eszközökkel való kapcsolat kezdeményezése és lezárása biztonságosan történik. | X | X | X |

| 169. | SECCOM-2 | Az IoT-eszköz forgalomirányítási szabályok érvényesítésére képes. | 0 | X | X |

| 170. | SECCOM-3 | Az IoT-eszköz a kommunikáció során standardizált protokollokat használ. | X | X | X |

| 171. | SECCOM-4 | Az IoT-eszköz IP-címe beállítható. | X | X | X |

| 172. | SECCOM-5 | Az IoT-eszköz interfészeinek portjai konfigurálhatóak. | 0 | X | X |

| 173. | SECCOM-6 | Az IoT-eszköz DNS-támogatással rendelkezik. | X | X | X |

| 174. |  | Erőforrások biztonságos használata | – | – | – |

| 175. | RESRC-1 | Az IoT-eszköz erőforrások megosztott használatára képes. | 0 | X | X |

| 176. | RESRC-2 | Az IoT-eszköz képes memóriaterületeket folyamatokhoz rendelni. | 0 | X | X |

| 177. | RESRC-3 | Az egyes folyamatok más folyamathoz rendelt memóriaterületet nem érnek el. | 0 | X | X |

| 178. | RESRC-4 | A memóriaterület csak kernelen keresztül hozzáférhető. | 0 | X | X |

| 179. | RESRC-5 | A memória hardveralapú hozzáférés-vezérléssel védett. | 0 | X | X |

| 180. | RESRC-6 | A lemezhasználathoz kvóták rendelhetőek. | 0 | 0 | X |

| 181. | RESRC-7 | Hálózati kapcsolat elvesztése esetén korlátozott működés biztosított. | X | X | X |

| 182. | RESRC-8 | Az IoT-eszköz tömörített adattárolást támogat. | 0 | 0 | X |

| 183. |  | Integritásvédelem | – | – | – |

| 184. | INT-1 | Az IoT-eszköz egyedi, nem hiteles forrásból származó kód futtatása elleni védelemmel rendelkezik. | 0 | X | X |

| 185. | INT-2 | Az IoT-eszköz rendelkezik a nem kívánt hardver- és szoftvermódosítás észlelési képességgel. | 0 | X | X |

| 186. | INT-3 | Az IoT-eszköz az alapkonfiguráció biztonsági megfelelőségét ellenőrző funkcióval rendelkezik. | 0 | X | X |

| 187. | INT-4 | Az IoT-eszköz integritás-ellenőrző funkcióval rendelkezik. | 0 | X | X |

| 188. | INT-5 | Az IoT-eszköz a szoftverét biztonságos rendszerindítási mechanizmusok segítségével ellenőrzi. | 0 | X | X |

| 189. | INT-6 | Ha az IoT-eszköz a szoftver jogosulatlan módosítását észleli, figyelmezteti a felhasználót, illetve a rendszergazdát a problémára, és nem csatlakozik a riasztási funkció végrehajtásához szükségesnél szélesebb hálózatokhoz. | 0 | X | X |

| 190. | INT-7 | Az IoT-eszköz a rendszer fejlesztési életciklusa során manipuláció észlelésére képes. | 0 | 0 | X |

| 191. | INT-8 | A futtató környezet read-only adathordozón tárolódik. | 0 | X | X |
