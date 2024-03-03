# Git эхлүүлэх - Анхны алхмууд

- [Git анхан шатны үйлдлүүд](#git-анхан-шатны-үйлдлүүд)
- [Linux-д Git Repository тохируулах](#linux-д-git-repository-тохируулах)
- [Windows-д Git Repository тохируулах](#windows-д-git-repository-тохируулах)
- [Mac-д Git Repository тохируулах](#macos-д-git-repository-тохируулах)

## Git анхан шатны үйлдлүүд:

Git хувилбар хянах иж бүрдэл командуудыг олгодог. Цөөн үндсэн хэдийн жишээнд:

`git init` идэвхтэй хавтсанд Git repository үүсгэдэг. Жишээ нь:

```
git init havtasniiner
```

`git clone <repository_url>` нь зайны repository-г өөрийн компьютерт хуулбарлана. Жишээ нь:

```
git clone repository_url
```

`git add <файл>` файлд хийсэн өөрчлөлтүүдийг хадгалахад(commit) бэлдэнэ(stage). Бүх файлыг бэлдэхэд:

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

`git push` хадгалсан өөрчлөлтүүдийг зайны repository-руу upload хийнэ.

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

`cd` командаар repository үүсгэх хавтас руу оч. Жишээ нь ~/Documents хавтас руу очих бол дараах командыг ашиглана:

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

Суусан Git Bash программыг нээнэ. Энэ нь Windows-д ашиглаж болох Linux-тэй төстэй command-line орчин юм.

Repository үүсгэхийг хүссэн хавтас руу оч. Жишээ нь C: drive дахь Document хавтас руу очих бол:

```
cd /c/Documents
```

`git init` командыг ашилгаж Git repository үүсгэнэ:

```
git init
```

Ингээд таны repository бэлэн болсон. Та одоо файл нэмж, өөрчлөлтүүдээ хадгалж бас бусад Git командуудаа ашиглаж болно.

## MacOS-д Git Repository тохируулах:

Mac-ынхаа terminal цонх онгойлгоно.

`cd` командаар repository үүсгэх хавтас руу оч. Жишээ нь Documents хавтас руу очих бол дараах командыг ашиглана:

```
cd ~/Documents
```

`git init` командыг ашилгаж Git repository үүсгэнэ:

```
git init
```

Ингээд таны repository бэлэн болсон. Та одоо файл нэмж, өөрчлөлтүүдээ хадгалж бас бусад Git командуудаа ашиглаж болно. Эдгээр үйлдлүүдийн талаар дэлгэрэнгүй мэдээллийг Git-н баримт бичиг болон бусад хичээлүүдээс аваарай.

**Тэмдэглэл: Дээрх алхмууд нь local(өөрийн компьютер) Git repository-н анхан шатны тохиргоонд зориулсан болно. Зайны repository буюу GitHub, GitLab гэх зэрэг платформууд дээр байрлуулсан repository ажиллах бол нэмэгдэл алхмууд хэрэгтэй болохыг анхаарна уу.**
