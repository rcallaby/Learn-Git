# Geschichte und Grundlagen von Git

# Einführung

Git ist ein verteiltes Versionskontrollsystem, das von Linus Torvalds im Jahr 2005 erstellt wurde. Git stellt die Historie auf eine grundlegend andere Weise dar als zentrale Versionskontrollsysteme (CVCS) wie Team Foundation Version Control, Perforce oder Subversion. Zentrale Systeme speichern eine separate Historie für jede Datei in einem Repository. Git speichert die Historie als Graph von Snapshots des gesamten Repositories. Diese Snapshots, in Git als Commits bezeichnet, können mehrere Eltern haben und erzeugen so eine Historie, die wie ein Graph und nicht wie eine gerade Linie aussieht. Dieser Unterschied in der Historie ist äußerst wichtig und der Hauptgrund, warum Benutzer, die mit CVCS vertraut sind, Git als verwirrend empfinden.

Es ist heute wichtig, Git zu lernen, da es von Entwicklern und Unternehmen auf der ganzen Welt weit verbreitet ist. Es ist ein unverzichtbares Werkzeug für das Verwalten von Codeänderungen und die Zusammenarbeit mit anderen Entwicklern an Projekten. Git ermöglicht es Entwicklern, unabhängig an Code zu arbeiten und dann ihre Änderungen zusammenzuführen, wenn sie bereit sind.

## Wer hat Git erstellt?

Git wurde ursprünglich von Linus Torvalds im Jahr 2005 für die Entwicklung des Linux-Kernels erstellt. Seitdem haben andere Kernel-Entwickler zu seiner anfänglichen Entwicklung beigetragen. Junio Hamano ist seit 2005 der Kernwartungsperson.

## Der Grund, warum Git erstellt wurde

Das ursprüngliche Team konnte BitKeeper, ein vorheriges Versionskontrollsystem, nicht mehr verwenden, nachdem sie ihre kostenlose Lizenz dafür verloren hatten. Zu der Zeit erfüllten keine anderen Source Control Management (SCMs) ihre speziellen Anforderungen für ein verteiltes System. Einige der Ziele des neuen Systems waren Geschwindigkeit, einfaches Design, starke Unterstützung für nicht-lineare Entwicklung (Tausende paralleler Zweige), vollständig verteilt und in der Lage, große Projekte wie den Linux-Kernel effizient zu handhaben (Geschwindigkeit und Datengröße).

## Alternativen zu Git

Es gibt mehrere Alternativen zu Git, darunter Subversion (SVN), Mercurial (Hg) und Perforce.

Subversion ist ein zentrales Versionskontrollsystem, das CVS ähnelt. Es wird oft in Unternehmensumgebungen verwendet, weil es einfach zu bedienen ist und eine gute Integration mit anderen Tools bietet.

Mercurial ist ein verteiltes Versionskontrollsystem, das Git ähnelt. Es wird oft in kleineren Projekten verwendet, weil es einfacher zu erlernen ist als Git.

Perforce ist ein zentrales Versionskontrollsystem, das oft in Unternehmensumgebungen verwendet wird. Es bietet gute Unterstützung für große und binäre Dateien.

Jedes dieser Systeme hat seine eigenen Stärken und Schwächen, und die Wahl, welches verwendet werden soll, hängt von den spezifischen Anforderungen des Projekts ab. Git wird von Entwicklern und Unternehmen weltweit weit verbreitet eingesetzt, da es ein unverzichtbares Werkzeug für das Verwalten von Codeänderungen und die Zusammenarbeit mit anderen Entwicklern an Projekten ist. Git ermöglicht es Entwicklern, unabhängig an Code zu arbeiten und dann ihre Änderungen zusammenzuführen, wenn sie bereit sind.

## Wo Sie Ihre Repositories kostenlos speichern können

Es gibt mehrere kostenlose Orte im Internet, an denen Sie Ihre Git-Repositories speichern können. Hier sind einige der beliebtesten:

- GitHub
- GitLab
- Bitbucket
- SourceForge

Jeder dieser Dienste hat seine eigenen Stärken und Schwächen, und die Wahl, welchen davon zu verwenden, hängt von den spezifischen Anforderungen des Projekts ab. GitHub ist der beliebteste Dienst und wird von Entwicklern und Unternehmen weltweit weit verbreitet genutzt. Es bietet unbegrenzte öffentliche Repositories und eine begrenzte Anzahl von privaten Repositories kostenlos.

GitLab ist ein weiterer beliebter Dienst, der unbegrenzte private Repositories kostenlos anbietet. Bitbucket wird oft von kleinen Teams verwendet, da es bis zu fünf Benutzern unbegrenzte private Repositories kostenlos bietet. SourceForge ist ein Dienst, der schon lange existiert und oft für Open-Source-Projekte verwendet wird.