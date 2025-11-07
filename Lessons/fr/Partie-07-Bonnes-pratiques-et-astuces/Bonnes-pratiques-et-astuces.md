# Bonnes pratiques et astuces pour Git

## Gérer un historique de commits propre

Les systèmes de contrôle de version comme Git et les plateformes comme GitHub ont révolutionné la manière dont on gère le développement de logiciels et collabore. Pour utiliser Git et GitHub de manière efficace, un aspect essentiel est de conserver un historique de commits propre et organisé. Un historique de commits bien tenu aide non seulement les développeurs à mieux comprendre l'évolution du projet, mais aide aussi pour le débogage, la revue de code et la collaboration. Dans cet article, nous examinerons les différentes pratiques et techniques pour gérer un historique de commits propre avec Git et GitHub.

### Des commits fréquents et intuitifs
Des commits fréquents et logiques sont la base d'un historique de commits propre. Au lieu de regrouper de nombreuses modifications en un seul commit gigantesque, il vaut mieux faire plusieurs commits plus petits, représentant les différentes divisions logiques du travail.Idéalement, chaque commit devrait concerner un problème, une correction de bug, ou une fonctionnalité spécifique. Cette approche permet de mieux comprendre les modifications, et d'annuler plus facilement les modifications si nécessaire.

### Rédiger des messages de commits descriptifs
Un message de commit bien écrit est essentiel pour comprendre les modifications apportées par ce commit. Évitez les messages génériques comme « Correction de bug » ou « Mise à jour du code ». Visez plutôt une description claire et concise des modifications et de leur raison.

Si vous rédigez votre message de commit en anglais, il doit être écrit à l'impératif, pour être lu comme une commande ou une instruction. Par exemple :
- Bien: «  Add user authentication feature »
- Pas terrible : « Added some stuff and fixed things »

Si vous rédigez votre message de commit en français, utilisez la norme que votre projet a décidé de suivre.
- Exemple: « Ajout d'une fonctionnalité d'authentification des utilisateurs »
- Exemple: « Ajoute une fonctionnalité d'authentification des utilisateurs »
- Exemple: « Ajouter une fonctionnalité d'authentification des utilisateurs »

### Utilisez les branches à bon escient
Avec Git, les branches sont de puissants outils qui permettent de travailler sur des fonctionnalités ou corrections de bugs séparés, sans toucher à la base de code principale. Créez une nouvelle branche pour chaque fonctionnalité ou problème sur lequel vous travaillez. Ainsi, la branche principale (en général appelée « master » ou « main ») continue à être stable et il est possible de l'utiliser comme base pour le projet. Une fois que le travail sur la branche est terminé et testé, fusionnez-la avec la branche principale avec un commit de fusion (merge commit) propre et bien documenté.

### Utilisez Rebase pour garder un historique propre
Git fournit un outil très utile appelé « rebase », qui permet d'intégrer des modifications depuis une branche vers une autre, tout en conservant un historique linéaire. Au lieu de fusionner des branches, ce qui peut créer des commits de fusion (merge commits) inutiles, utilisez Git rebase pour intégrer des modifications depuis la branche principale vers votre branche. Rebase aide à conserver un historique de commits propre et facile à suivre.

### Combinez et éditez les commits avant un push
Avant d'appliquer vos modifications sur un dépôt partagé comme un dépôt GitHub en effectuant un push, vous pouvez nettoyer votre historique de commits en combinant et éditant les commits. Utilisez `git rebase -i` pour lancer un rebase interactif sur votre branche et combiner de nombreux commits en un seul ou pour éditer les messages de commit pour plus de clarté. Combiner des commits permet non seulement de réduire le désordre, mais aussi de s'assurer que chaque commit correspond à une modification cohérente et complète.

### Évitez de faire des push directement sur la branche principale
Dans un environnement collaboratif, il est essentiel d'éviter de faire des push directement sur la branche principale. Utilisez plutôt les pull requests sur des plateformes comme GitHub pour proposer des modifications et les faire vérifier par les membres de votre équipe. Cela permet une approche plus structurée et organisée pour intégrer du nouveau code dans la branche principale tout en gardant un historique de commits propre.

### Utilisez les Git Hooks
Les Git hooks sont des scripts qui peuvent être déclenchés à des moments spécifiques du flux de travail Git. Utilisez des Git hooks pré-commit afin d'assurer que les messages de commit suivent une certaine norme, ou des Git hooks pré-push pour exécuter des tests avant d'effectuer un push du code vers le dépôt distant. Cela aide à maintenir une bonne cohérence et à s'assurer que seules les modifications propres et bien testées soient intégrées par un push.

### Documentez les modifications et mises à jour
En plus de messages de commits clairs, envisagez de tenir un journal de modifications ou des notes de version pour votre projet. Cette documentation peut être inclue dans le fichier README du dépôt, ou dans un fichier dédié. Un journal de modifications donne une vue d'ensemble des modifications apportées par chaque version, ce qui permet aux contributeurs et utilisateurs de comprendre plus facilement ce qui est nouveau et ce qui a été corrigé.

### Maintenance et nettoyage régulier
Au fur et à mesure que le projet évolue, prenez le temps de passer en revue et de nettoyer l'historique de commits régulièrement. Retirez les branches inutiles ou temporaires, supprimez les branches qui ont été fusionnées, et envisagez de faire une rebase ou d'écraser les commits qui sont devenus obsolètes ou qui peuvent prêter à confusion.

Un historique de commits propre avec Git et GitHub est non seulement une bonne pratique, mais c'est aussi un aspect essentiel du développement de logiciels efficace. En créant des commits fréquemment, en rédigeant des messages de commit descriptifs, en utilisant les branches à bon escient, et en tirant profit des fonctionnalités puissantes de Git comme Git rebase et la possibilité de combiner des commits, les développeurs peuvent maintenir un historique de commits organisé et judicieux. De plus, intégrer les Git hooks, documenter les modifications, et s'occuper régulièrement de maintenance aide à assurer que le projet reste bien structuré et collaboratif tout au long de son cycle de vie.

## Utilisez des alias et raccourcis Git

Git est un système de contrôle de version puissant et largement utilisé par les développeurs pour gérer du code source et collaborer sur des projets. Un atout de git est sa flexibilité et sa capacité à être personnalisé, en permettant aux utilisateurs de créer des alias et des raccourcis pour les commandes fréquemment utilisées. Les alias et raccourcis Git permettent d'améliorer sa productivité de manière significative, de réduire le temps passé à taper, et de rendre les commandes Git plus intuitives. Dans cet article, nous examinerons comment mettre en place et utiliser les alias et raccourcis Git pour améliorer votre flux de travail avec Git et GitHub.

### Comprendre les alias Git
Les alias Git sont des raccourcis personnalisés pour des commandes Git. Ils permettent de créer des abréviations plus simples ou même de toutes nouvelles commandes pour des opérations Git complexes ou fréquemment utilisées. Les alias Git sont définis dans le fichier de configuration de Git (.gitconfig), qui est situé soit dans votre répertoire home (~/.gitconfig) soit à la racine du répertoire Git du projet (.git/config). Vous pouvez définir des alias qui s'appliquent à tous les dépôts, ou des alias locaux spécifiques à un projet particulier.

Pour créer un alias Git, vous pouvez utiliser la commande git config ou éditer le fichier .gitconfig directement.

Créer un alias Git global :
Pour créer un alias Git global avec la commande git config, ouvrez un terminal et tapez :
```
git config --global alias.nom_de_l_alias 'commande_d_origine'

```
Remplacez nom_de_l_alias avec l'alias de votre choix, et commande_d_origine avec la commande complète que vous souhaitez raccourcir. Par exemple, pour créer un alias pour git status, vous pouvez utiliser :

```
git config --global alias.st status

```
Créer un alias Git local :
Pour créer un alias Git local pour un projet spécifique, allez à la racine du répertoire du projet dans votre terminal et utilisez la même commande sans --global :

```
git config alias.nom_de_l_alias 'commande_d_origine'

```
### Utiliser des alias Git
Une fois que vous avez mis en place vos alias, vous pouvez les utiliser immédiatement. Tapez simplement l'alias au lieu de la commande complète quand vous effectuez des opérations Git. Par exemple, si vous avez créé l'alias st pour status, vous pouvez maintenant utiliser :

```
git st

```
Cela aura le même effet que si vous aviez tapé git status.

#### Exemples d'alias Git utiles
Voici quelques exemples d'alias Git utiles qui peuvent améliorer votre flux de travail :

```
# Raccourcis pour des commandes fréquentes
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.br branch

# Afficher un historique de commit abrégé
git config --global alias.lg "log --oneline --decorate --all --graph"

# Afficher un output de log plus coloré et plus lisible
git config --global alias.l "log --pretty=format:'%C(auto)%h %Cblue%ad %Creset%s%C(auto)%d %Cgreen[%an]' --date=short"

# Afficher le status actuel du dépôt
git config --global alias.s status

# Afficher l'historique de commits d'un fichier spécifique
git config --global alias.filelog "log -u"

# Annuler le dernier commit mais conserver les modifications
git config --global alias.undo "reset HEAD~1"

# Amender le dernier commit en y ajoutant les modifications marquées
git config --global alias.amend "commit --amend --no-edit"


```
N'hésitez pas à personnaliser cet alias selon vos préférences et votre flux de travail.

### Partager des alias Git
Si vous travaillez en équipe ou sur plusieurs machines, il peut être avantageux de partager vos alias Git. Vous pouvez partager des alias en copiant les lignes pertinentes dans votre fichier .gitconfig et en les ajoutant dans les fichiers .gitconfig de vos coéquipiers ou d'autres machines. Alternativement, vous pouvez utiliser la commande git config pour définir des alias directement sur ces machines.

Pour partager vos alias à d'autres, donnez-leur la commande suivante :

```
git config --global alias.nom_de_l_alias_name 'commande_d_origine'

```
### Utiliser des alias Git avec GitHub
Les alias Git fonctionnent sans accroc avec les dépôts GitHub. Que vous effectuiez un clonage, un push ou un pull depuis un dépôt GitHub, vous pouvez utiliser les alias que vous avez définis comme lorsque vous utilisez des commandes Git ordinaires. Ces alias sont appliqués localement sur votre machine et n'affectent par le dépôt distant hébergé sur GitHub.

Les alias et raccourcis Git sont un outil précieux pour n'importe quel développeur utilisant Git et GitHub. En mettant in place des alias judicieux et intuitifs, vous pouvez améliorer votre productivité de manière significative et rendre les commandes Git plus faciles à se souvenir et à utiliser. Que vous préfériez des abréviations concises pour des commandes courantes, ou des raccourcis personnalisés pour des opérations complexes, les alias Git vous permettent de personnaliser votre flux de travail pour répondre à vos besoins. En utilisant et partageant les alias Git de manière efficace, vous et votre équipe pouvez rationaliser le processus de développement et collaborer de manière plus efficace.

## Ignorer des fichiers et dossiers avec .gitignore

En développement de logiciel, le contrôle de version est essentiel pour gérer les modifications du code source et pour collaborer avec d'autres développeurs de manière efficace. Git, un des systèmes de contrôle de version les plus populaires, permet aux développeurs de suivre des modifications, de créer des branches, et de fusionner du code sans accroc. Cependant, tous les fichiers et dossiers dans un projet ne doivent pas être suivis par Git. Par exemple, il vaut mieux exclure du contrôle de version les artefacts de build, les fichiers temporaires et les données sensibles. Pour cela, Git fournit une solution simple et puissante : le fichier .gitignore. Dans cet article, nous examinerons comment utiliser .gitignore pour empêcher certains fichiers et répertoires d'être suivis par Git.

### Qu'est-ce que .gitignore?
Le fichier .gitignore est un fichier de texte brut qui indique à Git quels fichiers et dossiers doivent être ignorés lors du marquage de modifications. Quand vous ajoutez un fichier ou dossier à la liste de .gitignore, Git va les empêcher d'être suivis, ce qui signifie qu'ils n'apparaîtront pas dans la zone de marquage, et les modifications futures ne seront pas enregistrées dans des commits.

### Créer un fichier .gitignore
Pour commencer, créez un fichier nommé .gitignore à la racine de votre dépôt Git. Vous pouvez utiliser n'importe quel éditeur de texte pour créer ce fichier. Il est important de le nommer exactement .gitignore, sans aucune extension.

Par exemple, en ligne de commande, vous pouvez créer le fichier .gitignore de cette manière :

```
touch .gitignore

```
### Syntaxe de .gitignore
Le fichier .gitignore utilise le filtrage par motifs pour indiquer quels fichiers et dossiers doivent être ignorés. Voici les règles de base de la syntaxe à utiliser :

Les lignes vides et les lignes commençant par # sont considérées comme des commentaires et ignorées par Git.
Pour ignorer un fichier spécifique, écrivez son nom avec son emplacement relatif depuis le répertoire racine du dépôt.
Pour ignorer un dossier, écrivez son nom avec un slash (/) à la fin.

### Utiliser des motifs dans .gitignore
Vous pouvez utiliser divers motifs dans .gitignore pour indiquer plusieurs fichiers ou répertoires à ignorer. Voici quelques motifs fréquents :

Caractères de remplacement (*) : Correspond à n'importe quel nombre de caractères dans le nom d'un fichier ou dossier. Par exemple, *.log ignorera tous les fichiers .log, et build/*/ ignorera tous les répertoires appelés build.

Caractères de remplacement de dossiers (**) : --> Correspond à des dossiers à n'importe quel niveau de l'arborescence. Par exemple, logs/**/*.log ignorera tous les fichiers .log dans n'importe quel sous-dossier de logs.

Négation (!): Renverse une règle établie précédemment. Par exemple, si vous voulez ignorer tous les fichiers .txt sauf un, vous pouvez utiliser *.txt pour ignorer tous les fichiers .txt, puis !important.txt pour conserver le fichier important.txt

### Exemples de .gitignore
Voici des exemples courants d'entrées .gitignore :

```
# Ignore les artefacts de build
build/
dist/
bin/

# Ignore les fichiers de log
*.log

# Ignore les fichiers temporaires
*.tmp
*.temp

# Ignore les fichiers de configuration contenant des données sensibles
config.ini
secrets.json

# Ignore les fichiers d'un répertoire spécifique
data/*

# Ignore les fichiers ayant des extensions spécifiques
*.exe
*.dll


```
Gardez à l'esprit le fait que .gitignore ne s'applique qu'aux fichiers non suivis. Si vous avez déjà suivi un fichier avant de l'ajouter à .gitignore, il va continué à être suivi.

### Fichier .gitignore global
Il est possible que vous ayez des motifs similaires à ignorer dans plusieurs dépôts Git. Au lieu de créer un fichier .gitignore séparément pour chaque dépôt, vous pouvez créer un .gitignore global qui s'appliquera à tous vos dépôts.

Pour cela, créez un fichier .gitignore global dans votre répertoire home et indiquez à Git de l'utiliser. Suivez ces instructions :

Créez le fichier .gitignore global:

```
touch ~/.gitignore_global

```
Ajoutez vos règles dans le fichier en utilisant la même syntaxe que pour un fichier .gitignore classique.

Dites à Git d'utiliser le fichier .gitignore global :

```
git config --global core.excludesfile ~/.gitignore_global

```
L'utilisation de .gitignore est un aspect fondamental pour gérer efficacement un dépôt Git. En ignorant les fichiers et répertoires qui ne doivent pas être suivis, vous pouvez garder votre dépôt propre, éviter d'encombrer votre historique de version avec des modifications non-pertinentes, et éviter que des données sensibles soient accidentellement incluses dans un commit. The fichier .gitignore est un outil puissant qui vous permet d'indiquer quels fichiers et dossiers exclure en utilisant un filtrage par motifs simple. Que vous élaboriez un nouveau projet ou que vous collaboriez dans une équipe, maîtriser l'utilisation de .gitignore améliorera votre flux de travail et contribuera à un processus de développement plus organisé et efficace.

## Flux de travail collaboratif et étiquette de revue de code

La collaboration est au cœur du développement moderne de logiciels, et les systèmes de contrôle de version comme Git, unis aux plateformes comme GitHub, ont révolutionné la manière dont les développeurs travaillent ensemble. Un flux de travail collaboratif efficace et une bonne étiquette de revue de code sont essentiels pour maintenir des bases de code de haute qualité, pour promouvoir une culture d'équipe positive, et pour assurer une intégration fluide de nouvelles fonctionnalités et de corrections de bugs. Dans cet article, nous examinerons les éléments clé du flux de travail collaboratif et de l'étiquette de revue de code avec Git et GitHub.

### Flux de travail collaboratif avec Git
Git offre plusieurs flux de travail collaboratifs, les deux les plus populaires étant le flux de travail centralisé, et le flux de travail par branche.

Flux de travail centralisé:
Avec un flux de travail centralisé, tous les membres de l'équipe travaillent directement sur une branche unique, en général la branche « main » ou « master ». Les développeurs clonent le dépôt, font leurs modifications localement, puis appliquent ces modifications au dépôt centralisé avec un push. Cette approche est simple et appropriée pour des équipes de taille réduite ou pour des projets avec des modifications de code peu fréquentes.

Cependant, un flux de travail centralisé manque d'isolation pour le développement de fonctionnalités, ce qui peut causer des conflits et gêner le développement parallèle.

Flux de travail par branche:
Le flux de travail par branche est plus extensible et est approprié pour des équipes et projets plus larges. Avec cette approche, chaque nouvelle fonctionnalité ou correction de bug est développée sur une branche qui lui est dédiée. Les développeurs créent une nouvelle branche pour une tâche spécifique, travaillent sur ces modifications, puis fusionnent la branche dans la branche principale lorsqu'ils ont terminé.

Le flux de travail par branche fourni de l'isolation pour le développement de fonctionnalités, réduit les conflits, et permet de meilleures pratiques de revue de code. Il encourage les développeurs à travailler de manière indépendante, et permet une meilleure intégration du nouveau code dans la branche principale.

### Étiquette de revue de code
La revue de code est une partie cruciale du processus de développement collaboratif. Elle aide à identifier des bugs, à améliorer la qualité du code, et garantit que de bonnes pratiques soient suivies. Voici quelques conseils essentiels concernant l'étiquette de revue de code :

Soyez respectueux et constructif:
Gardez à l'esprit le fait que la revue de code a pour but d'améliorer le code, pas de critiquer le développeur. Soumettez vos remarques d'une manière respectueuse et constructive. Focalisez-vous sur la qualité du code, sur l'adhésion aux standards, et sur le design global plutôt que sur des préférences personnelles.

Comprenez le contexte:
Essayez de comprendre le contexte de modifications avant de donner votre avis. Familiarisez-vous avec les objectifs de la fonctionnalité ou de la correction de bug, ainsi qu'avec les choix ou les contraintes de design qui sont pertinents.

### Utilisez les outils de revue de code de manière efficace:
Tirez profit des outils de revue de code fournis par GitHub ou d'autres plateformes. Utilisez des commentaires à la fin des lignes de code concernées concernées pour désigner des problèmes précis et suggérer des améliorations. Évitez les commentaires longs et imposants; divisez-les plutôt en points plus petits et concrets.

Abordez à la fois les aspects haut niveau et bas niveau :
Donnez un retour sur les aspects haut niveau comme l'architecture, le design, et l'organisation du code, mais aussi sur les détails bas niveau comme les noms de variables, le format du code, et la gestion des erreurs. Une attention portée sur les deux aspects contribue à une revue de code plus complète.

Évitez de pinailler :
Il est essentiel d'avoir le soucis du détail, mais évitez de pinailler ou de trop vous focaliser sur des problèmes mineurs qui n'ont pas d'impact significatif sur la fonctionnalité du code ou sa maintenabilité.

Fixez des objectifs réalistes en terme de délais :
Prenez en considération l'urgence des modifications et fixez des objectifs réalistes pour les délais de revue. Des modifications plus réduites et moins critiques peuvent nécessiter des délais plus courts, tandis que des modifications plus étendues ou des implémentations de fonctionnalités peuvent demander plus de temps.

Soyez ouvert aux retours
En tant qu'auteur de code, soyez ouvert aux retours. Accueillez les retours comme une opportunité de développement et d'amélioration, et soyez prêt à répondre aux inquiétudes des réviseurs de code.

Utilisez des vérifications et tests automatiques :
Avant d'initier une revue de code, lancez des vérifications et des tests automatisées pour identifier des problèmes courants comme le non-respect de normes de codage et des erreurs basiques. Cela permet de s'assurer que les réviseurs de code peuvent se focaliser sur des aspects de plus haut niveau lors de la revue de code.

### Collaborer sur GitHub
GitHub fournit de nombreuses fonctionnalités pour collaborer qui complètent le flux de travail Git. Certaines fonctionnalités essentielles pour le développement collaboratif incluent :

#### Pull Requests :
Les Pull Requests (PRs) sont la pierre angulaire du flux de travail par branche. Les développeurs créent une pull request lorsqu'ils sont prêts à fusionner leur branche dans la branche principale. Les PR fournissent un aperçu clair des modifications et facilite la revue de code en permettant aux membres de l'équipe de commenter, suggérer des modifications, et discuter du code avant la fusion.

#### Requêtes de revue de code :
Quand vous créez une pull request, demandez à des membres spécifiques de l'équipe de vérifier les modifications. Cela permet de s'assurer que les bonnes personnes soient prévenues et que le processus de revue soit efficace.

#### Vérifications de status et Intégration Continue (CI : Continuous Integration) :
Mettez en place des vérifications de status et CI pour lancer des tests automatiquement lorsque des modifications sont proposées dans une pull request. Cela fournit une garantie supplémentaire avant de fusionner le code dans la branche principale.

#### Étiquettes et jalons :
Utilisez des étiquettes (labels) et jalons (milestones) pour catégoriser et suivre les pull requests. Les étiquettes peuvent indiquer le statut d'une PR (par exemple : « besoin de vérification », « travail en cours »), tandis que les jalons peuvent regrouper des PRs liées pour une sortie de version ou une fonctionnalité spécifique.

Les flux de travail collaboratifs et l'étiquette de revue de code sont des aspects fondamentaux à la réussite du développement de logiciel avec Git et GitHub. En adoptant un flux de travail approprié pour votre équipe, comme le flux de travail par branche, vous pouvez garantir un développement parallèle plus fluide et minimiser les conflits. Une étiquette de revue de code efficace, qui inclus des retours constructifs, une compréhension du contexte, et l'utilisation efficace d'outils de revue de code, promeut une culture d'équipe positive et améliore la qualité du code. Tirer profit des fonctionnalités collaboratives de GitHub comme les pull requests, les vérifications de statut et jalons aide à rationaliser le processus de développement et améliore la collaboration au sein d'une équipe. En intégrant ces bonnes pratiques dans votre flux de travail, vous pouvez obtenir un processus de développement plus organisé, collaboratif et efficace.


