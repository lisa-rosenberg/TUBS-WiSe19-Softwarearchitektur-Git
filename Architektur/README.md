# Architektur und Datentypen

## Architektur
![Git-Architektur](Git-Architecture.png "Git-Architektur")

### 

### Quellen
* [Architecture of Open-Source-Software (Git)](https://www.aosabook.org/en/git.html)

## Datentypen und Referenzen
### Beschreibung der Datentypen
![Git-Objects](Git-Objects.png "Git-Objects")

#### blob
* Ähnlich einer Datei
* Aber: Dateiname wird nicht gespeichert!
* Inhalt von blob-Objekten
    * Objekttyp "blob"
    * SHA-1-Wert
    * Inhalt der Datei
    
#### tree
* Ähnlich zu einem UNIX-Ordner
* Inhalt von tree-Objekten
    * Objekttyp "tree"
    * SHA-1-Wert
    
#### commit
* Führt mehrere trees und blobs zu einer Art Snapshot-Objekt zusammen
* Commits werden dabei chronologisch sortiert
* Inhalt von commit-Objekten
    * Objekttyp "commit"
    * SHA-1-Wert vom root-tree-Objekt
    * SHA-1-Wert vom parent-commit-Objekt
    * Autor
    * Datum (Autor)
    * Committer
    * Datum (Comnmitter)
    * Commit-Message
    
#### tag
* Eine Art Pointer auf einen bestimmten Commit
* Ein bestimmter Commit kann durch einen annotierten Tag leichter wiedergefunden werden
* Inhalt von tag-Objekten
    * Objekttyp "tag"
    * SHA-1-Wert des Objektes, an das das Tag gesetzt wird
    * Objekttyp des Objektes, an das das Tag gesetzt wird
    * Tag-Name
    * Autor
    * Datum (Autor)
    * Tag-Message
    
### Git-References
![Git-References](Git-References.png "Git-References")

* Git-References bezeichnen Tags in einem Ordner innerhalb des .git-Ordners
* Sämtliche Tags sind dort gespeichert
    * Tags
    * Remote-HEADs (Remote-Branches, die durch Git-Fetch lokal bekannt sind)
    * Local-HEADs (Ausgecheckte lokale Branches)
* Branches sind eigentlich nur Tags, die auf den aktuellsten Commit eines Branches zeigen bzw. referenzieren
* Tags referenzieren persistent einen bestimmten Commit (z.B. "v.1.0")
* HEADs sind "dynamische/flüchtige" Tags, die auf einen bestimmten Commit zeigen 

### Quellen
* [Git Documentation: Git Internals - Git Objects](https://git-scm.com/book/en/v2/Git-Internals-Git-Objects)
* [Git Documentation: Git Internals - Git References](https://git-scm.com/book/en/v2/Git-Internals-Git-References)
* [Git Object Types](https://matthew-brett.github.io/curious-git/git_object_types.html)
* [Tags vs Branches](https://en.wikibooks.org/wiki/Git/Advanced)
* [Tagging](https://git-scm.com/book/en/v2/Git-Basics-Tagging)
