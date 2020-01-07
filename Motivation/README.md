# Motivation

## Quellen
* [Qick Intro to Git and Github](http://hplgit.github.io/teamods/bitgit/html/._main_bitgit001.html)
* [Git for Scientists](https://neurathsboat.blog/post/git-intro/)
* [The entire Pro Git book - Kapitel 1.3](https://www.git-scm.com/book/de/v2)

## Entstehung
* für OpenSourceProjekt Linux Kernel (angestoßen von Linus Torvalds) wurde ab 2002 Bitkeeper verwendet (Verteilte Versionsverwaltung)
* 2005 ging Beziehnung zwischen Linux-Community und dem komertiellen Unternehmen von Bitkeeper zu Brücke -> kostenloser Zugang nicht mehr gewährt
* 2005 Geburt von Git (eigene Entwicklung eines Versionsverwaltungs-Tools der Linux-Community, wieder angestoßen von Linus Torvalds)

## Ziele von Git
* Geschwindigkeit
* einfaches Design
* gute Unterstützung von nicht linearer Entwiklung
* vollständige dezentrale Struktur
* Fähigkeit große Projekte effektiv zu verwalten


## Abgrenzung von Dropbox und GoogleDrive

### Alle
* Dateien auf verschiedenen Geräten teilen
* so viele Nutzer wie man möchte
* auf alte Versionen zugreifbar (bei Dropbox/GoogleDrive letzte 30 Tage)

### Git
* Kommentare für jede neue Verion -> leichteres Finden einer gewünschten alten Version
* Mergen bei Konflikten durch zeitgleiches Arbeiten an einer Datei -> alte Versionmuss nicht manuell gesucht und anschließend von Hand gemerged werden
* => Git ermöglicht schnelles Arbeiten im Team (bei kleinen und großen Projekten)