# Git - Temel Gezinme

- [Giriiş](#giriiş)
- [BASH Terminalini Açma](#bash-terminalini-açma)
- [Dizinlerde Gezinme](#dizinlerde-gezinme)
- [Dizin İçeriğini Listeleme](#dizin-icerigini-listeleme)
- [Dizin Oluşturma ve Taşıma](#dizin-oluşturma-ve-kaldırma)
- [Dosya Oluşturma ve Kaldırma](#dosya-oluşturma-ve-kaldırma)
- [Sonuç](#sonuç)

# Giriiş:
BASH terminali, kullanıcıların bilgisayarlarının dosya sisteminde gezinmelerine, çeşitli görevleri gerçekleştirmelerine ve Git gibi sürüm kontrol sistemleriyle etkileşim kurmalarına olanak tanıyan güçlü bir komut satırı arayüzüdür. Git, kod depolarındaki değişikliklerin verimli bir şekilde işbirliği ve izlenmesini sağlayan yaygın olarak kullanılan bir dağıtılmış sürüm kontrol sistemidir. Bu makalede, Git ile etkili bir şekilde çalışmak için BASH terminalindeki temel komutlarda nasıl gezinileceğini ve kullanılacağını inceleyeceğiz.

## BASH Terminalini Açma:
Başlamak için tercih ettiğiniz terminal uygulamasını açın. Çoğu Unix tabanlı sistemde, terminali "Uygulamalar" veya "Yardımcı Programlar" klasöründe bulabilirsiniz. Başlatıldığında, komutlarınızı kabul etmeye hazır bir komut istemi görünecektir.

## Dizinlerde Gezinme:

pwd, Print Working Directory'nin kısaltmasıdır ve çalışma dizininin yolunu yazdırır.
```commandline
pwd
```
Bu komutun herhangi bir argümanı veya seçeneği yoktur.

cd komutu ("change directory" ifadesinin kısaltması) dosya sisteminde gezinmek için temeldir. İşte bazı yaygın cd kullanım örnekleri:

Bir dizine geçmek için cd <directory> (<directory> ifadesini istediğiniz dizin adıyla değiştirin) kullanın. Örneğin:
```
cd Documents
```
Bir dizin düzeyine geri dönmek için cd .. yazın, örneğin:
```
cd ..
```
Ana dizininize gitmek için cd veya cd ~ komutunu kullanın. Örneğin:
```
cd ~
```
Önceki dizine gitmek için cd - komutunu kullanın. Örneğin:
```
cd ~
```

## Dizin İçeriğini Listeleme:
ls komutu bir dizinin içeriklerini listelemek için kullanılır. Varsayılan olarak, geçerli dizindeki dosyaları ve dizinleri görüntüler. ls işlevselliğini geliştirmek için bazı yararlı işaretler:

ls -l içerikleri ayrıntılı liste biçiminde görüntüler.
```
ls -l
```
ls -a gizli dosya ve dizinleri gösterir.
```
ls -a
```
ls -h, insan tarafından okunabilir dosya boyutları sağlar.
```
ls -h
```
ls -R dizinleri ve içeriklerini özyinelemeli olarak listeler.
```
ls -R
```

## Dizin Oluşturma ve Kaldırma:
mkdir komutunu ve ardından istediğiniz dizin adını kullanarak dizinler oluşturabilirsiniz:
Mevcut konumda bir dizin oluşturmak için mkdir <dizin> kullanın. Örneğin:
```
mkdir thisdirectory
```
İç içe dizinler oluşturmak için mkdir -p <üst_dizin>/<alt_dizin> komutunu kullanın.
```
mkdir -p thisdirectory/subdirectory
```
Dizinleri kaldırmak için rmdir komutunu kullanın:
rmdir <dizin> boş bir dizini siler.
```
rmdir thisdirectory
```
Dosyaları ve Dizinleri Taşıma ve Yeniden Adlandırma:
mv komutu, dosyaları ve dizinleri taşımanıza ve yeniden adlandırmanıza olanak tanır:
Bir dosyayı veya dizini taşımak için mv <kaynak> <hedef> kullanın. Örneğin:
```
mv thisdirectory newdirectoryname
```

Bir dosya veya dizinin adını değiştirmek için mv <eski_ad> <yeni_ad> komutunu kullanın.
```
mv olddirectory newdirectory
```

## Dosya Oluşturma ve Kaldırma:
Touch komutunu kullanarak yeni bir dosya oluşturabilirsiniz.
```commandline
touch yeni_dosya_adı
```
Veya bir dizinde, şöyle:
```commandline
touch dizini/yeni_dosya_adı
```
Şimdi rm komutunu kullanarak bir dosyayı kaldıralım.
```commandline
rm dosya_adı
```
Dizinleri ve içeriklerini yinelemeli olarak kaldırmak için
```commandline
rm -r dosya_adı
```
Varolmayan dosyaları ve argümanları yok saymak için asla komut isteminde bulunmayın.
```commandline
rm -f dosya_adı
```
Ne yapıldığını kontrol etmek için
```commandline
rm -v dosya_adı
```
Bir dizinin içindeki her şeyi kaldırmak için.
```commandline
rm *
```
## Sonuç:
Git ile birleştirilen BASH terminali, verimli sürüm kontrolü ve dosya yönetimi için sağlam bir ortam sunar. mkdir, rmdir, rm, mv, cd, ls, pwd gibi temel komutlarla ve git init, git add, git commit, git push ve git pull gibi Git'e özgü komutlarla kendinizi tanıştırarak dizinlerde gezinebilir, dizinleri oluşturabilir ve kaldırabilir, dosyaları taşıyabilir ve yeniden adlandırabilir, dosyaları silebilir ve Git depolarınızı etkili bir şekilde yönetebilirsiniz. Uygulama ve keşif, bu komutları kullanmada daha yetkin olmanıza yardımcı olacak ve geliştirme iş akışınızı kolaylaştırmanızı sağlayacaktır.