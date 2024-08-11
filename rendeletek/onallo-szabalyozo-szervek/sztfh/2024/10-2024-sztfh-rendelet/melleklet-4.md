## A 2. melléklet szerinti követelmények közül a következő követelmények esetében végzendő sérülékenységvizsgálat az értékelés során:

|  | A | B |

| 1. | Azonosító | Leírás |

| 2. | DEVID-3 | Távolról vezérelhető IoT-eszköz egyedi azonosítója és modelljelölése megállapítható. |

| 3. | DEVID-4 | Az IoT-eszköz biztosítson egyedi fizikai azonosító hozzáadására lehetőséget, amelyhez az arra jogosult entitások hozzáférnek. |

| 4. | DEVOP-3 | Nem jogosult felhasználó által az egyedi logikai IoT-eszközazonosító nem megismerhető. |

| 5. | IDSUPP-2 | Más IoT-eszközök hitelességének ellenőrzése biztosított. |

| 6. | IDSUPP-3 | Az IoT-eszköz hálózati és távoli hálózati kapcsolat esetén az azonosított kapcsolat felépítése előtt kriptográfiai alapú, kétirányú azonosítást végez. |

| 7. | IDSUPP-4 | Az IoT-eszköz tanúsítványalapú azonosítást és hitelesítést támogat. |

| 8. | DEVCONF-1 | A logikai hozzáférési jogosultságok beállítására, az IoT-eszköz konfigurációjára – A logikai hozzáférés az Interfészekhez című részben leírtak szerint – csak privilegizált felhasználókon keresztül nyílik lehetőség. |

| 9. | DEVCONF-2 | Csak arra jogosult felhasználók konfigurálhatják az IoT-eszköz azonosítási házirendjét és a hozzáférési korlátozási listákat. A logikai hozzáférés az Interfészekhez című résszel összhangban. |

| 10. | DEVCONF-3 | Csak arra jogosult felhasználók konfigurálhatják az IoT-eszköz logikai és fizikai interfészeit A logikai hozzáférés az Interfészekhez című résszel összhangban. |

| 11. | CRYPT-1 | Az IoT-eszköz megfelelő erősségű és hatékonyságú kriptográfiai algoritmust biztosít az adatok védelme érdekében. |

| 12. | CRYPT-2 | Az IoT-eszköz képes egyedi tanúsítványok érvényesítésére. |

| 13. | CRYPT-3 | Digitális aláírások ellenőrzése biztosított. |

| 14. | CRYPT-4 | Az IoT-eszköz képes Hash algoritmusok futtatására. |

| 15. | CRYPT-6 | Az eszköz forráskódja nem tartalmaz hard-coded kritikus biztonsági paramétereket. |

| 16. | CRYPT-7 | A szoftverfrissítések integritásának és hitelességének ellenőrzésére, valamint az eszközszoftverben a kapcsolódó szolgáltatásokkal folytatott kommunikáció védelmére használt kritikus biztonsági paramétereknek eszközönként egyedinek kell lenniük, és azokat olyan mechanizmussal kell előállítani, amely csökkenti az eszközosztályok elleni automatizált támadások kockázatát. |

| 17. | CRYKEY-1 | Az IoT-eszköz a kriptográfiai kulcsokat biztonságosan kezeli. |

| 18. | CRYKEY-2 | Az IoT-eszköz képes kulcspárok generálására. |

| 19. | CRYKEY-3 | Az IoT-eszköz a kriptográfiai kulcsokat biztonságosan tárolja. |

| 20. | CRYKEY-4 | Az IoT-eszköz a kriptográfiai kulcsok változtatását biztonságosan végzi. |

| 21. | CRYKEY-5 | Az IoT-eszköz a külső rendszerek által generált kriptográfiai kulcsokat ellenőrzi. |

| 22. | SECSTR-1 | Az IoT-eszköz a jelszavakat nem tárolja – ide nem értve az irreverzibilis kriptográfiai hasító függvénnyel a jelszóból képzett hash érték tárolást – és nem továbbítja. |

| 23. | SECSTR-4 | A személyes adatok védelme a természetes személyeknek a személyes adatok kezelése tekintetében történő védelméről és az ilyen adatok szabad áramlásáról, valamint a 95/46/EK irányelv hatályon kívül helyezéséről szóló, 2016. április 27-i (EU) 2016/679 európai parlamenti és tanácsi rendelettel (általános adatvédelmi rendelet) összhangban biztosított. |

| 24. | SECDT-3 | Az IoT-eszköz rendelkezik a jogosulatlan hozzáférés és módosítás elleni védelemmel az adatkapcsolati közegben. |

| 25. | SECDT-4 | Az IoT-eszköz a továbbított és fogadott adatok integritását kriptográfiai megoldással ellenőrzi. |

| 26. | AUTH-3 | Az IoT-eszköz többfaktoros hitelesítési metódust támogat meghatározott felhasználói kör esetén. |

| 27. | AUTH-5 | Az IoT-eszköz a gyári alapértelmezett jelszavak generálása során olyan generálási algoritmust alkalmaz, amely csökkenti az automata támadások kockázatát. |

| 28. | AUTH-7 | Az IoT-eszköz a hitelesítési folyamat során az adatokat elrejti. |

| 29. | AUTH-8 | Az IoT-eszköz standardizált, egységes authentikációs metódust támogat (pl. SAML, OAuth2). |

| 30. | AUTH-9 | Az IoT-eszköz távoli elérés esetén az authentikációs adatokat műveletenként ellenőrzi. |

| 31. | AUTH-10 | Az IoT-eszköz a hitelesítési metódus feedbackjében található információk rejtett visszacsatolásával biztosítja, hogy a hitelesítési azonosítók illetéktelenek számára megismerhetővé, újrafelhasználhatóvá váljanak. |

| 32. | IDENT-10 | Az IoT-eszköz a külső felhasználók és rendszerek authentikációját támogatja. |

| 33. | NOTIF-4 | Személyes adatokat tartalmazó, továbbá biztonsági értesítések teljes tartalma csak azonosítás után megismerhető, érzékeny adatok a figyelmeztető üzenetben nem jelennek meg. |

| 34. | ACCESS-1 | Az IoT-eszköz a jogosulatlan műveleteknek ellenáll. |

| 35. | ROLE-12 | Az IoT-eszköz az egyes felhasználótípusokhoz korlátozó feltételek megadására biztosít lehetőséget (pl. időalapú korlátozás, IP-korlát). |

| 36. | INTCTRL-2 | Az IoT-eszköz komponenseinek használata korlátozható (portok, funkciók, be- és kimeneti eszközök). |

| 37. | INTCTRL-3 | Azok a fizikai vagy logikai interfészek, amelyek nem szükségesek az IoT-eszköz működéséhez, tilthatóak. |

| 38. | INTCTRL-4 | Gyári alapértelmezett állapotban csak a telepítéshez, beüzemeléshez minimálisan szükséges logikai és fizikai interfészek engedélyezettek. |

| 39. | INTCTRL-5 | Gyári alapértelmezett állapotban az IoT-eszköz védelmet biztosít a biztonsági információk azonosítás nélküli kinyerése ellen. |

| 40. | INTCTRL-8 | A menedzsment felület elérésének külső hozzáférése tiltható. |

| 41. | INTCTRL-9 | Az IoT-eszköz logikai interfészeinek elérése szabályozható. |

| 42. | INTCTRL-10 | Az IoT-eszköz vezeték nélküli kapcsolatot támogat, amelynek biztonságos és engedélyezett authentikációs protokollja konfigurálható. |

| 43. | INTCTRL-11 | Ha az IoT-eszköz rendelkezik debug interfésszel, az szoftveresen tiltott. |

| 44. | UPD-4 | Feljogosított fiókok a szoftvert korábbi szoftververzióra visszaállíthatják (pl. downgrade attack). |

| 45. | UPD-5 | A szoftverfrissítések hiteles forrásból származnak, és ennek a feltételnek a teljesülését az IoT-eszköz ellenőrzi. |

| 46. | SECCOM-2 | Az IoT-eszköz forgalomirányítási szabályok érvényesítésére képes. |

| 47. | RESRC-3 | Az egyes folyamatok más folyamathoz rendelt memóriaterületet nem érnek el. |

| 48. | RESRC-4 | A memóriaterület csak kernelen keresztül hozzáférhető. |

| 49. | RESRC-5 | A memória hardveralapú hozzáférés-vezérléssel védett. |

| 50. | INT-1 | Az IoT-eszköz egyedi, nem hiteles forrásból származó kód futtatása elleni védelemmel rendelkezik. |

| 51. | INT-2 | Az IoT-eszköz rendelkezik a nem kívánt hardver- és szoftvermódosítás észlelési képességgel. |

| 52. | INT-4 | Az IoT-eszköz integritás-ellenőrző funkcióval rendelkezik. |

| 53. | INT-5 | Az IoT-eszköz a szoftverét biztonságos rendszerindítási mechanizmusok segítségével ellenőrzi. |

| 54. | INT-6 | Ha az IoT-eszköz a szoftver jogosulatlan módosítását észleli, figyelmezteti a felhasználót, illetve a rendszergazdát a problémára, és nem csatlakozik a riasztási funkció végrehajtásához szükségesnél szélesebb hálózatokhoz. |

4. melléklet a 10/2024. (VIII. 8.) SZTFH rendelethez

Értékelési módszertan
