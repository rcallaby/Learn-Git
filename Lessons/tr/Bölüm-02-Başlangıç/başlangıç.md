# Git'i Başlatma - Başlangıç  

- [Temel Git İşlemleri](#temel-git-işlemleri-)
- [Linux'ta Bir Git Deposu Kurma](#linuxta-bir-git-deposu-kurma-)  
- [Windows'ta Bir Git Deposu Kurma](#windowsta-bir-git-deposu-kurma-)  
- [Mac'te Bir Git Deposu Kurma](#macte-bir-git-deposu-kurma-)  

## Temel Git İşlemleri:  
Git, sürüm kontrolü için geniş bir komut yelpazesi sunar, ancak işte en temel olanlardan bazıları:  

**`git init`**, mevcut dizinde yeni bir Git deposu başlatır. Örneğin:  
```
git init directoryname
```  
**`git clone <repository_url>`**, uzak bir depoyu yerel makinenize kopyalar. Örneğin:  
```
git clone directoryname
```  
**`git add`**, bir dosyada yapılan değişiklikleri commit için hazırlar.  
```
git add . 
```  
veya  
```
git add filename
```  
**`git commit -m "<commit_message>"`** hazırlanan değişiklikleri depoya kaydeder. Örneğin:  
```
git commit -m "a detailed commit message"
```  
**`git push`**, commit edilmiş değişiklikleri uzak bir depoya yükler.  
```
git push repositoryname
```  
**`git pull`**, uzak bir depodan değişiklikleri indirir ve yerel depo ile birleştirir.  
```
git pull
```  

Aşağıda Linux, Windows ve Mac’te Git kurulumu için adım adım bir rehber bulunmaktadır.  

---

## Linux'ta Bir Git Deposu Kurma:  

1. Bir terminal penceresi açın.  
2. **cd** komutunu kullanarak deponuzu oluşturmak istediğiniz dizine gidin. Örneğin, **~/Documents** dizinine gitmek için şu komutu kullanabilirsiniz:  
   ```
   cd ~/Documents
   ```
3. **git init** komutunu kullanarak yeni bir Git deposu başlatın:  
   ```
   git init
   ```
4. Depo artık kurulmuş durumda. Dosya eklemeye, değişiklikleri commit etmeye ve diğer Git komutlarını kullanmaya başlayabilirsiniz.  

---

## Windows'ta Bir Git Deposu Kurma:  

1. Git'i Windows'a kurmak için resmi web sitesinden indirin: [https://git-scm.com/download/win](https://git-scm.com/download/win).  
2. Kurulum dosyasını çalıştırın ve adımları takip edin.  
3. **Git Bash**'i açın (Bu, Windows'ta Linux benzeri bir komut satırı ortamı sağlar).  
4. **cd** komutunu kullanarak deponuzu oluşturmak istediğiniz dizine gidin. Örneğin, **C:** sürücüsündeki **Documents** dizinine gitmek için şu komutu kullanabilirsiniz:  
   ```
   cd /c/Documents
   ```
5. **git init** komutunu kullanarak yeni bir Git deposu başlatın:  
   ```
   git init
   ```
6. Depo artık kurulmuş durumda. Dosya eklemeye, değişiklikleri commit etmeye ve diğer Git komutlarını kullanmaya başlayabilirsiniz.  

---

## Mac'te Bir Git Deposu Kurma:  

1. Mac'inizde **Terminal** uygulamasını açın.  
2. **cd** komutunu kullanarak deponuzu oluşturmak istediğiniz dizine gidin. Örneğin, **Documents** dizinine gitmek için şu komutu kullanabilirsiniz:  
   ```
   cd ~/Documents
   ```
3. **git init** komutunu kullanarak yeni bir Git deposu başlatın:  
   ```
   git init
   ```
4. Depo artık kurulmuş durumda. Dosya eklemeye, değişiklikleri commit etmeye ve diğer Git komutlarını kullanmaya başlayabilirsiniz.  

---

Git deposunu başarıyla kurduğunuza göre, dosya ekleme, commit yapma ve diğer Git işlemlerini gerçekleştirmek için **git add**, **git commit**, **git push** gibi komutları kullanabilirsiniz. Bu işlemlerle ilgili daha fazla ayrıntı için Git belgelerine veya diğer Git eğitimlerine başvurmayı unutmayın.  

**Not:** Burada verilen adımlar, temel bir yerel Git deposu kurulumunu içermektedir. Eğer bir uzak depo oluşturmak veya GitHub, GitLab gibi platformlardaki mevcut depolarla çalışmak istiyorsanız, ek adımlara ihtiyacınız olacaktır.