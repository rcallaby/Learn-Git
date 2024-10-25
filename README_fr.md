# Apprendre-Git
C'est ici que vous trouverez un exemple de référentiel pour ma série de tutoriels YouTube sur l'apprentissage de Git et Github.
Si vous avez trouvé ce référentiel utile, pensez à lui attribuer une étoile ⭐, car il sera plus facile pour les autres de le trouver.

De plus, cela m'aiderait beaucoup si vous vous abonnez à ma [chaîne YouTube](https://www.youtube.com/@richardcallaby) car c'est là que je publie des tutoriels gratuits et d'autres ressources éducatives gratuites.

## Voici un tutoriel étape par étape sur la façon de contribuer à GitHub
Créer un compte GitHub : Si vous n'avez pas encore de compte GitHub, vous devrez en créer un. Accédez à github.com et cliquez sur le bouton « S'inscrire » dans le coin supérieur droit. Suivez les instructions pour créer votre compte.

Trouver un référentiel auquel contribuer : Une fois que vous avez un compte GitHub, vous pouvez rechercher les référentiels auxquels vous souhaitez contribuer. Vous pouvez utiliser la barre de recherche GitHub pour rechercher des référentiels par nom ou par mot-clé.

Dupliquer le référentiel : une fois que vous avez trouvé un référentiel auquel vous souhaitez contribuer, vous devez le dupliquer.

Le dupliquage crée une copie du référentiel dans votre propre compte GitHub, que vous pouvez modifier sans affecter le référentiel d'origine.

### Image de référence
Cliquez sur le bouton ci-dessous pour dupliquer le référentiel qui se trouve dans le coin supérieur droit.

![fork_image](./images/Readme_images/fork.png)

Cloner le référentiel dupliqué : après avoir dupliqué le référentiel, vous devez le cloner sur votre machine locale. Le clonage crée une copie du référentiel sur votre ordinateur sur laquelle vous pouvez travailler. Pour cloner le référentiel, ouvrez une fenêtre de terminal et saisissez la commande suivante :

```
git clone https://github.com/your-username/repository-name.git
```
Assurez-vous de remplacer « your-username » et « repository-name » par votre nom d'utilisateur GitHub et le nom du référentiel que vous avez créé.

### Image de référence
![Clone_repo](./images/Readme_images/Clone.png)

Assurez-vous de créer une branche au nom unique pour refléter les modifications que vous souhaitez apporter au code source. Pour créer une branche, utilisez la syntaxe suivante :

```
git branch "branch-name"
```
### Image de référence
![branch_making](./images/Readme_images/Branch_making.png)

Pour activer cette branche, utilisez la syntaxe suivante :
```
git checkout "branch-name"
```
### Image de référence

![branch_switch](./images/Readme_images/branch_switch.png)

Apportez des modifications au code : une fois le référentiel cloné sur votre machine locale, vous pouvez apporter des modifications au code. Utilisez votre éditeur de texte ou IDE préféré pour modifier les fichiers.

Validez les modifications : après avoir apporté des modifications au code, vous devrez les valider dans votre référentiel local. Pour ce faire, ouvrez une fenêtre de terminal et accédez à la racine du référentiel cloné. Utilisez la commande suivante pour mettre en scène les modifications :

```
git add .
```

### Image de référence
![add](./images/Readme_images/add.png)

Cela mettra en scène toutes les modifications apportées aux fichiers dans le référentiel.

Ensuite, validez les modifications à l'aide de la commande suivante :

```
git commit -m "A brief description of the changes made"
```

### Image de référence
![Commit](./images/Readme_images/commit.png)

Veillez à inclure un message bref et informatif décrivant les modifications que vous avez apportées.

Envoyez les modifications à GitHub : après avoir validé les modifications dans votre référentiel local, vous devrez les envoyer à GitHub. Cela mettra à jour la copie du référentiel dans votre compte GitHub avec les modifications que vous avez apportées. Pour envoyer les modifications, utilisez la commande suivante :
```
git push origin branch-name
```

### Image de référence
![Push_image](./images/Readme_images/push.png)

Créer une demande d'extraction : après avoir envoyé les modifications à GitHub, lorsque vous rechargez le dépôt forké, vous verrez l'option permettant de créer une demande d'extraction. Cliquez sur ce bouton pour créer une demande d'extraction.

### Image de référence
![Pull_Request](./images/Readme_images/pull%20request.png)

Cela vous amènera à une page où vous pourrez consulter les modifications que vous avez apportées et fournir une description de votre demande d'extraction.

Assurez-vous d'inclure une description claire et concise des modifications que vous avez apportées et des raisons pour lesquelles vous les avez apportées.

S'il y a des problèmes ou des préoccupations dont le propriétaire du dépôt doit être conscient, assurez-vous de les mentionner dans la description de la demande d'extraction.

Une fois que vous êtes satisfait de la description, cliquez sur le bouton « Créer une demande d'extraction ».

### Image de référence
![Create_pull_request](./images/Readme_images/Create_pull_request.png)

Attendez les commentaires : après avoir créé la demande d'extraction, le propriétaire du référentiel examinera vos modifications et vous fournira ses commentaires.

Il peut vous demander d'apporter des modifications supplémentaires ou de fusionner vos modifications dans le référentiel d'origine.

Soyez patient et réactif pendant ce processus, et assurez-vous de répondre à tous les commentaires ou préoccupations soulevés par le propriétaire du référentiel.

Mettez à jour votre référentiel dupliqué : si le propriétaire du référentiel fusionne vos modifications dans le référentiel d'origine, vous devrez mettre à jour votre référentiel dupliqué pour refléter ces modifications.

Pour ce faire, accédez à votre référentiel dupliqué sur GitHub et cliquez sur le bouton « Récupérer en amont ».

Ensuite, exécutez la commande suivante dans votre référentiel local pour le mettre à jour :

```
git pull
```

Cela devrait vous donner une brève idée de la façon d'utiliser Git. Bien sûr, vous pouvez consulter les leçons que j'ai créées dans ce référentiel pour des explications plus approfondies.

## Bon premier problème

Vous pouvez utiliser ce projet comme un moyen de commencer à contribuer à des projets open source. Cela pourrait être un **bon premier problème**, il suffit de modifier le fichier [CONTRIBUTORS.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) pour qu'il soit lié à votre propre référentiel GitHub. Utilisez Markdown comme indiqué dans le fichier.

Veuillez consulter le répertoire [First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions) pour obtenir des instructions étape par étape sur la façon de contribuer à ce référentiel.
### Table des matières

- [Partie 00 - Historique et fondations](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-00-History-and-Foundations/history-of-git.md)
- [Partie 01 - Navigation de base](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-01-Basic-Navigation/basic-navigation.md)
- [Partie 02 - Initialisation de Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-02-Initializing-Git/getting-started.md)
- [Partie 03 - Branchement et Fusion](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-03-Branching-and-Merging/branching-and-merging.md)
- [Partie 04 - Collaboration avec des référentiels distants](https://github.com/rcallaby/Learn-Git/tree/main/Lessons/en/Part-04-Collaborating-with-Remote-Repositories/collaborating-with-remote-repos.md)
- [Partie 05 - Concepts avancés de Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-05-Advanced-Git-Concepts/advanced-git.md)
- [Partie 06 - CI-CD avec Git et Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-06-CI-CD-with-Git-and-Github/ci-cd-git-github.md)
- [Partie 07 - Bonnes pratiques et astuces Git](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-07-Git-Best-Practices-and-Tips/best-practices-tips.md)
- [Partie 08 - Git et Github dans le développement Agile](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-08-Git-and-Github-in-Agile-Development/git-github-agile-dev.md)
- [Partie 09 - Github et Espaces de code](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-09-Github-and-Codespaces/github-codespaces.md)
- [Partie 10 - Actions Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-10-Github-Actions/github-actions.md)
- [Partie 11 - Actions Github avancées](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-11-Advanced-Github-Actions/advanced-github-actions.md)
- [Partie 12 - Utilisation des espaces de code Jupyter dans Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-12-Using-Jupyter-Codespaces-in-Github/github-jupyter-codespace.md)
- [Partie 13 - Utilisation des espaces de code C# dans Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-13-Using%20Csharp-Codespaces-in-Github/github-Csharp-codespace.md)
- [Partie 14 - Utilisation des espaces de code React dans Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-14-Using-React-Codespaces-in-Github/github-react-codespace.md)
- [Partie 15 - Utilisation des espaces de code Express dans Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-15-Using-Express-Codespaces-in-Github/github-express-codespace.md)
- [Partie 16 - Utilisation des espaces de code Ruby on Rails](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-16-Using-Ruby-on-Rails-Codespaces/github-rubyrails-codespace.md)
- [Partie 17 - Utilisation des espaces de code Django dans Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-17-Using%20Django%20Codespaces-in-Github/github-django-codespace.md)
- [Partie 18 - Outils de gestion de projet Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-18-Github-Project-Management-Tools/github-project-management-tools.md)
- [Partie 19 - Tableaux et notes de projet Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/en/Part-19-Github-Project-Boards-and-Notes/github-project-boards-and-notes.md)

#### Traductions de ce tutoriel
Vous trouverez ci-dessous des traductions de ce tutoriel dans de nombreuses langues différentes. Veuillez garder à l'esprit que certaines de ces traductions sont en cours de réalisation et ne sont pas encore entièrement terminées.

- Chinois (simplifié)
- Français
- Allemand
- Russe
- Espagnol
- Hindi
- Italien
- Mongol
- Japonais
- Malayalam
- turc 
