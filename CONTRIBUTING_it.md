# Linee Guida per la Collaborazione
Grazie per considerare di contribuire a Learn-Git! Questo repository è pensato per essere una risorsa per coloro che stanno imparando Git, e le tue contribuzioni possono aiutare a migliorarlo ulteriormente.

Se desideri contribuire a questo repository migliorando il tutorial o potenzialmente traducendolo in un'altra lingua, crea una nuova issue con quell'idea o miglioramento, e se l'idea è abbastanza buona, io o potenzialmente i membri di questo repository la approveremo. A quel punto potrai apportare la modifica e quindi creare una pull request.

## Codice di Condotta
Prima di iniziare, leggi e attieniti al codice di condotta. Vogliamo mantenere una comunità rispettosa e accogliente per tutti i partecipanti.

## Per Iniziare
Ecco i passaggi di base per contribuire a Learn-Git:

- **Fai il fork del repository**

![immagine fork](./images/Readme_images/fork.png)

- **Crea un nuovo branch per le tue modifiche**

```
git branch "nome-branch"
```
### Immagine di Riferimento
![immagine branch](./images/Contributing_images/branch_making.png)

Poi passa a quel branch usando la seguente sintassi:

### Sintassi
```
git checkout "nome-branch"
```

### Immagine di Riferimento
![checkout branch](./images/Contributing_images/checkout_image.png)


- **Apporta le tue modifiche e commettile nel tuo branch**

Utilizza questo comando nel terminale dopo aver apportato qualsiasi modifica o aggiunta
```
git add .
```
Sintassi per commettere quella modifica o aggiunta

```
git commit -m "Breve descrizione delle modifiche apportate"
```

### Immagine di Riferimento
![immagini di commit](./images/Contributing_images/add_commit.png)

- **Pusha le tue modifiche nel tuo fork**
Pusha le modifiche su GitHub: dopo aver commesso le modifiche nel tuo repository locale, dovrai caricarle su GitHub. Questo aggiornerà la copia del repository nel tuo account GitHub con le modifiche apportate. Per fare push delle modifiche, usa il seguente comando:

```
git push origin nome-branch
```
### Immagine di Riferimento
![Push](./images/Contributing_images/push_origin.png)

- **Crea una pull request**

Dopo aver fatto push delle modifiche su GitHub, quando ricarichi il repository forkato, vedrai l'opzione per creare una pull request. Clicca su quel pulsante per creare una pull request.

### Immagine di Riferimento 

![Pull Request](./images/Contributing_images/pull_request.png)

Ciò ti porterà a una pagina in cui puoi rivedere le modifiche apportate e fornire una descrizione della tua pull request.

Assicurati di includere una descrizione chiara e concisa delle modifiche apportate e del motivo per cui le hai fatte.

Se ci sono problemi o preoccupazioni di cui il proprietario del repository dovrebbe essere a conoscenza, assicurati di menzionarli nella descrizione della pull request.

Una volta soddisfatto della descrizione, clicca sul pulsante "Crea pull request".

![Ultima Immagine](./images/Contributing_images/last.png)

Aspetta un feedback: dopo aver creato la pull request, il proprietario del repository rivedrà le tue modifiche e fornirà un feedback.

## Come Contribuire
Accogliamo le contribuzioni nelle seguenti forme:

### Correzioni
Se trovi errori o inaccuratezze nel contenuto esistente, apri una issue e descrivi gli errori o le inesattezze in dettaglio. Se l'accuratezza di questi errori o inesattezze viene verificata, puoi aprire una pull request con queste modifiche. Cerca di essere diligente e collega la issue alla tua pull request. Tieni presente che le preferenze personali in grammatica non costituiscono necessariamente una modifica necessaria.

### Aggiunte
Se hai un'idea per **nuovo contenuto** che pensi sarebbe utile per coloro che stanno imparando Git, **apri prima una issue per discuterne.** Una volta approvata, sentiti libero di creare una pull request con il tuo nuovo contenuto.

### Miglioramenti
Se hai suggerimenti per migliorare il contenuto esistente, **apri prima una issue per discuterne.** Una volta approvato, sentiti libero di creare una pull request con i tuoi miglioramenti.

## Guida allo Stile
Quando contribuisci a Learn-Git, attieniti alla seguente guida allo stile:

- Utilizza un linguaggio chiaro e conciso
- Usa titoli e sottotitoli per suddividere le sezioni
- Utilizza esempi e visualizzazioni per illustrare concetti
- Includi link a risorse pertinenti quando appropriato
- Utilizza la grammatica e l'ortografia dell'inglese americano

# Conclusione
Grazie per dedicare del tempo a contribuire a Learn-Git! Le tue contribuzioni possono aiutare a rendere Git più accessibile a coloro che stanno appena iniziando.