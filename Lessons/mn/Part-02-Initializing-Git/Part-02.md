# Git эхлүүлэх - Анхны алхмууд

- [Git анхан шатны ажиллагаа](#git-анхан-шатны-ажиллагаа)
- [Linux-д Git Repository тохируулах](#linux-д-git-repository-тохируулах)
- [Windows-д Git Repository тохируулах](#indows-д-git-repository-тохируулах)
- [Mac-д Git Repository тохируулах](#macos-д-git-repository-тохируулах)

## Git анхан шатны ажиллагаа :

Git хувилбар хянах иж бүрдэл командуудыг олгодог. Цөөн үндсэн хэдийн жишээнд:

`git init` идэвхтэй хавтсанд Git repository үүсгэдэг. Жишээ нь:

```
git init havtasniiner
```

`git clone <repository_url>` нь зайны repository-г өөрийн компьютерт хуулбарлана. Жишээ нь:

```
git clone repository_url
```

`git add <файл>` файлд хйисэн өөрчлөлтүүдийг хадгалхад(commit) бэлднэ(stage). Бүх файлыг бэлдэхэд:

```
git add .
```

эсвэл тодорхой файлыг бэлдэхэд:

```
git add filename
```

`git commit -m "<хадгалсан_мессеж>"` бэлдсэн өөрчлөлтүүдийг repository-руу хадгална. Жишээ нь:

```
git commit -m "тайлбар мессеж"
```

`git push` хадгалсан өөрчлөлтүүдийг зайны repository-руу upload хйинэ.

```
git push repositoryname
```

`git pull` зайны repository дахь өөрчлөлтүүдийг компьютер дээрх repository-руу татна.

```
git pull
```

Доорх бол Linux, Windows, болон Mac дээр хэрхэн Git тохируулах хичээл.

## Linux-д Git Repository тохируулах:

Terminal цонх онгойлгоно.

`cd` командаар repository үүсгэх хавтасруу оч. Жишээ нь ~/Documents хавтасруу очих бол дараах командийг ашиглана:

```
cd ~/Documents
```

Git repository `git init` командаар үүсгэнэ:

```
git init
```

Ингээд таны repository бэлэн болсон. Та одоо файл нэмж, өөрчлөлтүүдээ хадгалж бас бусад Git командуудаа ашиглаж болно.

## Windows-д Git Repository тохируулах:

Git-г албан ёсны website-аас Windows системдээ суулгана: https://git-scm.com/download/win. Хуулсан installer-г уншуулж суулгацын алхмуудыг дагаарай.

Суусан Git Bash програмыг нээнэ. Энэ нь Windows-д ашиглаж болох Linux-тэй төстэй command-line орчин юм.

`cd` командаар repository үүсгэх хавтасруу оч. Жишээ нь ~/Documents хавтасруу очих бол дараах командийг ашиглана:

Navigate to the desired directory where you want to create your repository. For example, to navigate to the Documents directory on your C: drive, use the following command:

```
cd /c/Documents
```

Initialize a new Git repository using the git init command:

```
git init
```

Your repository is now set up. You can start adding files, committing changes, and using other Git commands.

## MacOS-д Git Repository тохируулах:

Open Terminal on your Mac.

Navigate to the desired directory where you want to create your repository. For example, to navigate to the Documents directory, use the following command:

```
cd ~/Documents
```

Initialize a new Git repository using the git init command:

```
git init
```

Your repository is now set up. You can start adding files, committing changes, and using other Git commands.

Now that you have set up the Git repository, you can proceed with adding files, making commits, and performing other Git operations using commands such as git add, git commit, git push, etc. Remember to refer to the Git documentation or other Git tutorials for more details on these operations.

**Note: The steps provided assume a basic setup for a local Git repository. If you want to set up a remote repository or work with existing repositories on hosting platforms like GitHub or GitLab, additional steps are required.**
