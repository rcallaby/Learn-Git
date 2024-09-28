# Storia e Fondamenti di Git

- [Introduzione](#introduzione)
- [Chi ha creato Git](#chi-ha-creato-git)
- [La ragione per cui è stato creato Git](#la-ragione-per-cui-è-stato-creato-git)
- [Alternative a Git](#alternative-a-git)
- [Dove archiviare gratuitamente i tuoi repository](#dove-archiviare-gratuitamente-i-tuoi-repository)

# Introduzione

Git è un sistema di controllo versione distribuito creato da Linus Torvalds nel 2005. Git rappresenta la storia in modo fondamentalmente diverso dai sistemi di controllo versione centralizzati (CVCS) come Team Foundation Version Control, Perforce o Subversion. I sistemi centralizzati archiviano una storia separata per ogni file in un repository. Git archivia la storia come un grafico di istantanee dell'intero repository. Queste istantanee, chiamate commit in Git, possono avere più genitori, creando una storia che assomiglia a un grafico invece di una linea retta. Questa differenza nella storia è incredibilmente importante ed è la principale ragione per cui gli utenti familiari con CVCS trovano Git confuso.

È importante imparare Git oggi perché è ampiamente utilizzato da sviluppatori e aziende in tutto il mondo. È uno strumento essenziale per gestire le modifiche al codice e collaborare con altri sviluppatori su progetti. Git consente agli sviluppatori di lavorare sul codice in modo indipendente e quindi unire le loro modifiche quando sono pronti.

## Chi ha creato Git

Git è stato originariamente sviluppato da Linus Torvalds nel 2005 per lo sviluppo del kernel Linux. Da allora, altri sviluppatori del kernel hanno contribuito al suo sviluppo iniziale. Junio Hamano è stato il principale responsabile dal 2005.

## La ragione per cui è stato creato Git

Il team originale non poteva più utilizzare BitKeeper, un precedente sistema di controllo versione, dopo aver perso la licenza gratuita per usarlo. In quel momento, nessun altro sistema di Gestione del Controllo delle Fonti (SCMs) soddisfaceva i loro requisiti specifici per un sistema distribuito. Alcuni degli obiettivi del nuovo sistema erano la velocità, un design semplice, un forte supporto per lo sviluppo non lineare (migliaia di rami paralleli), completamente distribuito e in grado di gestire progetti di grandi dimensioni come il kernel Linux in modo efficiente (velocità e dimensioni dei dati).

## Alternative a Git

Ci sono diverse alternative a Git, tra cui Subversion (SVN), Mercurial (Hg) e Perforce.

Subversion è un sistema di controllo versione centralizzato simile a CVS. Viene spesso utilizzato in ambienti aziendali perché è facile da usare e si integra bene con altri strumenti.

Mercurial è un sistema di controllo versione distribuito simile a Git. Viene spesso utilizzato in progetti più piccoli perché è più facile da imparare rispetto a Git.

Perforce è un sistema di controllo versione centralizzato spesso utilizzato in ambienti aziendali. Ha un buon supporto per file di grandi dimensioni e file binari.

Ognuno di questi sistemi ha punti di forza e debolezze, e la scelta di quale utilizzare dipende dalle esigenze specifiche del progetto. Git è ampiamente utilizzato da sviluppatori e aziende in tutto il mondo perché è uno strumento essenziale per gestire le modifiche al codice e collaborare con altri sviluppatori su progetti. Git consente agli sviluppatori di lavorare sul codice in modo indipendente e quindi unire le loro modifiche quando sono pronti.

## Dove archiviare gratuitamente i tuoi repository

Ci sono diversi posti gratuiti su Internet dove puoi archiviare i tuoi repository Git. Ecco alcuni dei più popolari:

- GitHub
- GitLab
- Bitbucket
- SourceForge

Ciascuno di questi servizi ha punti di forza e debolezze, e la scelta di quale utilizzare dipende dalle esigenze specifiche del progetto. GitHub è il servizio più popolare ed è ampiamente utilizzato da sviluppatori e aziende in tutto il mondo. Offre repository pubblici illimitati e un numero limitato di repository privati gratuitamente.

GitLab è un altro servizio popolare che offre repository privati illimitati gratuitamente. Bitbucket è un servizio spesso utilizzato da piccoli team perché offre repository privati illimitati gratuitamente per un massimo di cinque utenti. SourceForge è un servizio che esiste da molto tempo ed è spesso utilizzato per progetti open source.