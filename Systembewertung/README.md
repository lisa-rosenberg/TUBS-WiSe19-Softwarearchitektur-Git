# Systembewertung
## Auffälligkeiten zur Architektur und Benutzung von Git
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

## Quellen
* [Quora: Design Patterns of Git](https://www.quora.com/What-design-patterns-did-Linus-Torvalds-use-when-writing-Git)

## Persönliche Bewertung der Architektur