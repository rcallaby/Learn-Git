# Learn-Git（Gitの学習）

これは、GitとGithubの学習に関する私のYouTubeチュートリアルシリーズ用のサンプルリポジトリがある場所です。

もし、このリポジトリが役立つと感じたら、他の人が見つけやすくなるように星を⭐で評価していただければ幸いです。

同様に、[YouTubeチャンネル](https://www.youtube.com/@richardcallaby)に購読していただけると大変助かります。そこでは無料のチュートリアルや他の無料の教育リソースを公開しています。

## GitHubへの貢献の手順についてのステップバイステップのチュートリアル

GitHubアカウントの作成：まず初めに、GitHubアカウントがない場合は作成する必要があります。github.comにアクセスし、右上の「Sign up」ボタンをクリックします。指示に従ってアカウントを作成してください。

貢献したいリポジトリの検索：GitHubアカウントができたら、貢献したいリポジトリを検索できます。GitHubの検索バーを使用して、名前やキーワードでリポジトリを検索できます。

リポジトリをフォークする：貢献したいリポジトリを見つけたら、それをフォークする必要があります。

フォークすると、リポジトリのコピーがあなた自身のGitHubアカウントに作成され、元のリポジトリに影響を与えずに変更できます。

### 参照画像
下のボタンをクリックして、右上にあるリポジトリをフォークします。

![fork_image](./images/Readme_images/fork.png)

フォークしたリポジトリをクローンする：リポジトリをフォークしたら、それをローカルマシンにクローンする必要があります。クローンすると、コンピュータ上にリポジトリのコピーが作成されます。リポジトリをクローンするには、ターミナルウィンドウを開き、次のコマンドを入力します：

```bash
git clone https://github.com/your-username/repository-name.git
```
必ず「your-username」と「repository-name」をあなたのGitHubのユーザー名とフォークしたリポジトリの名前に置き換えてください。

### 参照画像
![Clone_repo](./images/Readme_images/Clone.png)

変更を反映するために、変更を示すユニークな名前のブランチを作成してください。ブランチを作成するには、次の構文を使用します：

```bash
git branch "branch-name"
```
### 参照画像
![branch_making](./images/Readme_images/Branch_making.png)

そのブランチに切り替えるには、次の構文を使用します：

```bash
git checkout "branch-name"
```
### 参照画像
![branch_switch](./images/Readme_images/branch_switch.png)

コードの変更：リポジトリをローカルマシンにクローンしたら、コードを変更できます。お好きなテキストエディタまたはIDEを使用してファイルを修正してください。

変更をコミットする：コードを変更した後は、それをローカルリポジトリにコミットする必要があります。これには、ターミナルウィンドウを開いてクローンしたリポジトリのルートに移動し、次のコマンドを使用して変更をステージする必要があります：

```bash
git add .
```

### 参照画像
![add](./images/Readme_images/add.png)

これにより、リポジトリのファイルに対する行った変更がすべてステージされます。

次に、次のコマンドを使用して変更をコミットします：

```bash
git commit -m "変更の簡単な説明"
```

### 参照画像
![Commit](./images/Readme_images/commit.png)

行った変更についての簡潔で情報提供ができるメッセージを含めるようにしてください。

GitHubに変更をプッシュする：変更をローカルリポジトリにコミットしたら、それをGitHubにプッシュする必要があります。これにより、GitHubアカウントのリポジトリのコピーが行った変更で更新されます。変更をプッシュするには、次のコマンドを使用します：

```bash
git push origin branch-name
```

### 参照画像
![Push_image](./images/Readme_images/push.png)

プルリクエストの作成：GitHubに変更をプッシュしたら、フォークしたリポジトリをリロードすると、プルリクエストを作成するオプションが表示されます。そのボタンをクリックしてプルリクエストを作成します。

### 参照画像
![Pull_Request](./images/Readme_images/pull%20request.png)

これにより、変更のレビューとプルリクエストの説明を行うページに移動します。

行った変更とその理由について明

確かつ簡潔な説明を含めるようにしてください。

もし、リポジトリのオーナーが知っておくべき問題や懸念事項がある場合は、プルリクエストの説明にそれを記載してください。

説明に満足したら、「Create pull request」ボタンをクリックしてください。

### 参照画像
![Create_pull_request](./images/Readme_images/Create_pull_request.png)

フィードバックを待つ：プルリクエストを作成したら、リポジトリのオーナーが変更を確認し、フィードバックを提供します。

彼らは追加の変更を求めるかもしれませんし、変更を元のリポジトリにマージするかもしれません。

このプロセス中に忍耐強く対応し、リポジトリのオーナーが提起するフィードバックや懸念事項に対処してください。

フォークしたリポジトリを更新する：リポジトリのオーナーが変更を元のリポジトリにマージした場合、変更を反映するためにフォークしたリポジトリを更新する必要があります。

これを行うには、GitHub上でフォークしたリポジトリに移動し、「Fetch upstream」ボタンをクリックします。

次に、ローカルリポジトリで以下のコマンドを実行して更新します：

```bash
git pull
```

これでGitの使い方の簡単なアイディアが得られるはずです。もちろん、このリポジトリで作成したレッスンを見れば、より詳細な説明が得られます。

## Good first issue

このプロジェクトをオープンソースプロジェクトへの貢献の一環として活用できます。これは **初心者向けの良い課題** となるでしょう。[CONTRIBUTORS.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) ファイルを変更して、そこからあなたのGitHubリポジトリへのリンクを追加してください。ファイル内の指示に従って、Markdownを使用してください。

このリポジトリへの貢献方法についてのステップバイステップの手順は、[First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions) ディレクトリを参照してください。

### 目次

- [Part 00 - 履歴と基盤](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-00/part-00.md)
- [Part 01 - 基本的なナビゲーション](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-01/part-01.md)
- [Part 02 - Gitの初期化](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-02/part-02.md)
- [Part 03 - ブランチとマージ](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-03/Part-03.md)
- [Part 04 - リモートリポジトリとの協力](https://github.com/rcallaby/Learn-Git/tree/main/Lessons/ja/Part-04/Part-04.md)
- [Part 05 - Gitの高度なコンセプト](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-05/Part-05.md)
- [Part 06 - GitとGithubでのCI/CD](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-06/Part-06.md)
- [Part 07 - Gitのベストプラクティスとヒント](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-07/Part-07.md)
- [Part 08 - アジャイル開発におけるGitとGithub](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-08/Part-08.md)
- [Part 09 - GithubとCodespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-09/Part-09.md)
- [Part 10 - Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-10/Part-10.md)
- [Part 11 - 高度なGithub Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-11/Part-11.md)
- [Part 12 - GithubでのJupyter Codespacesの使用](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-12/Part-12.md)
- [Part 13 - GithubでのC# Codespacesの使用](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-13/Part-13.md)
- [Part 14 - GithubでのReact Codespacesの使用](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-14/Part-14.md)
- [Part 15 - GithubでのExpress Codespacesの使用](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-15/Part-15.md)
- [Part 16 - GithubでのRuby on Rails Codespacesの使用](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-16/Part-16.md)
- [Part 17 - GithubでのDjango Codespacesの使用](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-17/Part-17.md)
- [Part 18 - Githubプロジェクト管理ツール](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-18/Part-18.md)
- [Part 19 - Githubプロジェクトボードとノート](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/ja/Part-19/Part-19.md)
