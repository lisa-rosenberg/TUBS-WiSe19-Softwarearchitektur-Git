# Workflow

## Arbeitsweise von Git

### Quellen
* Bildquellen:
    * [Git-Lifecycle-git-scm](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository)
* [Git Internals - Plumbing and Porcelain](https://git-scm.com/book/en/v2/Git-Internals-Plumbing-and-Porcelain)


## Aktionen des Nutzers

### lokales Repository erhalten
#### git init
* lokales Verzeichnis in git-Repository umwandeln
#### git clone [Link]
* git-Repository von woanders (Link) klonen

### Änderungen zum Repository hinzufügen
#### git status
* Status/Zustand der Dateien prüfen
* zeigt Dateien, die unversioniert oder versioniert und bearbeitet sind
* gibt aktuellen Branch an
#### git diff
* Änderungen detailliert ansehen (geänderte Zeilen)
#### git add
* Dateien oder Änderungen zur Versionskontrolle hinzufügen
#### git commit
* Änderungen zum lokalen Repository hinzufügen
* erstellt "Schnappschuss" des Projektes zu aktuellem Zeitpunkt
* commits bilden Zustände, die später wieder hergestellt werden können
#### git rm
* Dateien aus Versionskontrolle entfernen
* zusätzliches Entfernen aus Working Directory

### Arbeiten mit Remote-Repository
#### git fetch
* lädt alle Daten aus Remote-Repository herunter, die lokal noch nicht vorhanden sind (ohne zu mergen)
#### git pull
* lädt Updates herunter und merged sie in lokales Repo
#### git push
* Updates ins Remote-Repository übertragen


### Quellen
* Bildquellen:
    * [Git Tutorial – Commands And Operations In Git](https://www.edureka.co/blog/git-tutorial/)
* [Einführung in Git (Teil 1): Versionsverwaltung](https://www.mittwald.de/blog/webentwicklung-design/webentwicklung/versionsverwaltung-einfuhrung-in-git-teil-1)
* [Git Basics - Getting a Git Repository](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)
* [Git Basics - Recording Changes to the Repository](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository)
* [Git Basics - Working with Remotes](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)
