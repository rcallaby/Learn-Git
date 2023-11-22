# Initialiser Git - Bien débuter

- [Commandes Git de base](#commandes-git-de-base)
- [Mettre en place un repository sur Linux](#mettre-en-place-un-repository-sur-Linux)
- [Mettre en place un repository sur Windows](#mettre-en-place-un-repository-sur-Windows)
- [Setting up a Git Repository in Mac](#setting-up-a-git-repository-on-macos)

## Commandes Git de base:
Git fournit une large gamme de commandes pour le contrôle de version. Voici quelques commandes fondamentales :

git init initialise un nouveau dépot Git (aussi appellé repository en anglais) dans le dossier courant. Par exemple :
```
git init nomdudossier
```
git clone <repository_url> copie un repository distant sur votre ordinateur en local. Par exemple :

```
git clone urldurepo
```
git add <file> met en forme les changments faits dans un fichier pour un commit.
```
git add . 
```
Pour ajouter tous les fichiers ou
```
git add nomdufichier
```
git commit -m "<commit_message>" commits les changements sur le repo. Par exemple :
```
git commit -m "un message de description"
```

git push upload les commit et les changements sur le répo distant.
```
git push 
```
git pull va chercher et les combine (merge) depuis un repo distant sur votre repo local.
```
git pull
```

En dessous, vous trouverez un tutoriel étape par étape sur comment setup Git sur Linux, Windows et Mac.

## Mettre en place un repository sur Linux:

Ouvrez une fenetre de terminal.

Naviguer vers le dossier où vous désirez créer le repository en utilisant la commande cd. Par exemple, pour naviguer vers le dossier ~/Documents, utilisez la commande suivante :

```
cd ~/Documents
```
Initialisez votre dépot Git en utilisant la commande git init:

```
git init
```

Votre repository est maintenant fonctionnel. Vous pouvez commencer à y ajouter des fichiers, commit des
changements et utilisez les autres commandes de Git.

## Mettre en place un repository sur Windows:

Installez Git sur votre system Windows en téléchargeant sur le site officiel: https://git-scm.com/download/win. Lancez l'exécutable d'installation et suivez les étapes d'installation.

Ouvrez Git Bash, qui fournit un environnement de ligne de commande similaire à Linux sur Windows.

Naviguez jusqu'au répertoire où vous souhaitez créer votre dépôt. Par exemple, pour accéder au répertoire Documents sur votre disque C:, utilisez la commande suivante :

```
cd /c/Documents
```
Initialisez votre dépot Git en utilisant la commande git init:

```
git init
```
Votre repository est maintenant fonctionnel. Vous pouvez commencer à y ajouter des fichiers, commit des
changements et utilisez les autres commandes de Git.

## Setting up a Git Repository on macOS:

Ouvrez le Terminal sur votre Mac.

Naviguez jusqu'au répertoire où vous souhaitez créer votre dépôt. Par exemple, pour accéder au répertoire Documents, utilisez la commande suivante :

```
cd ~/Documents
```
Initialisez votre dépot Git en utilisant la commande git init:

```
git init
```
Votre repository est maintenant fonctionnel. Vous pouvez commencer à y ajouter des fichiers, commit des
changements et utilisez les autres commandes de Git.

Maintenant que vous avez configuré le dépôt Git, vous pouvez procéder à l'ajout de fichiers, à la réalisation de commits et à l'exécution d'autres opérations Git à l'aide de commandes telles que git add, git commit, git push, etc. N'oubliez pas de consulter la documentation Git ou d'autres tutoriels Git pour plus de détails sur ces opérations.

**Note: Les étapes fournies supposent une configuration de base pour un dépôt Git local. Si vous souhaitez configurer un dépôt distant ou travailler avec des dépôts existants sur des plateformes d'hébergement telles que GitHub ou GitLab, des étapes supplémentaires sont nécessaires.** 