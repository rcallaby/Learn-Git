# Learn-Git
Burada Git ve Github Öğrenmek üzerine YouTube eğitim serim için bir örnek depo bulacaksınız.
Bu deponun faydalı olduğunu düşünüyorsanız, lütfen ona bir yıldız ⭐ vermeyi düşünün, çünkü başkalarının onu bulması daha kolay olacaktır.

Ayrıca, ücretsiz eğitimler ve diğer ücretsiz eğitim kaynakları yayınladığım yer olan [YouTube kanalıma](https://www.youtube.com/@richardcallaby) abone olursanız çok yardımcı olursunuz.

## GitHub'a nasıl katkıda bulunacağınıza dair adım adım bir eğitim burada
Bir GitHub hesabı oluşturun: Zaten bir GitHub hesabınız yoksa, bir tane oluşturmanız gerekir. github.com adresine gidin ve sağ üst köşedeki "Kaydol" düğmesine tıklayın. Hesabınızı oluşturmak için talimatları izleyin.

Katkıda bulunacağınız bir depo bulun: Bir GitHub hesabınız olduğunda, katkıda bulunmak istediğiniz depoları arayabilirsiniz. GitHub arama çubuğunu kullanarak ad veya anahtar kelimeye göre depoları arayabilirsiniz.

Depoyu çatallandırın: Katkıda bulunmak istediğiniz bir depo bulduğunuzda, onu çatallandırmanız gerekir.

Çatallandırma, kendi GitHub hesabınızda deponun bir kopyasını oluşturur ve bu kopyayı orijinal deponuzu etkilemeden değiştirebilirsiniz.

### Referans Görseli
Sağ üst köşede bulunan depoyu çatallandırmak için aşağıdaki düğmeye tıklayın.

![fork_image](./images/Readme_images/fork.png)

Çatallandırılmış depoyu klonlayın: Depoyu çatallandırdıktan sonra, onu yerel makinenize klonlamanız gerekir. Klonlama, bilgisayarınızda üzerinde çalışabileceğiniz deponun bir kopyasını oluşturur. Depoyu klonlamak için bir terminal penceresi açın ve aşağıdaki komutu girin:

```
git clone https://github.com/your-username/repository-name.git
```
"your-username" ve "repository-name" ifadelerini GitHub kullanıcı adınız ve çatalladığınız deponun adıyla değiştirdiğinizden emin olun.

### Referans Görüntüsü
![Clone_repo](./images/Readme_images/Clone.png)

Kaynak kodunda yapmak istediğiniz değişiklikleri yansıtacak şekilde benzersiz bir şekilde adlandırılmış bir dal oluşturduğunuzdan emin olun. Bir dal oluşturmak için aşağıdaki sözdizimini kullanın:

```
git branch "branch-name"
```
### Referans Görüntüsü
![branch_making](./images/Readme_images/Branch_making.png)

Bu dalı açmak için aşağıdaki sözdizimini kullanın:
```
git checkout "branch-name"
```
### Referans Görüntüsü

![branch_switch](./images/Readme_images/branch_switch.png)

Kodda değişiklikler yapın: Depoyu yerel makinenize kopyaladıktan sonra, kodda değişiklikler yapabilirsiniz. Dosyaları değiştirmek için tercih ettiğiniz metin düzenleyicisini veya IDE'yi kullanın.

Değişiklikleri kaydedin: Kodda değişiklikler yaptıktan sonra, bunları yerel deponuza kaydetmeniz gerekir. Bunu yapmak için bir terminal penceresi açın ve kopyalanan deponun köküne gidin. Değişiklikleri düzenlemek için aşağıdaki komutu kullanın:

```
git add .
```

### Referans Görüntüsü
![add](./images/Readme_images/add.png)

Bu, depodaki dosyalarda yapılan tüm değişiklikleri aşamalandıracaktır.

Sonra, aşağıdaki komutu kullanarak değişiklikleri kaydedin:

```
git commit -m "Yapılan değişikliklerin kısa bir açıklaması"
```

### Referans Görüntüsü
![Commit](./images/Readme_images/commit.png)

Yaptığınız değişiklikleri açıklayan kısa ve bilgilendirici bir mesaj eklediğinizden emin olun.

Değişiklikleri GitHub'a gönderin: Değişiklikleri yerel deponuza gönderdikten sonra, bunları GitHub'a göndermeniz gerekir. Bu, GitHub hesabınızdaki deponun kopyasını yaptığınız değişikliklerle günceller. Değişiklikleri göndermek için aşağıdaki komutu kullanın:

```
git push origin branch-name
```

### Referans Görüntüsü
![Push_image](./images/Readme_images/push.png)

Bir çekme isteği oluşturun: Değişiklikleri GitHub'a gönderdikten sonra, çatallanmış deponuzu yeniden yüklediğinizde, bir çekme isteği oluşturma seçeneğini göreceksiniz. Bir çekme isteği oluşturmak için bu düğmeye tıklayın.

### Referans Görüntüsü
![Pull_Request](./images/Readme_images/pull%20request.png)

Bu sizi yaptığınız değişiklikleri inceleyebileceğiniz ve çekme isteğinizin bir açıklamasını sağlayabileceğiniz bir sayfaya götürecektir.

Yaptığınız değişikliklerin ve bunları neden yaptığınızın açık ve öz bir açıklamasını eklediğinizden emin olun.

Depo sahibinin farkında olması gereken herhangi bir sorun veya endişe varsa, bunlardan çekme isteği açıklamasında bahsettiğinizden emin olun.

Açıklamadan memnun kaldığınızda, "Çekme isteği oluştur" düğmesine tıklayın.

### Referans Görüntüsü
![Create_pull_request](./images/Readme_images/Create_pull_request.png)

Geri bildirim bekleyin: Çekme isteğini oluşturduktan sonra, depo sahibi değişikliklerinizi inceleyecek ve geri bildirim sağlayacaktır.

Sizden ek değişiklikler yapmanızı isteyebilirler veya değişikliklerinizi orijinal depoya birleştirebilir.

Bu süreçte sabırlı ve duyarlı olun ve depo sahibinin dile getirdiği geri bildirimleri veya endişeleri ele aldığınızdan emin olun.

Çatallanmış deponuzu güncelleyin: Depo sahibi değişikliklerinizi orijinal depoya birleştirirse, çatallanmış deponuzu bu değişiklikleri yansıtacak şekilde güncellemeniz gerekir.

Bunu yapmak için GitHub'daki çatallanmış deponuza gidin ve "Yukarı akışa getir" düğmesine tıklayın.

Ardından, güncellemek için yerel deponuzda aşağıdaki komutu çalıştırın:

```
git pull
```

Bu size Git'i nasıl kullanacağınıza dair kısa bir fikir vermeli, elbette daha ayrıntılı açıklamalar için bu depoda oluşturduğum derslere bakabilirsiniz.

## İyi ilk sayı

Bu projeyi açık kaynaklı projelere katkıda bulunmaya başlamanın bir yolu olarak kullanabilirsiniz. Bu **iyi bir ilk sorun** olabilir, sadece [CONTRIBUTORS.md](https://github.com/rcallaby/Learn-Git/blob/main/CONTRIBUTORS.md) dosyasını kendi GitHub deponuza bağlanacak şekilde değiştirin. Dosyada gösterildiği gibi Markdown kullanın.

Lütfen bu depoya nasıl katkıda bulunacağınıza dair adım adım talimatlar için [First-Contributions](https://github.com/rcallaby/Learn-Git/tree/main/First-Contributions) dizinine bakın.
### İçindekiler

- [Bölüm 00 - Tarih ve Temel](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-00-Tarih-ve-Temelleri/git'in-tarihi.md)
- [Bölüm 01 - Temel Gezinme](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-01-Temel-Navigasyon/temel-navigasyon.md)
- [Bölüm 02 - Git'i Başlatma](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-02-Ba%C5%9Flang%C4%B1%C3%A7/ba%C5%9Flang%C4%B1%C3%A7.md)
- [Bölüm 03 - Dallanma ve Birleştirme](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-03-Bran%C5%9Flama-ve-Birle%C5%9Ftirme/bran%C5%9Flama-ve-birle%C5%9Ftirme.md)
- [Part 04 - Uzak Depolarla İşbirliği Yapma](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-04-Repositoryler/repositoryler.md)
- [Part 05 - Gelişmiş Git Kavramları](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-05-Geli%C5%9Fmi%C5%9F-Git-Kavramlar%C4%B1/geli%C5%9Fmi%C5%9F-git-kavramlar%C4%B1.md)
- [Part 06 - Git ve Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-06%20%E2%80%93%20Git-ve-GitHub-ile-CI-CD/ci-cd-git-GitHub.md)
- [Part 07 - Git En İyi Uygulamaları ve İpuçları](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-07%20%E2%80%93%20Git-En-%C4%B0yi-Uygulamalar%C4%B1-ve-%C4%B0pu%C3%A7lar%C4%B1/en-yi-uygulamalar.md)
- [Part 08 - Agile Geliştirmede Git ve Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-08%20%E2%80%93%20%C3%87evik%20(Agile)-Geli%C5%9Ftirmede-Git-ve-GitHub/git-GitHub-%C3%A7evik-geli%C5%9Ftirme.md)
- [Part 09 - Github ve Codespaces](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-09%20%E2%80%93%20GitHub-ve-Codespaces/GitHub-codespaces.md)
- [Part 10 - Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-10-Github-eylemleri/GitHub-actions.md)
- [Part 11 - Advanced Github Actions](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-11%20%E2%80%93%20Geli%C5%9Fmi%C5%9F-GitHub-Actions/geli%C5%9Fmi%C5%9F-GitHub-actions.md)
- [Part 12 - Jupyter Codespaces'i Kullanma Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-12%20%E2%80%93%20GitHub-da-Jupyter-Codespaces-Kullan%C4%B1m%C4%B1/GitHub-juypter-codespace.md)
- [Part 13 - Github'da C# Codespaces Kullanımı](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-13%20%E2%80%93%20GitHub-da-C%23-Codespaces-Kullan%C4%B1m%C4%B1/GitHub-CSharp-codespace.md)
- [Part 14 - React Codespaces Kullanımı Github](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-14%20%E2%80%93%20GitHub-da-React-Codespaces-Kullan%C4%B1m%C4%B1/GitHub-react-codespace.md)
- [Part 15 - Github'da Express Codespaces Kullanımı](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-15%20%E2%80%93%20GitHub-da-Express-Codespaces-Kullan%C4%B1m%C4%B1/GitHub-express-codespace.md)
- [Part 16 - Ruby on Rails Codespaces Kullanımı](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-16%20%E2%80%93%20Ruby-on-Rails-Codespaces-Kullan%C4%B1m%C4%B1/GitHub-rubyrails-codespaces.md)
- [Part 17 - Github'da Django Kod Alanlarını Kullanma](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-17%20%E2%80%93%20GitHub-da-Django-Codespaces-Kullan%C4%B1m%C4%B1/GitHub-Django-codespace.md)
- [Part 18 - Github Proje Yönetim Araçları](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-18%20%E2%80%93%20GitHub-Proje-Y%C3%B6netim-Ara%C3%A7lar%C4%B1/GitHub-proje-y%C3%B6netim-ara%C3%A7lar%C4%B1.md)
- [Part 19 - Github Proje Panoları ve Notlar](https://github.com/rcallaby/Learn-Git/blob/main/Lessons/tr/B%C3%B6l%C3%BCm-19%20%E2%80%93%20GitHub-Proje-Panolar%C4%B1-ve-Notlar/GitHub-proje-panolar%C4%B1-ve-notlar.md)

#### Bu eğitimin çevirileri
Aşağıda bu eğitimin birçok farklı dildeki çevirilerini bulabilirsiniz. Lütfen bu çevirilerin bazılarının devam eden bir çalışma olduğunu ve henüz tam olarak tamamlanmadığını unutmayın.

- Çince (Basitleştirilmiş)
- Fransızca
- Almanca
- Rusça
- İspanyolca
- Hintçe
- İtalyanca
- Moğolca
- Japonca
- Fransız
