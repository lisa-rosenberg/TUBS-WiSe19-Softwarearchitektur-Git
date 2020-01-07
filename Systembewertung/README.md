# Systembewertung

## Bewertung der Design Patterns
### Verwendete Design Patterns in Git
* Linus Torvald hat Git (und auch Linux) ins Leben gerufen
* Als Linus Torvald Linux geschrieben hat, existierte das Buch "Design Patterns" noch nicht
* Er ist ein sehr erfahrener Programmierer und hat sich noch nie an Design Patterns orientiert
* Demnach wurden in Git keine Design Patterns verwendet

### Auffälligkeiten zur Architektur und Benutzung von Git
* Git ähnelt einem vereinfachten OS-Filesystem, da Linus Torvald eine starke OS-Sicht bei der Architekturplanung hat
* Git ist dezentralisiert
* Die Transaktionen in Git sind immutable
* Die Transaktionen in Git sind independently verifiable
* Git besteht zu fast 50% aus C-Programmcode, 35% Shell-Skripten, etwa 7% Perl-Skripten, 5% Tcl-Skripten und 2% Python-Programmcode
* Git ist ein inhaltsadressierbares Dateisystem mit einem daraufliegenden VCS-UI
* Der Kern von Git ist ein einfacher Key-Value-Speicher
* Git wird durch feste Kommandos über die CLI bedient
    * Unterscheidung zwischen Plumbing- und Porcelain-Kommandos wird getroffen
* Commits ähneln einer Linked List und damit ähnelt Git in gewisser Weise einer vereinfachten Blockchain

### Ähnlichkeiten zu bekannten Design Patterns
#### Entwurfsmuster
* Facade
    * Der User nutzt fast nur Porcelain-Kommandos
    * Nur in Ausnahmefällen werden Plumbing-Kommandos verwendet (händische/tiefe Eingriffe, nie normale Git-Nutzung!)
    * Porcelain-Kommandos rufen in der inneren Struktur von Git Plumbing-Kommandos auf

#### Architekturmuster
* Client-Server
    * Das Zusammenspiel zwischen remote- und local-Repository kann als Client-Server-Model angesehen werden
    * Mithilfe von z.B. git pull wird ein Request zum Webserver (z.B. GitHub) gesendet, auf dem das remote-Repository liegt
    * Als Antwort kann der Webserver den Request entweder akzeptieren oder ablehnen
* Peer-to-Peer
    * Zwischen mehreren entfernten Repositories besteht eine Art Peer-to-Peer-Netzwerk

### Quellen
* [Quora: Design Patterns of Git](https://www.quora.com/What-design-patterns-did-Linus-Torvalds-use-when-writing-Git)
* [Architecture of Open-Source-Software (Git)](https://www.aosabook.org/en/git.html)
* [Client-Server Model](https://techterms.com/definition/client-server_model)

## Persönliche Bewertung der Architektur