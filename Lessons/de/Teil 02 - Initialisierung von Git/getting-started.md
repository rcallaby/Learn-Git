# Git initialisieren - Erste Schritte

- [Grundlegende Git-Operationen](#grundlegende-git-operationen)
- [Einrichten eines Git-Repositorys unter Linux](#einrichten-eines-git-repositorys-unter-linux)
- [Einrichten eines Git-Repositorys unter Windows](#einrichten-eines-git-repositorys-unter-windows)
- [Einrichten eines Git-Repositorys unter macOS](#einrichten-eines-git-repositorys-unter-macos)

## Grundlegende Git-Operationen:
Git bietet eine Vielzahl von Befehlen für die Versionskontrolle, hier sind jedoch einige grundlegende:

`git init` initialisiert ein neues Git-Repository im aktuellen Verzeichnis. Zum Beispiel:
```
git init Verzeichnisname
```
`git clone <Repository-URL>` kopiert ein Remote-Repository auf Ihren lokalen Rechner. Zum Beispiel:
```
git clone Verzeichnisname
```
`git add <Datei>` staged Änderungen an einer Datei für den Commit.
```
git add . 
```
oder
```
git add Dateiname
```
`git commit -m "<Commit-Nachricht>"` committet die gestagten Änderungen im Repository. Zum Beispiel:
```
git commit -m "eine ausführliche Commit-Nachricht"
```

`git push` lädt Ihre committeten Änderungen in ein Remote-Repository hoch.
```
git push Repositoryname
```
`git pull` holt Änderungen aus einem Remote-Repository und führt sie in Ihrem lokalen Repository zusammen.
```
git pull
```

Im Folgenden finden Sie eine schrittweise Anleitung zur Einrichtung von Git unter Linux, Windows und macOS.

## Einrichten eines Git-Repositorys unter Linux:

Öffnen Sie ein Terminalfenster.

Navigieren Sie mit dem Befehl `cd` zum gewünschten Verzeichnis, in dem Sie Ihr Repository erstellen möchten. Zum Beispiel, um zum Verzeichnis ~/Dokumente zu navigieren, verwenden Sie den folgenden Befehl:

```
cd ~/Dokumente
```
Initialisieren Sie ein neues Git-Repository mit dem Befehl `git init`:

```
git init
```
Ihr Repository ist jetzt eingerichtet. Sie können nun Dateien hinzufügen, Änderungen committen und andere Git-Befehle verwenden.

## Einrichten eines Git-Repositorys unter Windows:

Installieren Sie Git auf Ihrem Windows-System, indem Sie es von der offiziellen Website herunterladen: https://git-scm.com/download/win. Führen Sie den Installer aus und folgen Sie den Installationsanweisungen.

Öffnen Sie Git Bash, das eine Linux-ähnliche Kommandozeilenumgebung unter Windows bereitstellt.

Navigieren Sie mit dem Befehl `cd` zum gewünschten Verzeichnis, in dem Sie Ihr Repository erstellen möchten. Zum Beispiel, um zum Verzeichnis "Dokumente" auf Laufwerk C: zu navigieren, verwenden Sie den folgenden Befehl:

```
cd /c/Dokumente
```
Initialisieren Sie ein neues Git-Repository mit dem Befehl `git init`:

```
git init
```
Ihr Repository ist jetzt eingerichtet. Sie können nun Dateien hinzufügen, Änderungen committen und andere Git-Befehle verwenden.

## Einrichten eines Git-Repositorys unter macOS:

Öffnen Sie das Terminal auf Ihrem Mac.

Navigieren Sie mit dem Befehl `cd` zum gewünschten Verzeichnis, in dem Sie Ihr Repository erstellen möchten. Zum Beispiel, um zum Verzeichnis "Dokumente" zu navigieren, verwenden Sie den folgenden Befehl:

```
cd ~/Dokumente
```
Initialisieren Sie ein neues Git-Repository mit dem Befehl `git init`:

```
git init
```
Ihr Repository ist jetzt eingerichtet. Sie können nun Dateien hinzufügen, Änderungen committen und andere Git-Befehle verwenden.

Nun, da Sie das Git-Repository eingerichtet haben, können Sie mit dem Hinzufügen von Dateien, dem Committen von Änderungen und anderen Git-Operationen fortfahren, indem Sie Befehle wie `git add`, `git commit`, `git push` usw. verwenden. Beachten Sie, dass für eine detailliertere Anleitung zu diesen Operationen die Git-Dokumentation oder andere Git-Tutorials herangezogen werden sollten.

**Hinweis: Die bereitgestellten Schritte gehen von einer grundlegenden Einrichtung für ein lokales Git-Repository aus. Wenn Sie ein Remote-Repository einrichten oder mit bestehenden Repositories auf Hosting-Plattformen wie GitHub oder GitLab arbeiten möchten, sind zusätzliche Schritte erforderlich.**