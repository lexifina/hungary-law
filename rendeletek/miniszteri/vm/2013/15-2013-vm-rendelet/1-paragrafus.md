## I. Fejezet

## AZ ÁLLAMI ALAPADATOK ÉS TÉRKÉPI ADATBÁZISOK VONATKOZTATÁSI ÉS VETÜLETI RENDSZERÉRŐL

## 1. Értelmező rendelkezések

## 1. § E rendelet alkalmazásában:

1. aktív GNSS hálózat: folyamatosan üzemelő GNSS referenciaállomások hálózata, amely helymeghatározó alkalmazások széles körét szolgálja ki valós idejű-, illetve utólagos referenciaadatokkal;

2. alappont: az EOVA, EOMA, GNSSnet.hu országos hálózatán belül, helyi felmérési-kitűzési cél érdekében létrehozott helyi vízszintes, magassági és háromdimenziós felmérési alappont;

3. bázisállomás: ismert, vagy az adott munka folyamán meghatározott alapponton felállított GNSS vevőberendezés, amely ideiglenesen szolgáltatja a relatív helymeghatározásokhoz szükséges referenciaméréseket;

4. ciklus-többértelműség: a GNSS vevő és a műhold közötti távolságra eső vivőhullám egész ciklusai számának bizonytalansága;

5. EHT2 (ETRS89-EOV Hivatalos Helyi Térbeli Transzformáció): az ETRS89 és az EOV közötti, az OGPSH pontjaira támaszkodó, egységes, 7 paraméteres Helmert transzformációt alkalmazó szoftver;

6. EOMA (Egységes Országos Magassági Alapponthálózat): a magyar magassági vonatkoztatási rendszert fizikailag képviselő országos magassági alappontok hálózata;

7. EOTR (Egységes Országos Térképrendszer): Az állami térképi adatbázisok magyarországi térképezési és szelvényezési rendszere;

8. EOV (Egységes Országos Vetület): az állami földmérési, ingatlan-nyilvántartási, topográfiai térképi és távérzékelési adatbázisok és térképek sík vetületi rendszere;

9. EOVA (Egységes Országos Vízszintes Alapponthálózat): a magyar vízszintes vonatkoztatási rendszert fizikailag képviselő országos vízszintes alappontok hálózata EOV-ban adott koordinátákkal;

10. EPN (EUREF Permanens Hálózat): az ETRS89 vonatkoztatási rendszert a gyakorlatban megtestesítő európai aktív GNSS hálózat;

11. ETRS89: a GNSS méréseknek az európai kontinensen érvényes, 1989. évi epochára meghatározott földi vonatkoztatási rendszere;

12. EUREF: az európai szintű geodéziai vonatkoztatási rendszerek fenntartásáért és fejlesztéséért felelős szakmai szervezet;

13. EVRS2007: a magasságmérések európai vonatkoztatási rendszere;

14. félkinematikus módszer: ún. „stop and go” technikával végzett, rendszerint utófeldolgozáson alapuló, kinematikus mérési eljárás;

15. fix megoldás: a ciklus-többértelműség egész számként történő meghatározása;

16. float megoldás: a ciklus-többértelműség valós (nem egész) számként történő meghatározása;

17. GNSS (Global Navigation Satellite Systems): a globális műholdas helymeghatározó rendszerek (GPS, GLONASS, Galileo, COMPASS) közös elnevezése;

18. GNSSnet.hu: a központi földmérési és térinformatikai államigazgatási szervezet által fenntartott magyar aktív GNSS hálózat és az arra épülő szolgáltatások rendszere;

19. GSZK (GNSS Szolgáltató Központ): az aktív GNSS hálózat kiépítéséért és üzemeltetéséért felelős szervezet. A GSZK a referenciaállomásokról beérkezett mérési adatok feldolgozásával valós idejű korrekciókat és utófeldolgozáshoz szükséges adatokat állít elő és szolgáltat;

20. hálózati RTK: aktív GNSS hálózat állomásainak együttes méréseire támaszkodó, a felhasználó pozíciójára optimalizált valós idejű adatok felhasználásával végzett helymeghatározás;

21. INGA (Integrált Geodéziai Alapponthálózat): többféle szabatos geodéziai mérési technológiával - GNSS, szintezés, gravimetria - meghatározott alappontok szelektíven egyesített hálózata;

22. kisalappont: nem állandósított felmérési alappont, melynek meghatározása a mérés és számítás tekintetében az alappontokra vonatkozó követelmények szerint történt;

23. mérőállomás: olyan elektronikus földmérő műszer, mely digitálisan méri a távolságot, vízszintes és magassági szöget;

24. Mountpoint: az NtripCaster-en elérhető valós idejű GNSS adattípusok egyedi azonosítója;

25. Ntrip (Networked Transport of RTCM via Internet Protocol): RTCM adatok Interneten keresztül történő továbbítására szolgáló nemzetközi szabvány;

26. NtripCaster: Ntrip alapú valós idejű adattovábbításhoz szükséges szerver szoftver.

27. OGPSH (Országos GPS Hálózat): az EOVA hálózatból kiválasztott, az ETRS89 rendszerben GPS mérésekkel meghatározott alappontokból álló hálózat;

28. permanens állomás: ismert alapponton folyamatosan észlelő GNSS vevőberendezés;

29. ppm (parts per million): relatív pontossági mérőszám, az adott mértékegység egy-milliomod része;

30. referencia állomás: hitelesített és minőségbiztosítással ellátott, az aktív GNSS hálózat részét képező permanens állomás;

31. RTCM (Radio Technical Commission For Maritime Services): rádiónavigációs és rádiókommunikációs eljárások szabványosításáért felelős nemzetközi szervezet. A valós idejű GNSS helymeghatározás során felhasznált referenciaadatok nemzetközi szabványosítása az RTCM SC104 bizottság feladata;

32. RTK (Real Time Kinematic): GNSS fázismérésen alapuló valós idejű kinematikus helymeghatározás, ahol a helymeghatározást végző vevők különálló bázis-, permanens- vagy referenciaállomásokra támaszkodnak;

33. vesztett pont: nem állandósított, de a hálózat mérésében és számításában részt vevő geodéziai pont;

34. virtuális állomás: a referencia állomások méréseire támaszkodva, az aktív GNSS hálózattal lefedett terület tetszőleges helyére generált virtuális mérési adatok, korrekciók;

35. VITEL: valós idejű GNSS helymeghatározáshoz kidolgozott transzformációs eljárás, az EHT2 egyenértékű változata.
