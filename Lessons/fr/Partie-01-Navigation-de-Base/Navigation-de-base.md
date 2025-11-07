# Git - Navigation de Base

# Introduction:
Le terminal BASH est une interface de ligne de commande puissante qui permet aux utilisateurs de naviguer à travers le système de fichiers de leur ordinateur, d'effectuer diverses tâches et d'interagir avec des systèmes de contrôle de version tels que Git. Git est un système de contrôle de version distribué largement utilisé qui offre une collaboration efficace et le suivi des changements apportés aux dépôts de code. Dans cet article, nous explorerons comment naviguer et utiliser des commandes de base dans le terminal BASH pour travailler efficacement avec Git.

## Ouverture du Terminal BASH:
Pour commencer, ouvrez votre terminal préférée. Sur la plupart des systèmes basés sur Unix, vous pouvez trouver le terminal dans le dossier "Applications" ou "Utilitaires". Une fois lancé, une invite de commande apparaîtra, prête à accepter vos commandes.

## Navigation à travers les Répertoires:

La commande `pwd` signifie "Print Working Directory" et affiche le chemin du répertoire de travail.
```commandline
pwd
```
Cette commande n'a pas d'arguments ou d'options.

La commande `cd` (abrégée de "change directory") est fondamentale pour naviguer dans le système de fichiers. Voici quelques exemples d'utilisation courante de `cd` :

Pour vous déplacer dans un répertoire, utilisez `cd <répertoire>` (remplacez `<répertoire>` par le nom du répertoire désiré), par exemple :
```
cd Documents
```
Pour revenir d'un niveau dans le répertoire, tapez `cd ..`, par exemple :
```
cd ..
```
Pour aller dans votre répertoire personnel, utilisez `cd` ou `cd ~`, par exemple :
```
cd ~
```
Pour revenir au répertoire précédent, utilisez `cd -`, par exemple :
```
cd -
```

## Liste des Contenus du Répertoire:
La commande `ls` est utilisée pour lister le contenu d'un répertoire. Par défaut, elle affiche les fichiers et répertoires dans le répertoire actuel. Quelques indicateurs utiles pour améliorer la fonctionnalité de `ls` :

`ls -l` affiche le contenu sous forme de liste détaillée.
```commandline
ls -l
```
`ls -a` montre les fichiers et répertoires cachés.
```commandline
ls -a
```
`ls -h` fournit des tailles de fichier lisibles par l'homme.
```commandline
ls -h
```
`ls -R` liste les répertoires et leurs contenus de manière récursive.
```commandline
ls -R


## Création et Déplacement de Répertoires:
Vous pouvez créer des répertoires en utilisant la commande `mkdir` suivie du nom du répertoire souhaité :
Pour créer un répertoire à l'emplacement actuel, utilisez `mkdir <répertoire>`. Par exemple :

mkdir cedossier
```
Pour créer des répertoires imbriqués, utilisez `mkdir -p <répertoire_parent>/<répertoire_enfant>`.
```commandline
mkdir -p cedossier/sousdossier
```
Pour supprimer des répertoires, utilisez la commande `rmdir` :
`rmdir <répertoire>` supprime un répertoire vide.
```commandline
rmdir cedossier
```

Déplacement et Renommage de Fichiers et Répertoires :
La commande `mv` vous permet de déplacer et renommer des fichiers et des répertoires :
Pour déplacer un fichier ou un répertoire, utilisez `mv <source> <destination>`. Par exemple :
```commandline
mv cedossier nouveaunomdedossier
```

Pour renommer un fichier ou un répertoire, utilisez `mv <ancien_nom> <nouveau_nom>`.
```commandline
mv vieuxdossier nouveaudossier
```

## Création et Suppression de Fichiers:
Vous pouvez créer un nouveau fichier en utilisant la commande `touch`.
```commandline
touch nouveau_nom_de_fichier
```
Ou dans un répertoire, comme par exemple :
```commandline
touch repertoire/nouveau_nom_de_fichier
```
Maintenant, supprimons un fichier en utilisant la commande `rm`.
```commandline
rm nom_de_fichier
```
Pour supprimer des répertoires et leurs contenus de manière récursive
```commandline
rm -r nom_de_fichier
```
Pour ignorer les fichiers et les arguments qui n'existent pas, sans jamais demander.
```commandline
rm -f nom_de_fichier
```
Pour montrer en mode verbeux tous les fichiers supprimés
```commandline
rm -v nom_de_fichier
```
Pour supprimer tous les fichiers à l'intérieur d'un répertoire.
```commandline
rm *
```
# Conclusion:
Le terminal BASH, associé à Git, offre un environnement robuste pour un contrôle de version efficace et une gestion de fichiers efficace. En vous familiarisant avec des commandes de base telles que `mkdir`, `rmdir`, `rm`, `mv`, `cd`, `ls`, `pwd` et des commandes spécifiques à Git telles que `git init`, `git add`, `git commit`, `git push` et `git pull`, vous pouvez naviguer à travers les répertoires, créer et supprimer des répertoires, déplacer et renommer des fichiers, supprimer des fichiers et gérer efficacement vos dépôts Git. La pratique et l'exploration vous aideront à devenir plus compétent dans l'utilisation de ces commandes, vous permettant d'optimiser votre flux de travail de développement.
