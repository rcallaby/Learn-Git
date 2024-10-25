# Katkıda Bulunma Yönergeleri
Learn-Git'e katkıda bulunmayı düşündüğünüz için teşekkür ederiz! Bu havuz, Git öğrenen kişiler için bir kaynak olmayı amaçlamaktadır ve katkılarınız onu daha da iyi hale getirmeye yardımcı olabilir.

Bu havuza, eğitimi daha iyi hale getirerek veya potansiyel olarak başka bir dile çevirerek katkıda bulunmak isterseniz, lütfen bu fikir veya iyileştirmeyle ilgili yeni bir sorun oluşturun ve fikir yeterince iyiyse ben veya potansiyel olarak bu havuzun üyeleri bunu onaylayacaktır. O noktada değişikliği oluşturabilir ve ardından bir çekme isteği oluşturabilirsiniz.

## Davranış Kuralları
Başlamadan önce lütfen davranış kurallarını okuyun ve bunlara uyun. Tüm katılımcılar için saygılı ve misafirperver bir topluluk sürdürmek istiyoruz.

## Başlarken
Learn-Git'e katkıda bulunmak için temel adımlar şunlardır:

- **Depoyu çatallandırın**

![fork_image](./images/Readme_images/fork.png)

- **Değişiklikleriniz için yeni bir dal oluşturun**

```
git branch "branch-name"
```
### Referans Görüntüsü
![branch_image](./images/Contributing_images/branch_making.png)

Ardından bu dalı açın ve aşağıdaki sözdizimini kullanın:

### Sözdizimi
```
git checkout "branch-name"
```

### Referans Görüntüsü
![checkout_branch](./images/Contributing_images/checkout_image.png)

- **Değişikliklerinizi yapın ve bunları dalınıza kaydedin**

Herhangi bir değişiklik veya ekleme yaptıktan sonra terminalde bu komutu kullanın
```
git add .
```
Değişikliği veya eklemeyi onaylamak için sözdizimi

```
git commit -m "Yapılan değişikliklerin kısa bir açıklaması"
```

### Referans Görseli
![commiting_images](./images/Contributing_images/add_commit.png)

- **Değişikliklerinizi çatalınıza gönderin**
Değişiklikleri GitHub'a gönderin: Değişiklikleri yerel deponuza gönderdikten sonra, bunları GitHub'a göndermeniz gerekir. Bu, GitHub hesabınızdaki deponun kopyasını yaptığınız değişikliklerle günceller. Değişiklikleri göndermek için şu komutu kullanın:

```
git push origin branch-name
```
### Referans Görüntüsü
![Push](./images/Contributing_images/push_origin.png)

- **Çekme isteği oluştur**

Değişiklikleri GitHub'a gönderdikten sonra, çatallı deponuzu yeniden yüklediğinizde, bir çekme isteği oluşturma seçeneğini göreceksiniz. Bir çekme isteği oluşturmak için bu düğmeye tıklayın.

### Referans Görüntüsü

![Çekme İsteği](./images/Contributing_images/pull_request.png)

Bu sizi yaptığınız değişiklikleri inceleyebileceğiniz ve çekme isteğinizin bir açıklamasını sağlayabileceğiniz bir sayfaya götürecektir.

Yaptığınız değişikliklerin ve bunları neden yaptığınızın açık ve öz bir açıklamasını eklediğinizden emin olun.

Depo sahibinin farkında olması gereken herhangi bir sorun veya endişe varsa, çekme isteği açıklamasında bunlardan bahsettiğinizden emin olun.

Açıklamadan memnun kaldığınızda, "Çekme isteği oluştur" düğmesine tıklayın.

![Son Resim](./images/Contributing_images/last.png)

Geri bildirim bekleyin: Çekme isteğini oluşturduktan sonra, depo sahibi değişikliklerinizi inceleyecek ve geri bildirim sağlayacaktır.

## Nasıl Katkıda Bulunulur
Aşağıdaki biçimlerde katkılarınızı bekliyoruz:

### Düzeltmeler
Mevcut içerikte herhangi bir hata veya yanlışlık bulursanız lütfen bir sorun açın, lütfen hataları veya yanlışlıkları ayrıntılı olarak açıklayın. Bu hataların veya yanlışlıkların doğruluğu doğrulanırsa, bu değişikliklerle bir çekme isteği açabilirsiniz. Lütfen dikkatli olmaya çalışın ve sorunu çekme isteğinize bağlayın. Ayrıca, dilbilgisindeki kişisel tercihin mutlaka gerekli bir değişiklik oluşturmadığını da unutmayın.

### Eklemeler
Git öğrenen kişiler için değerli olacağını düşündüğünüz **yeni içerik** için bir fikriniz varsa, **lütfen önce tartışmak için bir sorun açın.** Onaylandıktan sonra, yeni içeriğinizle bir çekme isteği oluşturmaktan çekinmeyin.

### İyileştirmeler
Mevcut içeriği iyileştirmek için önerileriniz varsa, lütfen **önce tartışmak için bir sorun açın**. Onaylandıktan sonra, iyileştirmelerinizle bir çekme isteği oluşturmaktan çekinmeyin.

## Stil Kılavuzu
Learn-Git'e katkıda bulunurken lütfen aşağıdaki stil kılavuzuna uyun:

- Açık ve öz bir dil kullanın
- Bölümleri ayırmak için başlıklar ve alt başlıklar kullanın
- Kavramları göstermek için örnekler ve görseller kullanın
- Uygun olduğunda ilgili kaynaklara bağlantılar ekleyin
- Verilen çeviriniz için her yerde kullanılan uygun yazım ve dilbilgisini kullanın.

## İşbirlikçiler
Bu havuzdaki en önemli rol, bu projede bir işbirlikçinin rolüdür. İşbirlikçi rolü için değerlendirilmek üzere öncelikle bu projeyi sürdürmek ve güncel tutmak için çalışmaya istekli olduğunuzu kanıtlamalısınız. Gelecekteki işbirlikçileri her zaman ararken lütfen artık sürdürmeye katılmamaya karar verirseniz rolünüzün bu havuzdan sonlandırılabileceğini unutmayın. Bu havuza anlamlı bir şekilde ekleme yapmamanız, işbirlikçi rolünüzün uyarı yapılmadan sonlandırılmasına neden olabilir.

# Sonuç
Learn-Git'e katkıda bulunmak için zaman ayırdığınız için teşekkür ederiz! Katkılarınız Git'i yeni başlayanlar için daha erişilebilir hale getirmeye yardımcı olabilir.