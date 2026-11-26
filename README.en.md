# Hungary: law history in git

**[Magyarul](README.md)** · **English**

The law of Hungary as a git history: one file per provision (§, article, annex), one commit per time state (időállapot) on the day it took force, with the law that made the change as the commit author. Part of [lexifina/global-law](https://github.com/lexifina/global-law) (`hu/`).

**What is in it now:** the Fundamental Law (Alaptörvény) in every state from 2012, and the Acts of Parliament with every open time state of the Nemzeti Jogszabálytár (NJT) from 2010, main codes first (Civil Code, Criminal Code, Civil and Criminal Procedure, Labour Code, tax codes, administrative procedure). The remaining Acts, decrees, resolutions, the Magyar Közlöny gazette and court decisions are being added.

## Layout

- `alaptorveny/`: `nemzeti-hitvallas.md`, `cikk-A.md` ... `cikk-U.md`, `cikk-I.md` ... `cikk-XXXI.md`, `cikk-01.md` ..., `zaro-rendelkezesek.md`
- `torvenyek/<year>/<year>-evi-<roman>-torveny[-<abbreviation>]/<n>-paragrafus.md` (e.g. `torvenyek/2013/2013-evi-v-torveny-ptk/1-1-paragrafus.md` is Civil Code 1:1. §), `melleklet-<n>.md` (annexes), `preambulum.md`; each Act folder has a `README.md` listing its states
- later: `rendeletek/` (decrees), `hatarozatok/` (resolutions), `magyar-kozlony/`, `alkotmanybirosag/`, `birosagi-hatarozatok/`

## Questions as git commands

| Question | Command |
| --- | --- |
| Every change to Civil Code 6:519. § | `git log -p -- torvenyek/2013/2013-evi-v-torveny-ptk/6-519-paragrafus.md` |
| Which law wrote each line of Article IX of the Fundamental Law? | `git blame alaptorveny/cikk-IX.md` |
| Criminal Code states with their in-force days | `git log --format="%h %(trailers:key=In-force,valueonly,separator=) %an" -- torvenyek/2012/2012-evi-c-torveny-btk` |

## Dates and authors

Each commit is dated 12:00 Europe/Budapest on the in-force day; `In-force:` gives the day, `In-force-evidence:` and `Source:` the NJT time state (`<id>.<version>`). NJT's states before 2010 are not open; they will be rebuilt from the Magyar Közlöny later. Future states are not committed before their day. The author is the law NJT's footnotes name as making the changes new in that state, else `Nemzeti Jogszabálytár (egységes szerkezet)`. A repeal is a commit deleting the files at the end of the last state.

The text is NJT's consolidated text, not the authentic edition (that is the text promulgated in the Magyar Közlöny). Not legal advice.

Licence: [LICENSE](LICENSE) (Lexifina's work CC0; statutory text is outside copyright under Szjt. 1. § (4)).
