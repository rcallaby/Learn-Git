# Git - Navigazione di Base

- [Introduzione](#introduzione)
- [Apertura del Terminale BASH](#apertura-del-terminale-bash)
- [Navigazione tra le Directory](#navigazione-tra-le-directory)
- [Elencazione dei Contenuti della Directory](#elencazione-dei-contenuti-della-directory)
- [Creazione e Spostamento delle Directory](#creazione-e-spostamento-delle-directory)
- [Creazione e Rimozione dei File](#creazione-e-rimozione-dei-file)
- [Conclusioni](#conclusioni)

# Introduzione:
Il terminale BASH è un potente interfaccia a riga di comando che consente agli utenti di navigare attraverso il sistema di file del proprio computer, svolgere varie attività e interagire con sistemi di controllo versione come Git. Git è un sistema di controllo versione distribuito ampiamente utilizzato che offre una collaborazione efficiente e il tracciamento delle modifiche ai repository di codice. In questo articolo, esploreremo come navigare e utilizzare comandi di base nel terminale BASH per lavorare efficacemente con Git.

## Apertura del Terminale BASH:
Per iniziare, apri l'applicazione del terminale preferita. Sui sistemi basati su Unix, puoi trovare il terminale nella cartella "Applicazioni" o "Utility". Una volta avviato, comparirà un prompt dei comandi, pronto ad accettare i tuoi comandi.

## Navigazione tra le Directory:

Il comando pwd sta per "Print Working Directory" e stampa il percorso della directory di lavoro.
```commandline
pwd
```
Questo comando non ha argomenti o opzioni.

Il comando cd (abbreviazione di "change directory") è fondamentale per navigare nel sistema di file. Ecco alcuni esempi comuni di utilizzo di cd:

Per spostarti in una directory, usa cd <directory> (sostituisci <directory> con il nome della directory desiderata), ad esempio:
```
cd Documenti
```
Per tornare al livello di directory precedente, digita cd .. come segue:
```
cd ..
```
Per andare nella tua directory home, usa cd o cd ~ come segue:
```
cd ~
```
Per tornare alla directory precedente, usa cd - come segue:
```
cd -
```

## Elencazione dei Contenuti della Directory:
Il comando ls viene utilizzato per elencare i contenuti di una directory. Per impostazione predefinita, mostra i file e le directory nella directory corrente. Alcune opzioni utili per migliorare la funzionalità di ls:

ls -l visualizza i contenuti in un formato dettagliato.
```
ls -l
```
ls -a mostra file e directory nascosti.
```
ls -a
```
ls -h fornisce dimensioni dei file leggibili dall'utente.
```
ls -h
```
ls -R elenca le directory e i loro contenuti in modo ricorsivo.
```
ls -R
```

## Creazione e Spostamento delle Directory:
Puoi creare directory usando il comando mkdir seguito dal nome della directory desiderata:
Per creare una directory nella posizione corrente, usa mkdir <directory> come segue:
```
mkdir questadirectory
```
Per creare directory nidificate, utilizza mkdir -p <directory_genitore>/<directory_figlio>.
```
mkdir -p questadirectory/sottodirectory
```
Per rimuovere directory, utilizza il comando rmdir:
rmdir <directory> elimina una directory vuota.
```
rmdir questadirectory
```

Spostamento e Rinomina di File e Directory:
Il comando mv ti consente di spostare e rinominare file e directory:
Per spostare un file o una directory, usa mv <origine> <destinazione>. Ad esempio:
```
mv questadirectory nuovonomecartella
```

Per rinominare un file o una directory, usa mv <vecchionome> <nuovonome>.
```
mv vecchiadirectory nuovadirectory
```

## Creazione e Rimozione dei File:
Puoi creare un nuovo file usando il comando touch.
```commandline
touch nuovonomefile
```
O in una directory, come:
```commandline
touch directory/nuovonomefile
```
Ora vediamo come rimuovere un file usando il comando rm.
```commandline
rm nomefile
```
Per rimuovere directory e i loro contenuti in modo ricorsivo
```commandline
rm -r nomefile
```
Per ignorare file e argomenti inesistenti, senza richiesta di conferma.
```commandline
rm -f nomefile
```
Per verificare cosa viene fatto
```commandline
rm -v nomefile
```
Per rimuovere tutto all'interno di una directory.
```commandline
rm *
```
# Conclusioni:
Il terminale BASH, abbinato a Git, offre un ambiente robusto per un efficiente controllo delle versioni e la gestione dei file. Familiarizzandoti con comandi di base come mkdir, rmdir, rm, mv, cd, ls, pwd, e comandi specifici di Git come git init, git add, git commit, git push e git pull, puoi navigare tra le directory, creare e rimuovere directory, spostare e rinominare file, eliminare file e gestire efficacemente i tuoi repository Git. La pratica e l'esplorazione ti aiuteranno a diventare più competente nell'uso di questi comandi, consentendoti di ottimizzare il tuo flusso di lavoro di sviluppo.