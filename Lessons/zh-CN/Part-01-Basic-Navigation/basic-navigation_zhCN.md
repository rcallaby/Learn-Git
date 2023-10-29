# Git - 基本导航

- [介绍](#介绍)
- [打开BASH终端](#打开BASH终端)
- [浏览目录](#浏览目录)
- [列出目录内容](#列出目录内容)
- [创建和移动目录](#创建和移动目录)
- [创建和删除文件](#创建和删除文件)
- [结论](#结论)

# 介绍:
BASH 终端是一个强大的命令行界面，允许用户浏览计算机的文件系统、执行各种任务以及与 Git 等版本控制系统进行交互。Git 是一个广泛使用的分布式版本控制系统，它提供高效的协作和跟踪代码存储库的更改。在本文中，我们将探讨如何在 BASH 终端中导航和利用基本命令来有效地使用 Git。

## 打开BASH终端:
首先，打开您喜欢的终端应用程序。在大多数基于 Unix 的系统上，您可以在“应用程序”或“实用程序”文件夹中找到终端。启动后，将出现命令提示符，准备接受您的命令。

## 浏览目录:

pwd 代表打印工作目录，并打印工作目录的路径。
```commandline
pwd
```
此命令没有任何参数或选项。

cd 命令（“更改目录”的缩写）是浏览文件系统的基础。以下是一些常见的 cd 使用示例：

要移动到目录中，请使用 cd（替换为所需的目录名称）。例如：
```
cd Documents
```
若要返回一个目录级别，请键入 cd .。例如：
```
cd ..
```
要转到您的主目录，请使用 cd 或 cd ~ 例如：
```
cd ~
```
要移动到上一个目录，请使用 cd - 例如：
```
cd -
```

## 列出目录内容:
ls 命令用于列出目录的内容。默认情况下，它显示当前目录中的文件和目录。一些有用的标志来增强 ls 功能。

ls -l 以详细的列表格式显示内容。
```
ls -l
```
ls -a 显示隐藏的文件和目录。
```
ls -a
```
ls -h 提供人类可读的文件大小。
```
ls -h
```
ls -R 以递归方式列出目录及其内容。
```
ls -R
```

## 创建和移动目录:
您可以使用 mkdir 命令后跟所需的目录名称来创建目录： 要在当前位置创建目录，请使用 mkdir 。如：
```
mkdir thisdirectory
```
要创建嵌套目录，请使用 mkdir -p <parent_directory>/<child_directory>。
```
mkdir -p thisdirectory/subdirectory
```
要删除目录，请使用 rmdir 命令： rmdir 删除一个空目录。
```
rmdir thisdirectory
```
移动和重命名文件和目录： mv 命令允许您移动和重命名文件和目录： 要移动文件或目录，请使用 mv 。如：
```
mv thisdirectory newdirectoryname
```

要重命名文件或目录，请使用 mv <old_name> <new_name>。
```
mv olddirectory newdirectory
```

## 创建和删除文件:
您可以使用touch命令创建新文件。
```commandline
touch new_file_name
```
或者在一个目录中，例如:
```commandline
touch directory/new_file_name
```
现在让我们使用 rm 命令删除文件。
```commandline
rm file_name
```
以递归方式删除目录及其内容。
```commandline
rm -r file_name
```
要忽略不存在的文件和参数，并永远不要提示。
```commandline
rm -f file_name
```
检查正在执行的操作。
```commandline
rm -v file_name
```
删除目录中的所有内容。
```commandline
rm *
```
# 结论:
BASH 终端与 Git 相结合，为高效的版本控制和文件管理提供了一个强大的环境。通过熟悉基本命令（如 mkdir、rmdir、rm、mv、cd、ls、pwd）和特定于 Git 的命令（如 git init、git add、git commit、git push 和 git pull），您可以浏览目录、创建和删除目录、移动和重命名文件、删除文件以及有效管理 Git 存储库。练习和探索将帮助您更熟练地使用这些命令，从而简化开发工作流程。
