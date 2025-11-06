# 初始化 Git - 入门

## 基本Git操作:
Git 提供了大量用于版本控制的命令，以下是一些基本命令：

git init 初始化当前目录中的新 Git 存储库。如：
```
git init directoryname
```
git clone <repository_url>将远程存储库复制到本地计算机。如：
```
git clone directoryname
```
git add <file> 阶段对文件所做的更改以进行提交。
```
git add . 
```
或
```
git add filename
```
git commit -m “<commit_message>” 将暂存的更改提交到存储库。如：
```
git commit -m "a detailed commit message"
```

Git Push 将提交的更改上传到远程存储库。
```
git push repositoryname
```
git pull 提取更改并将其从远程存储库合并到本地存储库。
```
git pull
```

以下是有关如何在 Linux、Windows 和 Mac 上设置 Git 的分步教程。

## 在Linux中设置Git存储库:

打开终端窗口。

使用 cd 命令导航到要在其中创建存储库的所需目录。例如，若要导航到 ~/Documents 目录，请使用以下命令：

```
cd ~/Documents
```
使用 git init 命令初始化新的 Git 存储库：

```
git init
```
您的存储库现已设置完毕。您可以开始添加文件、提交更改和使用其他 Git 命令。

## 在Windows中设置Git存储库:

从官方网站下载 Git 到您的 Windows 系统上安装 Git：https://git-scm.com/download/win。运行安装程序并按照安装步骤操作。

打开 Git Bash，它在 Windows 上提供类似 Linux 的命令行环境。

导航到要在其中创建存储库的所需目录。例如，若要导航到 C： 驱动器（C盘）上的 Documents 目录，请使用以下命令：

```
cd /c/Documents
```
使用 git init 命令初始化新的 Git 存储库：

```
git init
```
您的存储库现已设置完毕。您可以开始添加文件、提交更改和使用其他 Git 命令。

## 在Mac中设置Git存储库:

在 Mac 上打开“终端”。

导航到要在其中创建存储库的所需目录。例如，若要导航到 Documents 目录，请使用以下命令：

```
cd ~/Documents
```
使用 git init 命令初始化新的 Git 存储库：

```
git init
```
您的存储库现已设置完毕。您可以开始添加文件、提交更改和使用其他 Git 命令。

现在您已经设置了 Git 存储库，您可以使用 git add、git commit、git push 等命令继续添加文件、提交和执行其他 Git 操作。请记住参阅 Git 文档或其他 Git 教程，了解有关这些操作的更多详细信息。

**注意：提供的步骤假定对本地 Git 存储库进行了基本设置。如果要设置远程存储库或在 GitHub 或 GitLab 等托管平台上使用现有存储库，则需要执行其他步骤。
