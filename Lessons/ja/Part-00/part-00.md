# Gitの歴史と基礎

- [はじめに](#introduction)
- [Gitの創設者](#who-created-git)
- [Gitが作られた理由](#the-reason-why-git-was-created)
- [Gitの代替手段](#alternatives-to-git)
- [無料でリポジトリを保存する場所](#where-to-store-your-repositories-for-free)

# はじめに

Gitは、2005年にLinus Torvaldsによって作成された分散型バージョン管理システムです。Gitは、Team Foundation Version Control、Perforce、またはSubversionなどの中央集中型バージョンコントロールシステム（CVCS）とは根本的に異なる方法で履歴を表現します。中央集中型システムは、リポジトリ内の各ファイルに対して個別の履歴を保存します。Gitはリポジトリ全体のスナップショットのグラフとして履歴を保存します。これらのスナップショットはGitではコミットと呼ばれ、複数の親を持つことができ、直線ではなくグラフのような履歴を作成します。この履歴の違いは非常に重要であり、CVCSに慣れたユーザーがGitを理解するのに主な理由です。

今日Gitを学ぶことは重要です。なぜなら、Gitは世界中の開発者や企業に広く使用されており、コードの変更を管理し、他の開発者とプロジェクトで協力するための不可欠なツールだからです。Gitは開発者がコードを独立して作業し、準備ができたときに変更をマージすることを可能にします。

## Gitの創設者

Gitはもともと2005年にLinuxカーネルの開発のためにLinus Torvaldsによって作成されました。その後、他のカーネル開発者も初期の開発に貢献しました。Junio Hamanoは2005年以来、中核のメンテナーでした。

## Gitが作られた理由

元のチームは以前のバージョン管理システムであるBitKeeperを使用できなくなり、その無料ライセンスを失いました。当時、他の分散システムとしての要件を満たすソースコントロールマネジメント（SCMs）がありませんでした。新しいシステムの目標のいくつかは、速さ、シンプルなデザイン、非線形開発（数千の並行ブランチ）、完全に分散されていてLinuxカーネルのような大規模なプロジェクトを効率的に処理できること（速度とデータサイズ）でした。

## Gitの代替手段

Git以外にもいくつかの代替手段があります。Subversion（SVN）、Mercurial（Hg）、およびPerforceが含まれます。

SubversionはCVSに類似した中央集中型のバージョン管理システムです。使いやすく、他のツールとの統合が良いため、企業環境でよく使用されます。

MercurialはGitに似た分散型のバージョン管理システムです。Gitよりも学びやすいため、小規模なプロジェクトでよく使用されます。

Perforceは中央集中型のバージョン管理システムで、企業環境でよく使用されます。大きなファイルとバイナリファイルに対するサポートが良いです。

これらのシステムはそれぞれ強みと弱みを持っており、使用するものはプロジェクトの具体的なニーズに依存します。Gitは世界中の開発者や企業に広く使用されています。なぜなら、それはコードの変更を管理し、他の開発者とプロジェクトで協力するための不可欠なツールだからです。Gitは開発者がコードを独立して作業し、準備ができたときに変更をマージすることを可能にします。

## 無料でリポジトリを保存する場所

インターネット上にはGitリポジトリを保存できる無料の場所がいくつかあります。以下はその中で最も人気のあるものです。

- GitHub
- GitLab
- Bitbucket
- SourceForge

これらのサービスはそれぞれ独自の強みと弱みを持っており、使用するものはプロジェクトの具体的なニーズに依存します。GitHubは最も人気のあるサービスであり、世界中の開発者や企業に広く使用されています。無制限のパブリックリポジトリと限られた数のプライベートリポジトリを無料で提供しています。

GitLabは別の人気のあるサービスで、無制限のプライベートリポジトリを無料で提供しています。Bitbucketは小規模なチームによく使用されるサービスで、最大5人のユーザーに


