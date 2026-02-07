# Impara-Git

Questo è dove troverai un repository di esempio per la mia serie di tutorial su YouTube su come imparare Git e Github.
Se hai trovato utile questo repository, considera di dargli una stella ⭐ in modo che sia più facile per gli altri trovarlo.

Inoltre, mi aiuteresti molto iscrivendoti al mio [canale YouTube](https://www.youtube.com/@richardcallaby), poiché è il luogo in cui pubblico tutorial gratuiti e altri materiali educativi gratuiti.

## Ecco un tutorial passo dopo passo su come contribuire a GitHub
Crea un account GitHub: Se non hai già un account GitHub, dovrai crearne uno. Vai su github.com e clicca sul pulsante "Iscriviti" nell'angolo in alto a destra. Segui le istruzioni per creare il tuo account.

Trova un repository a cui contribuire: Una volta che hai un account GitHub, puoi cercare i repository a cui sei interessato a contribuire. Puoi utilizzare la barra di ricerca di GitHub per cercare i repository per nome o parola chiave.

Forka il repository: Una volta trovato un repository a cui vuoi contribuire, dovrai forkarlo.

Forkare crea una copia del repository nel tuo account GitHub, che puoi modificare senza influire sul repository originale.

### Immagine di riferimento
Clicca sul pulsante sottostante per forkare il repository, che si trova in alto a destra.

![fork_image](./images/Readme_images/fork.png)

Clona il repository forkato: Dopo aver forkato il repository, dovrai clonarlo sul tuo computer locale. Clonare crea una copia del repository sul tuo computer su cui puoi lavorare. Per clonare il repository, apri una finestra del terminale e inserisci il seguente comando:

```bash
git clone https://github.com/tuo-nomeutente/nome-repository.git
```
Assicurati di sostituire "tuo-nomeutente" e "nome-repository" con il tuo nome utente GitHub e il nome del repository che hai forkato.

### Immagine di riferimento
![Clone_repo](./images/Readme_images/Clone.png)

Assicurati di creare un branch con un nome univoco per riflettere le modifiche che desideri apportare al codice sorgente. Per creare un branch, utilizza la seguente sintassi:

```bash
git branch "nome-branch"
```
### Immagine di riferimento
![branch_making](./images/Readme_images/Branch_making.png)

Per passare a quel branch, utilizza la seguente sintassi:
```bash
git checkout "nome-branch"
```
### Immagine di riferimento
![branch_switch](./images/Readme_images/branch_switch.png)

Apporta modifiche al codice: Una volta che hai clonato il repository sul tuo computer locale, puoi apportare modifiche al codice. Usa il tuo editor di testo o IDE preferito per modificare i file.

Fai il commit delle modifiche: Dopo aver apportato modifiche al codice, dovrai fare il commit nel tuo repository locale. Per farlo, apri una finestra del terminale e naviga nella radice del repository clonato. Utilizza il seguente comando per mettere in stage le modifiche:

```bash
git add .
```

### Immagine di riferimento
![add](./images/Readme_images/add.png)

Questo metterà in stage tutte le modifiche apportate ai file nel repository.

Successivamente, esegui il commit delle modifiche utilizzando il seguente comando:

```bash
git commit -m "Breve descrizione delle modifiche apportate"
```

### Immagine di riferimento
![Commit](./images/Readme_images/commit.png)

Assicurati di includere un breve messaggio informativo che descrive le modifiche apportate.

Esegui il push delle modifiche su GitHub: Dopo aver eseguito il commit delle modifiche nel tuo repository locale, dovrai eseguire il push su GitHub. Questo aggiornerà la copia del repository nel tuo account GitHub con le modifiche apportate. Per eseguire il push delle modifiche, utilizza il seguente comando:

```bash
git push origin nome-branch
```

### Immagine di riferimento
![Push_image](./images/Readme_images/push.png)

Crea una pull request: Dopo aver eseguito il push delle modifiche su GitHub, quando ricarichi il repository forkato, vedrai l'opzione per creare una pull request. Clicca su quel pulsante per creare una pull request.

### Immagine di riferimento
![Pull_Request](./images/Readme_images/pull%20request.png)

Questo ti porterà a una pagina dove potrai rivedere le modifiche apportate e fornire una descrizione della tua pull request.

Assicurati di includere una descrizione chiara e concisa delle modifiche apportate e del motivo per cui le hai apportate.

Se ci sono problemi o preoccupazioni di cui il proprietario del repository dovrebbe essere a conoscenza, assicurati di menzionarli nella descrizione della pull request.

Una volta soddisfatto della descrizione, clicca sul pulsante "Crea pull request".

### Immagine di riferimento
![Create_pull_request](./images/Readme_images/Create_pull_request.png)

Aspetta il feedback: Dopo aver creato la pull request, il proprietario del repository rivedrà le tue modifiche e fornirà un feedback.

Potrebbero chiederti di apportare ulteriori modifiche, o potrebbero incorporare le tue modifiche nel repository originale.

Sii paziente e responsivo durante questo processo, e assicurati di affrontare qualsiasi feedback o preoccupazione sollevata dal proprietario del repository.

Aggiorna il tuo repository forkato: Se il proprietario del repository incorpora le tue modifiche nel repository originale, dovrai aggiornare il tuo repository forkato per riflettere tali modifiche.

Per farlo, vai al tuo repository forkato su GitHub e clicca sul pulsante "Fetch upstream".

Quindi, esegui il seguente comando nel tuo repository locale per aggiornarlo:

```bash
git pull
```

Questo dovrebbe darti una breve idea di come utilizzare Git; naturalmente, puoi consultare le lezioni che ho creato in questo repository per spiegazioni più approfondite.

## Buon primo problema

Puoi utilizzare questo progetto come modo per iniziare a contribuire a progetti open source. Questo potrebbe essere un **buon primo problema**: modifica il file [CONTRIBUTORS.md] (https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) in modo che punti al tuo repository GitHub. Usa il markdown come mostrato nel file.

Per favore, guarda la directory [First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions) per istruzioni passo dopo passo su come contribuire a questo repository.

### Tabella dei contenuti

- [Parte 00 - Storia e Fondamenti](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-00-Storia%20e%20Fondamenti/storia%20di%20git.md)
- [Parte 01 - Navigazione di Base](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-01-Navigazione%20di%20Base/navigazione%20di%20base.md)
- [Parte 02 - Inizializzazione di Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-02-Inizializzazione%20di%20Git/per%20iniziare.md)
- [Parte 03 - Branching e Merging](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-03-Creazione%20di%20Rami%20e%20Unione%20(Branching%20e%20Merging)/branching-e-merging.md)
- [Parte 04 - Collaborazione con Repository Remoti](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-04-Collaborazione%20con%20i%20Repository%20Remoti/collaborazione%20con%20repository%20remoti.md)
- [Parte 05 - Concetti Avanzati di Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-05-Concetti%20Avanzati%20di%20Git/git-avanzato.md)
- [Parte 06 - CI-CD con Git e Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-06-CI-CD%20con%20Git%20e%20Github/ci-cd-git-GitHub.md)
- [Parte 07 - Migliori Pratiche e Suggerimenti di Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-07-Migliori%20Pratiche%20e%20Consigli%20per%20Git/migliori-pratiche.md)
- [Parte 08 - Git e Github nello Sviluppo Agile](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-08-Git%20e%20Github%20nello%20Sviluppo%20Agile/git-GitHub-sviluppo-agile.md)
- [Parte 09 - Github e Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-09-Github%20e%20Codespaces/GitHub-codespaces.md)
- [Parte 10 - Azioni di Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-10-Github%20Actions/GitHub-actions.md)
- [Parte 11 - Azioni Avanzate di Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-11-Github%20Actions%20Avanzati/GitHub-actions-avanzate.md)
- [Parte 12 - Uso di Jupyter Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-12-Utilizzo%20di%20Jupyter%20Codespaces%20in%20Github/GitHub-Juypter-codespace.md)
- [Parte 13 - Uso di C# Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-13-Utilizzo%20di%20C%23%20Codespaces%20in%20Github/GitHub%20CSharp%20codespace.md)
- [Parte 14 - Uso di React Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-14-Utilizzo%20di%20React%20Codespaces%20in%20Github/GitHub-react-codespace.md)
- [Parte 15 - Uso di Express Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-15-Utilizzo%20di%20Express%20Codespaces%20in%20Github/GitHub-express-codespace.md)
- [Parte 16 - Uso di Ruby on Rails Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-16-Utilizzo%20di%20Ruby%20on%20Rails%20Codespaces%20in%20Github/GitHub-rubyrails-codespaces.md)
- [Parte 17 - Uso di Django Codespaces in Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-17-Utilizzo%20di%20Django%20Codespaces%20in%20Github/GitHub-Django-codespace.md)
- [Parte 18 - Strumenti di Gestione Progetti Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-18-Strumenti%20di%20Gestione%20dei%20Progetti%20su%20Github/strumenti-di-gestione-dei-progetti-GitHub.md)
- [Parte 19 - Schede e Note di Progetto Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/IT/Part-19-Bacheche%20e%20Note%20dei%20Progetti%20su%20Github/bacheche-di-progetto-e-note-GitHub.md)

### Traduzioni di questo tutorial  
Puoi trovare le traduzioni di questo tutorial in molte lingue diverse qui sotto. Tieni presente che alcune di queste traduzioni sono ancora in fase di sviluppo e non sono state completamente completate.  

- Inglese
- Cinese (Semplificato)  
- Francese  
- Tedesco  
- Hindi  
- Italiano  
- Giapponese  
- Mongolo  
- Russo  
- Spagnolo  
- Turco  