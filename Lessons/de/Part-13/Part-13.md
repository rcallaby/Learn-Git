## Inhaltsverzeichnis

- [Verwendung von C# Codespaces in Github](#verwendung-von-c-codespaces-in-github)
    - [Voraussetzungen](#voraussetzungen)
    - [Arbeiten mit C# Codespaces](#arbeiten-mit-c-codespaces)
    - [Zusammenarbeit in der Entwicklung mit Codespaces](#zusammenarbeit-in-der-entwicklung-mit-codespaces)
- [Verwendung von Github Actions in C# Codespaces](#verwendung-von-github-actions-in-c-codespaces)
    - [Erstellen einer Codespace-Konfigurationsdatei:](#erstellen-einer-codespace-konfigurationsdatei)

# Verwendung von C# Codespaces in Github

GitHub Codespaces ist eine cloud-basierte Entwicklungsumgebung, die es Entwicklern ermöglicht, Code direkt innerhalb des GitHub-Repositories zu schreiben, zu erstellen, zu testen und zu debuggen. Es bietet eine leistungsstarke und bequeme Möglichkeit zur Zusammenarbeit mit Teammitgliedern und zum Arbeiten an Projekten, ohne dass eine komplexe Einrichtung oder Konfiguration erforderlich ist. Mit Codespaces können Sie direkt über Ihren Browser auf eine vollständig konfigurierte Entwicklungsumgebung zugreifen, was es einfach macht, an Ihrem Code von überall aus zu arbeiten.

In diesem Artikel werden wir erkunden, wie Sie C# Codespaces in GitHub einrichten und verwenden können, um C#-Projekte mühelos zu entwickeln. Wir werden auch Beispiele durchgehen, um die praktische Anwendung von Codespaces in der C#-Entwicklung zu veranschaulichen.

### Voraussetzungen

Bevor Sie mit C# Codespaces beginnen, stellen Sie sicher, dass Sie folgendes haben:

Ein GitHub-Konto: Sie benötigen ein Konto auf GitHub, um Codespaces erstellen und verwenden zu können.
Ein C#-Projekt: Bereiten Sie ein C#-Projekt vor, an dem Sie mit Codespaces arbeiten möchten. Sie können entweder ein neues Projekt erstellen oder ein vorhandenes verwenden.
Erstellen eines C# Codespace

Navigieren Sie zu Ihrem GitHub-Repository: Gehen Sie zunächst zum Repository, in dem Ihr C#-Projekt gehostet ist.

Klicken Sie auf die Schaltfläche "Code": Auf der Hauptseite des Repositories klicken Sie auf die grüne Schaltfläche "Code", um ein Dropdown-Menü anzuzeigen.

Wählen Sie "Mit Codespaces öffnen": Wählen Sie aus dem Dropdown-Menü "Mit Codespaces öffnen" aus. Wenn Sie Codespaces in diesem Repository noch nicht verwendet haben, werden Sie aufgefordert, eine Codespace-Konfigurationsdatei einzurichten.

Konfigurieren Sie Ihren Codespace (falls zutreffend): Wenn Sie Codespaces zum ersten Mal in diesem Repository einrichten, werden Sie aufgefordert, einen .devcontainer-Ordner mit einer devcontainer.json-Konfigurationsdatei zu erstellen. Diese Datei legt die Einstellungen für die Entwicklungsumgebung fest, einschließlich der Laufzeit, Erweiterungen und anderer Abhängigkeiten.

Hier ist eine Beispiel devcontainer.json-Datei für ein C#-Projekt:
```
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:5.0",
  "extensions": [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [5000]
}

```
In diesem Beispiel verwenden wir das offizielle .NET SDK 5.0-Image und installieren die C#-Erweiterung.

### Arbeiten mit C# Codespaces

Nachdem Ihr Codespace eingerichtet ist, können Sie darauf zugreifen, indem Sie auf den Tab "Codespaces" in Ihrem GitHub-Repository klicken. Wählen Sie den entsprechenden Codespace aus der Liste aus und klicken Sie auf "Verbinden", um die Entwicklungsumgebung in Ihrem Browser zu starten.

Sie werden mit einer vertrauten Visual Studio Code-Benutzeroberfläche begrüßt, die bereits mit allen notwendigen Tools für die Entwicklung von C#-Anwendungen konfiguriert ist.

Beispiel: Erstellen einer C#-Konsolenanwendung

Gehen wir durch ein Beispiel zur Erstellung einer einfachen C#-Konsolenanwendung unter Verwendung von Codespaces.

Verbindung zum Codespace herstellen: Befolgen Sie die oben beschriebenen Schritte, um Ihren Codespace zu erstellen und zu verbinden.

Öffnen Sie ein Terminal: Klicken Sie im Visual Studio Code auf das Menü "Terminal" und wählen Sie "Neues Terminal", um ein neues Terminalfenster zu öffnen.

Erstellen Sie eine neue C#-Konsolenanwendung: Verwenden Sie im Terminal die folgenden Befehle, um eine neue C#-Konsolenanwendung zu erstellen.

```
dotnet new console -n MyConsoleApp
cd MyConsoleApp

```
Code schreiben: Öffnen Sie die Datei Program.cs und schreiben Sie etwas Code in der Main-Methode.

```
using System;

namespace MyConsoleApp
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Hallo, Codespaces!");
        }
    }
}

```
Anwendung erstellen und ausführen: Verwenden Sie die folgenden Befehle, um die C#-Konsolenanwendung zu erstellen und auszuführen.

```
dotnet build
dotnet run

```

Sie sollten die Ausgabe "Hallo, Codespaces!" im Terminal sehen.

### Zusammenarbeit in der Entwicklung mit Codespaces

Einer der bedeutenden Vorteile von Codespaces ist seine Unterstützung für die Zusammenarbeit in der Entwicklung. Mehrere Teammitglieder können gleichzeitig an demselben Projekt arbeiten, jeder in seinem eigenen Codespace. Dies vermeidet Konflikte und vereinfacht den Prozess der Überprüfung und Zusammenführung von Codeänderungen.

Bei der Zusammenarbeit kann jeder Entwickler seinen eigenen Zweig erstellen, Änderungen vornehmen und wie gewohnt Pull Requests einreichen. Überprüfer können auch die Änderungen testen, indem sie die mit diesen Pull Requests verknüpften Codespaces starten, was den Überprüfungsprozess effizienter macht.

GitHub Codespaces bietet eine ausgezeichnete Plattform für C#-Entwickler, um gemeinsam und effizient zu arbeiten. Mit seiner cloud-basierten Entwicklungsumgebung und der einfachen Einrichtung können Sie sich auf das Schreiben von Code konzentrieren, ohne sich um die zugrunde liegende Infrastruktur kümmern zu müssen. Egal, ob Sie an persönlichen Projekten arbeiten oder zu Open-Source-Repositories

 beitragen, C# Codespaces optimieren Ihren Entwicklungsprozess und fördern die Zusammenarbeit zwischen Teammitgliedern.

# Verwendung von Github Actions in C# Codespaces

### Erstellen einer Codespace-Konfigurationsdatei:

Zunächst benötigen Sie eine .devcontainer/devcontainer.json-Datei, um Ihre Codespace-Umgebung zu konfigurieren. Hier ist ein Beispiel:

```
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:6.0",
  "extensions": [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [80]
}

```

Diese Konfiguration verwendet das .NET SDK 6.0-Image und installiert die C#-Erweiterung für Visual Studio Code.

Erstellen Sie eine Workflow-YAML-Datei: Erstellen Sie anschließend eine .github/workflows/build.yml-Datei, um Ihren GitHub Actions-Workflow zu definieren:

```
name: Build and Test

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - name: Code überprüfen
      uses: actions/checkout@v2

    - name: .NET einrichten
      uses: actions/setup-dotnet@v2
      with:
        dotnet-version: '6.0.x'

    - name: Abhängigkeiten wiederherstellen
      run: dotnet restore

    - name: Erstellen
      run: dotnet build --configuration Release

    - name: Tests ausführen
      run: dotnet test --configuration Release --no-build

```

Dieser Workflow wird bei Pushes in den Hauptzweig ausgelöst. Er richtet das .NET SDK ein, stellt Abhängigkeiten wieder her, erstellt das Projekt in der Release-Konfiguration und führt Tests aus.

Commit und Push: Commiten Sie die .devcontainer- und .github-Ordner zusammen mit Ihren C#-Projektdateien in Ihr GitHub-Repository.

Ausführung von GitHub Actions: Wenn Sie Änderungen in den Hauptzweig pushen, wird der in der build.yml-Datei definierte GitHub Actions-Workflow automatisch ausgeführt. Sie können den Fortschritt und die Ergebnisse des Workflows im Tab "Actions" Ihres GitHub-Repositorys überprüfen.

Denken Sie daran, dass diese Beispiele ziemlich grundlegend sind. Abhängig von der Komplexität und den Anforderungen Ihres Projekts können Sie den Workflow weiter anpassen, indem Sie Schritte für Bereitstellung, Integrationstests, Codeanalyse und mehr hinzufügen.

Bitte stellen Sie sicher, dass Sie diese Beispiele an die Struktur und Anforderungen Ihres Projekts anpassen.