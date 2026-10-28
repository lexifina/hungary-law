# Hungary: law history

This repository will hold the legislation of Hungary (HU) as a history: one file per provision and one commit per law taking effect, dated by the day it took force, with the law that made each change as the commit author. It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `hu/` in the world tree.

**Status:** no law yet. This first commit records where the law of Hungary can be read and what a build would need.

**Can it be built?** Past versions by date are online, but with no API or bulk download, so a build has to read the site page by page.

**This commit is a placeholder.** The first real build must replace this history from scratch and force-push. It must never append law commits on top of it: they are dated by when each law took effect, often decades earlier, so dates in `main` would run backwards and break every on-date lookup. Builders should refuse to append when the root commit is this placeholder (its subject ends "sources, before any law").

**Official sources**

- [Nemzeti Jogszabálytár](https://njt.jog.gov.hu): The text in force on any date from 2010 through ELI URIs such as /eli/TV/2010/45/2015-03-24, plus future states. HTML only. Old address njt.hu.

**Existing open projects to check first**

- [gitjog](https://github.com/godavid/gitjog): One commit per point-in-time state.

These are volunteer projects. Reconcile any of them against the official text before relying on it: a transcription is not the law (c3e/grundgesetz, for example, differs from the official gazette in 43 article texts on 20 July 2017).

All sources, with their status, are in [SOURCES.md](SOURCES.md). How these files were made is in [REPRODUCE.md](REPRODUCE.md).

This repository describes sources; it is not legal advice and holds no legal text yet.
