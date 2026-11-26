# Magyarország: a jog története gitben

**Magyar** · **[Read it in English](README.en.md)**

Magyarország joga git-történetként: egy fájl rendelkezésenként (§, cikk, melléklet), egy commit minden időállapotra azon a napon, amelyen hatályba lépett, és a commit szerzője a változást megállapító jogszabály. A [lexifina/global-law](https://github.com/lexifina/global-law) része (`hu/`).

**Mi van benne most:** az Alaptörvény minden időállapota 2012-től, és a törvények a Nemzeti Jogszabálytár (NJT) minden nyílt időállapotával 2010-től, a fő kódexekkel kezdve (Ptk., Btk., Pp., Be., Mt., Art., Áfa tv., Ákr., Kp., Szja tv.). A többi törvény, a rendeletek, a határozatok, a Magyar Közlöny és a bírósági határozatok folyamatosan kerülnek be.

## Szerkezet

- `alaptorveny/`: `nemzeti-hitvallas.md`, `cikk-A.md` ... `cikk-U.md`, `cikk-I.md` ... `cikk-XXXI.md`, `cikk-01.md` ..., `zaro-rendelkezesek.md`
- `torvenyek/<év>/<év>-evi-<római szám>-torveny[-<rövidítés>]/<n>-paragrafus.md` (például `torvenyek/2013/2013-evi-v-torveny-ptk/1-1-paragrafus.md` a Ptk. 1:1. §-a), `melleklet-<n>.md`, `preambulum.md`; minden törvény mappájában `README.md` az időállapotok táblázatával
- később: `rendeletek/`, `hatarozatok/`, `magyar-kozlony/`, `alkotmanybirosag/`, `birosagi-hatarozatok/`

## Kérdések git-parancsként

| Kérdés | Parancs |
| --- | --- |
| A Ptk. 6:519. §-ának minden változása | `git log -p -- torvenyek/2013/2013-evi-v-torveny-ptk/6-519-paragrafus.md` |
| Melyik jogszabály írta az Alaptörvény IX. cikkének sorait? | `git blame alaptorveny/cikk-IX.md` |
| A Btk. időállapotai a hatálybalépés napjával | `git log --format="%h %(trailers:key=In-force,valueonly,separator=) %an" -- torvenyek/2012/2012-evi-c-torveny-btk` |

## Dátumok és szerzők

Minden commit a hatálybalépés napján 12:00-kor (Europe/Budapest) kelt; a napot az `In-force:`, a forrást az `In-force-evidence:` és a `Source:` trailer adja (NJT időállapot `<azonosító>.<verzió>`). A 2010 előtti időállapotok nem nyíltak az NJT-ben; ezeket később a Magyar Közlönyből építjük újra. Jövőbeli időállapot a hatálybalépés napja előtt nem kerül be. A szerző az a jogszabály, amelyet az NJT lábjegyzetei az adott időállapotban új módosítóként neveznek meg; ahol ilyen nincs, `Nemzeti Jogszabálytár (egységes szerkezet)`. Hatályon kívül helyezés: a fájlokat törlő commit az utolsó időállapot végén.

A szöveg az NJT egységes szerkezetű szövege, nem hiteles kiadás; hiteles a Magyar Közlönyben kihirdetett szöveg. Ez nem jogi tanácsadás.

Licenc: [LICENSE](LICENSE) (a Lexifina munkája CC0; a jogszabályok szövege az Szjt. 1. § (4) bekezdése szerint nem áll szerzői jogi védelem alatt).
