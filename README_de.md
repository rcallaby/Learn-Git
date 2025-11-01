# Learn-Git
Hier finden Sie ein Beispiels-Repository für meine YouTube-Tutorial-Serie zum Thema Lernen von Git und Github.
Wenn Sie dieses Repository hilfreich finden, überlegen Sie bitte, ihm einen Stern ⭐ zu geben, da es so für andere leichter zu finden ist.

Außerdem würde es mir sehr helfen, wenn Sie meinen [YouTube-Kanal](https://www.youtube.com/@richardcallaby) abonnieren würden, denn das ist der Ort, an dem ich kostenlose Tutorials und andere kostenlose Bildungsmaterialien veröffentliche.

## Hier ist ein Schritt-für-Schritt-Tutorial, wie Sie zu GitHub beitragen können
Erstellen Sie ein GitHub-Konto: Wenn Sie noch kein GitHub-Konto haben, müssen Sie eins erstellen. Gehen Sie zu github.com und klicken Sie auf die Schaltfläche "Anmelden" oben rechts. Folgen Sie den Anweisungen, um Ihr Konto zu erstellen.

Suchen Sie ein Repository zum Beitrag: Nachdem Sie ein GitHub-Konto haben, können Sie nach Repositories suchen, zu denen Sie beitragen möchten. Sie können die GitHub-Suchleiste verwenden, um nach Repositories nach Namen oder Stichwort zu suchen.

Gabeln Sie das Repository: Wenn Sie ein Repository gefunden haben, zu dem Sie beitragen möchten, müssen Sie es gabeln.

Durch das Gabeln wird eine Kopie des Repositorys in Ihrem eigenen GitHub-Konto erstellt, die Sie ohne Auswirkungen auf das Originalrepository ändern können.

### Referenzbild
Klicken Sie auf die Schaltfläche unten, um das Repository zu gabeln, das sich oben rechts befindet.

![fork_image](./images/Readme_images/fork.png)

Klonen Sie das gegabelte Repository: Nachdem Sie das Repository gegabelt haben, müssen Sie es auf Ihren lokalen Computer klonen. Das Klonen erstellt eine Kopie des Repositorys auf Ihrem Computer, an dem Sie arbeiten können. Um das Repository zu klonen, öffnen Sie ein Terminalfenster und geben Sie den folgenden Befehl ein:

```
git clone https://github.com/your-username/repository-name.git
```
Stellen Sie sicher, dass Sie "your-username" und "repository-name" durch Ihren GitHub-Benutzernamen und den Namen des gegabelten Repositorys ersetzen.

### Referenzbild
![Clone_repo](./images/Readme_images/Clone.png)

Stellen Sie sicher, dass Sie einen eindeutig benannten Branch erstellen, um die Änderungen widerzuspiegeln, die Sie am Quellcode vornehmen möchten. Verwenden Sie die folgende Syntax, um einen Branch zu erstellen:

```
git branch "branch-name"
```
### Referenzbild
![branch_making](./images/Readme_images/Branch_making.png)

Um auf diesen Branch umzuschalten, verwenden Sie die folgende Syntax:
```
git checkout "branch-name"
```
### Referenzbild
![branch_switch](./images/Readme_images/branch_switch.png)

Nehmen Sie Änderungen am Code vor: Nachdem Sie das Repository auf Ihren lokalen Computer geklont haben, können Sie Änderungen am Code vornehmen. Verwenden Sie Ihren bevorzugten Texteditor oder Ihre IDE, um die Dateien zu ändern.

Bestätigen Sie die Änderungen: Nachdem Sie Änderungen am Code vorgenommen haben, müssen Sie sie in Ihrem lokalen Repository bestätigen. Öffnen Sie dazu ein Terminalfenster und navigieren Sie zum Stammverzeichnis des geklonten Repositorys. Verwenden Sie den folgenden Befehl, um die Änderungen zu stagen:

```
git add .
```

### Referenzbild
![add](./images/Readme_images/add.png)

Dies wird alle Änderungen an den Dateien im Repository stagen.

Bestätigen Sie als Nächstes die Änderungen mit dem folgenden Befehl:

```
git commit -m "Eine kurze Beschreibung der vorgenommenen Änderungen"
```

### Referenzbild
![Commit](./images/Readme_images/commit.png)

Achten Sie darauf, eine kurze, informative Nachricht einzufügen, die die vorgenommenen Änderungen beschreibt.

Pushen Sie die Änderungen auf GitHub: Nachdem Sie die Änderungen in Ihrem lokalen Repository bestätigt haben, müssen Sie sie auf GitHub pushen. Dadurch wird die Kopie des Repositorys in Ihrem GitHub-Konto mit den von Ihnen vorgenommenen Änderungen aktualisiert. Verwenden Sie den folgenden Befehl, um die Änderungen zu pushen:

```
git push origin branch-name
```

### Referenzbild
![Push_image](./images/Readme_images/push.png)

Erstellen Sie eine Pull-Anfrage: Nachdem Sie die Änderungen auf GitHub gepusht haben, sehen Sie beim Neuladen des gegabelten Repositorys die Option zum Erstellen einer Pull-Anfrage. Klicken Sie auf diese Schaltfläche, um eine Pull-Anfrage zu erstellen.

### Referenzbild 
![Pull_Request](./images/Readme_images/pull%20request.png)

Dies führt Sie zu einer Seite, auf der Sie die vorgenommenen Änderungen überprüfen und eine Beschreibung Ihrer Pull-Anfrage geben können.

Achten Sie darauf, eine klare und prägnante Beschreibung der vorgenommenen Änderungen und warum Sie sie vorgenommen haben, einzufügen.

Wenn es irgendwelche Probleme oder Bedenken gibt, von denen der Besitzer des Repositorys wissen sollte, stellen Sie sicher, diese in der Beschreibung der Pull-Anfrage zu erwähnen.

Sobald Sie mit der Beschreibung zufrieden sind, klicken Sie auf die Schaltfläche "Pull-Anfrage erstellen".

### Referenzbild
![Create_pull_request](./images/Readme_images/Create_pull_request.png)

Warten Sie auf Feedback: Nachdem Sie die Pull-Anfrage erstellt haben, wird der Besitzer des Repositorys Ihre Änderungen überprüfen und Feedback geben.

Es kann sein, dass er Sie bittet, weitere Änderungen vorzunehmen, oder er kann Ihre Änderungen in das Originalrepository übernehmen.

Seien Sie geduldig und reagieren Sie während dieses Prozesses, und stellen Sie sicher, auf jedes Feedback oder Bedenken, die der Besitzer des Repositorys äußert, einzugehen.

Aktualisieren Sie Ihr gegabeltes Repository: Wenn der Besitzer des Repositorys Ihre Änderungen in das Originalrepository übernimmt, müssen Sie Ihr gegabeltes Repository aktualisieren, um diese Änderungen zu reflektieren.

Navigieren Sie dazu zu Ihrem gegabelten Repository auf GitHub und klicken Sie auf die Schaltfläche "Upstream abrufen".

Führen Sie dann den folgenden Befehl in Ihrem lokalen Repository aus, um es zu aktualisieren:

```
git pull
```

Das sollte Ihnen eine kurze Vorstellung davon geben, wie Sie Git verwenden können. Natürlich können Sie sich die Lektionen in diesem Repository für ausführlichere Erklärungen ansehen.

## Gute erste Aufgabe

Sie können dieses Projekt als Möglichkeit nutzen, zu Open-Source-Projekten beizutragen. Dies könnte eine **gute erste Aufgabe** sein. Ändern Sie einfach die [CONTRIBUTORS.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md)-Datei so, dass sie zu Ihrem eigenen GitHub-Repository verlinkt ist. Verwenden Sie dabei Markdown, wie in der Datei gezeigt.

Schauen Sie sich bitte das [First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions)-Verzeichnis für eine schrittweise Anleitung an, wie Sie zu diesem Repository beitragen können.

### Inhaltsverzeichnis

- [Teil 00 - Geschichte und Grundlagen](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2000%20-%20Geschichte%20und%20Grundlagen/Part-00-History.md)
- [Teil 01 - Grundlegende Navigation](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2001%20-%20Grundlegende%20Navigation/basicnavigation.md)
- [Teil 02 - Initialisierung von Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2002%20-%20Initialisierung%20von%20Git/getting-started.md)
- [Teil 03 - Branching und Merging](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2003%20-%20Verzweigen%20und%20Zusammenf%C3%BChren/part3.md)
- [Teil 04 - Zusammenarbeit mit Remote-Repositories](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2004%20-%20Zusammenarbeit%20mit%20Remote-Repositories/part4.md)
- [Teil 05 - Fortgeschrittene Git-Konzepte](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2005%20-%20Erweiterte%20Git-Konzepte/part5.md)
- [Teil 06 - CI-CD mit Git und Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2006%20-%20CI-CD%20mit%20Git%20und%20GitHub/part6.md)
- [Teil 07 - Beste Praktiken und Tipps für Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2007%20-%20Git%20Best%20Practices%20und%20Tipps/part7.md)
- [Teil 08 - Git und Github in der agilen Entwicklung](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2008%20-%20Git%20und%20GitHub%20in%20der%20agilen%20Entwicklung/Part-08.md)
- [Teil 09 - Github und Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2009%20-%20GitHub%20und%20Codespaces/Part-09.md)
- [Teil 10 - Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2010%20-%20GitHub%20Actions/Part-10.md)
- [Teil 11 - Fortgeschrittene Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2011%20-%20Erweiterte%20GitHub%20Actions/Part11.md)
- [Teil 12 - Verwendung von Jupyter Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2012%20-%20Verwendung%20von%20Jupyter%20Codespaces%20in%20GitHub/Part12.md)
- [Teil 13 - Verwendung von C# Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2013%20-%20Verwendung%20von%20C%23%20Codespaces%20in%20GitHub/Part-13.md)
- [Teil 14 - Verwendung von React Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2014%20-%20Verwendung%20von%20React%20Codespaces%20in%20GitHub/Part-14.md)
- [Teil 15 - Verwendung von Express Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2015%20-%20Verwendung%20von%20Express%20Codespaces%20in%20GitHub/Part-15.md)
- [Teil 16 - Verwendung von Ruby on Rails Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2016%20-%20Verwendung%20von%20Ruby%20on%20Rails%20Codespaces/Part16.md)
- [Teil 17 - Verwendung von Django Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2017%20-%20Verwendung%20von%20Django%20Codespaces%20in%20GitHub/Part17.md)
- [Teil 18 - Github Projektmanagement-Tools](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2018%20-%20GitHub%20Projektmanagement-Tools/Part-18.md)
- [Teil 19 - Github Projektboards und Notizen](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/de/Teil%2019%20-%20GitHub%20Projektboards%20und%20Notizen/Part-19.md)

### Übersetzungen dieses Tutorials  
Unten findest du Übersetzungen dieses Tutorials in vielen verschiedenen Sprachen. Bitte beachte, dass einige dieser Übersetzungen noch in Arbeit sind und noch nicht vollständig abgeschlossen wurden.  

- Chinesisch (Vereinfacht)  
- Französisch  
- Deutsch  
- Hindi  
- Italienisch  
- Japanisch   
- Mongolisch  
- Russisch  
- Spanisch  
- Türkisch  
