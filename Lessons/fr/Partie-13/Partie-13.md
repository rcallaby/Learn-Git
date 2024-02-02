## Table des matières

- [Utilisation de C# Codespaces dans Github](#utilisation-de-c-codespaces-dans-github)
    - [Prérequis](#prérequis)
    - [Travailler avec C# Codespaces](#travailler-avec-c-codespaces)
    - [Développement collaboratif avec Codespaces](#développement-collaboratif-avec-codespaces)
- [Utilisation de Github Actions dans C# Codespaces](#utilisation-de-github-actions-dans-c-codespaces)
    - [Créer un fichier de configuration Codespace :](#créer-un-fichier-de-configuration-codespace)

# Utilisation de C# Codespaces dans Github

GitHub Codespaces est un environnement de développement basé sur le cloud qui permet aux développeurs d'écrire, de construire, de tester et de déboguer du code directement dans le référentiel GitHub. Il offre un moyen puissant et pratique de collaborer avec les membres de l'équipe et de travailler sur des projets sans avoir besoin d'une configuration complexe. Avec Codespaces, vous pouvez accéder à un environnement de développement entièrement configuré directement depuis votre navigateur, facilitant ainsi le travail sur votre code de n'importe où.

Dans cet article, nous explorerons comment configurer et utiliser C# Codespaces dans GitHub, vous permettant de développer des projets C# sans effort. Nous plongerons également dans des exemples pour illustrer l'utilisation pratique de Codespaces dans le développement C#.

### Prérequis

Avant de commencer avec C# Codespaces, assurez-vous de disposer des éléments suivants :

Un compte GitHub : Vous avez besoin d'un compte sur GitHub pour créer et utiliser des Codespaces.
Un projet C# : Préparez un projet C# sur lequel vous souhaitez travailler avec Codespaces. Vous pouvez soit créer un nouveau projet, soit utiliser un projet existant.
Création d'un Codespace C#

Accédez à votre référentiel GitHub : Tout d'abord, rendez-vous dans le référentiel où votre projet C# est hébergé.

Cliquez sur le bouton "Code" : Sur la page principale du référentiel, cliquez sur le bouton "Code" vert pour révéler un menu déroulant.

Sélectionnez "Ouvrir avec Codespaces" : Dans le menu déroulant, choisissez "Ouvrir avec Codespaces". Si vous n'avez pas encore utilisé Codespaces dans ce référentiel, il vous demandera de configurer un fichier de configuration Codespace.

Configurez votre Codespace (si applicable) : Si vous configurez Codespaces pour la première fois dans ce référentiel, il vous demandera de créer un dossier .devcontainer avec un fichier de configuration devcontainer.json. Ce fichier spécifie les paramètres de l'environnement de développement, y compris le runtime, les extensions et autres dépendances.

Voici un exemple de fichier devcontainer.json pour un projet C# :
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
Dans cet exemple, nous utilisons l'image officielle .NET SDK 5.0 et installons l'extension C#.

### Travailler avec C# Codespaces

Une fois votre Codespace configuré, vous pouvez y accéder en cliquant sur l'onglet "Codespaces" dans votre référentiel GitHub. Choisissez le Codespace approprié dans la liste et cliquez sur "Connecter" pour lancer l'environnement de développement dans votre navigateur.

Vous serez accueilli par une interface familière de Visual Studio Code, préconfigurée avec tous les outils nécessaires pour développer des applications C#.

Exemple : Création d'une application console C#

Marchons à travers un exemple de création d'une simple application console C# à l'aide de Codespaces.

Connectez-vous au Codespace : Suivez les étapes décrites ci-dessus pour créer et vous connecter à votre Codespace.

Ouvrez un terminal : Cliquez sur le menu "Terminal" dans Visual Studio Code et sélectionnez "Nouveau terminal" pour ouvrir une nouvelle fenêtre de terminal.

Créez une nouvelle application console C# : Dans le terminal, utilisez les commandes suivantes pour créer une nouvelle application console C#.
```
dotnet new console -n MyConsoleApp
cd MyConsoleApp
```
Écrivez du code : Ouvrez le fichier Program.cs et écrivez du code dans la méthode Main.
```
using System;

namespace MyConsoleApp
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Bonjour, Codespaces !");
        }
    }
}
```
Compilez et exécutez l'application : Utilisez les commandes suivantes pour compiler et exécuter l'application console C#.
```
dotnet build
dotnet run
```
Vous devriez voir la sortie : "Bonjour, Codespaces !" affichée dans le terminal.

### Développement collaboratif avec Codespaces

Un des avantages significatifs de Codespaces est son support pour le développement collaboratif. Plusieurs membres de l'équipe peuvent travailler sur le même projet simultanément, chacun dans son propre Codespace. Cela évite les conflits et simplifie le processus de révision et de fusion des modifications de code.

Lorsque vous travaillez en collaboration, chaque développeur peut créer sa propre branche, apporter des modifications et soumettre des demandes de fusion comme d'habitude. Les examinateurs peuvent également tester les modifications en lançant les Codespaces associés à ces demandes de fusion, rendant le processus de révision plus efficace.

GitHub Codespaces offre une excellente plateforme aux développeurs C# pour travailler de manière collaborative et efficace. Avec son environnement de développement basé sur le cloud et sa configuration facile, vous pouvez vous concentrer sur l'écriture de code sans vous soucier de l'infrastructure sous-jacente. Que vous travailliez sur des projets personnels ou contribuiez à des référentiels open-source, C# Codespaces rationalise votre processus de développement et favorise la collaboration entre les membres de l'équipe.

# Utilisation de Github Actions dans C# Codespaces

### Créer un fichier de configuration Codespace : 

Tout d'abord, vous aurez besoin d'un fichier .devcontainer/devcontainer.json pour configurer votre environnement Codespace. Voici un exemple :
```
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:6.0",
  "extensions":

 [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [80]
}
```
Cette configuration utilise l'image .NET SDK 6.0 et installe l'extension C# pour Visual Studio Code.

Créer un fichier Workflow YAML : Ensuite, créez un fichier .github/workflows/build.yml pour définir votre flux de travail GitHub Actions :
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
    - name: Checkout code
      uses: actions/checkout@v2

    - name: Configuration de .NET
      uses: actions/setup-dotnet@v2
      with:
        dotnet-version: '6.0.x'

    - name: Restaurer les dépendances
      run: dotnet restore

    - name: Construire
      run: dotnet build --configuration Release

    - name: Exécuter les tests
      run: dotnet test --configuration Release --no-build
```
Ce flux de travail est déclenché lors des poussées vers la branche principale. Il configure le SDK .NET, restaure les dépendances, construit le projet en configuration Release et exécute les tests.

Commit et Push : Committez les dossiers .devcontainer et .github ainsi que vos fichiers de projet C# dans votre référentiel GitHub.

Exécution de GitHub Actions : Lorsque vous poussez des modifications vers la branche principale, le flux de travail GitHub Actions défini dans le fichier build.yml s'exécutera automatiquement. Vous pouvez vérifier la progression et les résultats du flux de travail dans l'onglet "Actions" de votre référentiel GitHub.

N'oubliez pas que ces exemples sont assez basiques. En fonction de la complexité et des exigences de votre projet, vous pouvez personnaliser davantage le flux de travail en ajoutant des étapes pour le déploiement, les tests d'intégration, l'analyse de code, et plus encore.

Assurez-vous d'adapter ces exemples pour correspondre à la structure et aux exigences de votre projet.