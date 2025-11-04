# Git - Grundlegende Navigation

- [Einführung](#einführung)
- [Öffnen des BASH-Terminals](#bash-terminal-öffnen)
- [Navigieren durch Verzeichnisse](#durch-verzeichnisse-navigieren)
- [Auflisten von Verzeichnisinhalten](#verzeichnisinhalte-auflisten)
- [Erstellen und Löschen von Verzeichnissen](#verzeichnisse-erstellen-und-löschen)
- [Erstellen und Löschen von Dateien](#dateien-erstellen-und-löschen)
- [Fazit](#fazit)

# Einführung:
Das BASH-Terminal ist eine leistungsstarke Befehlszeilenschnittstelle, die es Benutzern ermöglicht, durch das Dateisystem ihres Computers zu navigieren, verschiedene Aufgaben auszuführen und mit Versionskontrollsystemen wie Git zu interagieren. Git ist ein weit verbreitetes verteiltes Versionskontrollsystem, das effiziente Zusammenarbeit und Nachverfolgung von Änderungen an Code-Repositories ermöglicht. In diesem Artikel werden wir erkunden, wie man sich durch die grundlegenden Befehle im BASH-Terminal bewegt und sie effektiv für die Arbeit mit Git nutzt.

## Öffnen des BASH-Terminals:
Um zu beginnen, öffnen Sie Ihre bevorzugte Terminalanwendung. Auf den meisten Unix-basierten Systemen finden Sie das Terminal im Ordner "Anwendungen" oder "Dienstprogramme". Nach dem Start erscheint eine Befehlsaufforderung, die bereit ist, Ihre Befehle entgegenzunehmen.

## Navigieren durch Verzeichnisse:
`pwd` steht für "Print Working Directory" und gibt den Pfad des aktuellen Arbeitsverzeichnisses aus.
```commandline
pwd
```
Dieser Befehl hat keine Argumente oder Optionen.

Der Befehl `cd` (Abkürzung für "change directory") ist grundlegend für die Navigation durch das Dateisystem. Hier sind einige häufige Beispiele für die Verwendung von `cd`:

Um in ein Verzeichnis zu wechseln, verwenden Sie `cd <verzeichnis>` (ersetzen Sie `<verzeichnis>` durch den gewünschten Verzeichnisnamen), z. B.:
```
cd Dokumente
```
Um eine Verzeichnisebene zurückzugehen, geben Sie `cd ..` ein, wie zum Beispiel:
```
cd ..
```
Um zum Benutzerverzeichnis zu wechseln, verwenden Sie `cd` oder `cd ~`, wie zum Beispiel:
```
cd ~
```
Um zum vorherigen Verzeichnis zu wechseln, verwenden Sie `cd -`, wie zum Beispiel:
```
cd -
```

## Auflisten von Verzeichnisinhalten:
Der Befehl `ls` wird verwendet, um die Inhalte eines Verzeichnisses aufzulisten. Standardmäßig zeigt er die Dateien und Verzeichnisse im aktuellen Verzeichnis an. Einige nützliche Flags zur Verbesserung der Funktionalität von `ls`:

`ls -l` zeigt die Inhalte in einer detaillierten Listenformatierung an.
```commandline
ls -l
```
`ls -a` zeigt versteckte Dateien und Verzeichnisse an.
```commandline
ls -a
```
`ls -h` zeigt lesbare Dateigrößen an.
```commandline
ls -h
```
`ls -R` listet Verzeichnisse und deren Inhalte rekursiv auf.
```commandline
ls -R
```

## Erstellen und Löschen von Verzeichnissen:
Sie können Verzeichnisse mit dem `mkdir`-Befehl und dem gewünschten Verzeichnisnamen erstellen:
Um ein Verzeichnis am aktuellen Speicherort zu erstellen, verwenden Sie `mkdir <verzeichnis>`. Zum Beispiel:
```
mkdir diesesverzeichnis
```
Um verschachtelte Verzeichnisse zu erstellen, verwenden Sie `mkdir -p <übergeordnetes_verzeichnis>/<untergeordnetes_verzeichnis>`.
```commandline
mkdir -p diesesverzeichnis/unterverzeichnis
```
Um Verzeichnisse zu löschen, verwenden Sie den Befehl `rmdir`:
`rmdir <verzeichnis>` löscht ein leeres Verzeichnis.
```commandline
rmdir diesesverzeichnis
```

## Verschieben und Umbenennen von Dateien und Verzeichnissen:
Der Befehl `mv` ermöglicht das Verschieben und Umbenennen von Dateien und Verzeichnissen:
Um eine Datei oder ein Verzeichnis zu verschieben, verwenden Sie `mv <quelle> <ziel>`. Zum Beispiel:
```commandline
mv diesesverzeichnis neuerverzeichnisname
```

Um eine Datei oder ein Verzeichnis umzubenennen, verwenden Sie `mv <alter_name> <neuer_name>`.
```commandline
mv altesverzeichnis neuesverzeichnis
```

## Erstellen und Löschen von Dateien:
Sie können eine neue Datei mit dem `touch`-Befehl erstellen.
```commandline
touch neue_datei_name
```
Oder in einem Verzeichnis, wie zum Beispiel:
```commandline
touch verzeichnis/neue_datei_name
```
Lassen Sie uns nun eine Datei mit dem `rm`-Befehl entfernen.
```commandline
rm datei_name
```
Um Verzeichnisse und deren Inhalte rekursiv zu entfernen
```commandline
rm -r datei_name
```
Um nicht vorhandene Dateien und Argumente zu ignorieren und niemals nachzufragen.
```commandline
rm -f datei_name
```
Um zu überprüfen, was getan wird
```commandline
rm -v datei_name
```
Um alles innerhalb eines Verzeichnisses zu entfernen.
```commandline
rm *
```
# Fazit:
Das BASH-Terminal, in Verbindung mit Git, bietet eine robuste Umgebung für effiziente Versionskontrolle und Dateiverwaltung. Durch die Vertrautheit mit grundlegenden Befehlen wie `mkdir`, `rmdir`, `rm`, `mv`, `cd`, `ls`, `pwd` und Git-spezifischen Befehlen wie `git init`, `git add`, `git commit`, `git push` und `git pull` können Sie durch Verzeichnisse navigieren, Verzeichnisse erstellen und löschen, Dateien verschieben und umbenennen, Dateien löschen und Ihre Git-Repositories effektiv verwalten. Praxis und