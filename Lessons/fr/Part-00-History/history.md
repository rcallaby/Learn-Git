# Histoire et Fondements de Git

- [Introduction](#introduction)
- [Qui a créé Git](#qui-a-créé-git)
- [La raison pour laquelle Git a été créé](#la-raison-pour-laquelle-git-a-été-créé)
- [Alternatives à Git](#alternatives-à-git)
- [Où stocker vos dépôts gratuitement](#où-stocker-vos-dépôts-gratuitement)

# Introduction

Git est un système de contrôle de version distribué créé par Linus Torvalds en 2005. Git représente l'histoire d'une manière fondamentalement différente des systèmes de contrôle de version centralisés (CVCS) tels que Team Foundation Version Control, Perforce ou Subversion. Les systèmes centralisés stockent une histoire distincte pour chaque fichier dans un référentiel. Git stocke l'histoire comme un graphe de clichés de l'ensemble du référentiel. Ces clichés, appelés commits dans Git, peuvent avoir plusieurs parents, créant ainsi une histoire qui ressemble à un graphe plutôt qu'à une ligne droite. Cette différence dans l'histoire est extrêmement importante et est la principale raison pour laquelle les utilisateurs familiarisés avec les CVCS trouvent Git déroutant.

Il est important d'apprendre Git aujourd'hui car il est largement utilisé par les développeurs et les entreprises du monde entier. C'est un outil essentiel pour gérer les changements de code et collaborer avec d'autres développeurs sur des projets. Git permet aux développeurs de travailler indépendamment sur du code, puis de fusionner leurs modifications lorsqu'ils sont prêts.

## Qui a créé Git?

Git a été initialement créé par Linus Torvalds en 2005 pour le développement du noyau Linux. Depuis lors, d'autres développeurs du noyau ont contribué à son développement initial. Junio Hamano est le mainteneur principal depuis 2005.

## La Raison pour laquelle Git a été créé

L'équipe d'origine ne pouvait plus utiliser BitKeeper, un système de contrôle de version précédent, après avoir perdu leur licence gratuite pour l'utiliser. À l'époque, aucun autre Système de Gestion de Contrôle de Source (SCM) ne répondait à leurs exigences spécifiques pour un système distribué. Certains des objectifs du nouveau système étaient la rapidité, un design simple, un support fort pour le développement non linéaire (des milliers de branches parallèles), une distribution complète et la capacité à gérer efficacement des projets volumineux comme le noyau Linux (vitesse et taille des données).

## Alternatives à Git

Il existe plusieurs alternatives à Git, telles que Subversion (SVN), Mercurial (Hg) et Perforce.

Subversion est un système de contrôle de version centralisé similaire à CVS. Il est souvent utilisé dans les environnements d'entreprise car il est facile à utiliser et s'intègre bien avec d'autres outils.

Mercurial est un système de contrôle de version distribué similaire à Git. Il est souvent utilisé dans des projets plus petits car il est plus facile à apprendre que Git.

Perforce est un système de contrôle de version centralisé souvent utilisé dans les environnements d'entreprise. Il offre une bonne prise en charge des fichiers volumineux et des fichiers binaires.

Chacun de ces systèmes a ses propres forces et faiblesses, et le choix de celui à utiliser dépend des besoins spécifiques du projet. Git est largement utilisé par les développeurs et les entreprises du monde entier car il est un outil essentiel pour gérer les changements de code et collaborer avec d'autres développeurs sur des projets. Git permet aux développeurs de travailler de manière indépendante sur le code, puis de fusionner leurs modifications lorsqu'ils sont prêts.

## Où stocker vos dépôts gratuitement

Il existe plusieurs endroits gratuits sur Internet où vous pouvez stocker vos dépôts Git. Voici quelques-uns des plus populaires :

- GitHub
- GitLab
- Bitbucket
- SourceForge

Chacun de ces services a ses propres forces et faiblesses, et le choix de celui à utiliser dépend des besoins spécifiques du projet. GitHub est le service le plus populaire et est largement utilisé par les développeurs et les entreprises du monde entier. Il offre des dépôts publics illimités et un nombre limité de dépôts privés gratuitement.

GitLab est un autre service populaire qui offre des dépôts privés illimités gratuitement. Bitbucket est souvent utilisé par de petites équipes car il offre des dépôts privés illimités gratuitement pour jusqu'à cinq utilisateurs. SourceForge est un service qui existe depuis longtemps et est souvent utilisé pour des projets open source.