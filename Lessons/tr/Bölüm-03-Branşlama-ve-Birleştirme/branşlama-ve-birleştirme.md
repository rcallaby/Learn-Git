# Branşlama ve Birleştirme

## Branşlara ve amaçlarına giriş:

Yazılım geliştirme alanında Git dalları, kod evrimini ve işbirliğini yönetmek için vazgeçilmez araçlardır. Git'teki bir dal, esasen bir deponun kayıt geçmişindeki belirli bir kayıt için hafif, taşınabilir bir işaretçidir. Geliştiriciler dalları kullanarak, bir projenin farklı yönleri üzerinde aynı anda çalışabilir, yeni özellikler veya düzeltmeler deneyebilir ve ana kod tabanını etkilemeden değişiklikleri izole edebilir. Bu makale, Git dallarının karmaşıklıklarını inceleyecek ve bunların oluşturulmasını, değiştirilmesini, geçmiş yönetimini ve birleştirme çatışmalarının işlenmesini kapsayacaktır.

### Branşlar oluşturma ve bunlar arasında geçiş yapma:

Git'te yeni bir branş oluşturmak için, geliştiriciler “git branch” komutunu ve ardından istenen branş adını kullanabilirler. Örneğin, “feature-branch” adlı bir branş oluşturmak için şu komut çalıştırılır: git branch feature-branch. Bu, yeni bir branş oluşturur, ancak deponun HEAD'i (şu anda etkin olan branş) değişmeden kalır. Burada bir örnek verilmiştir:
```bash
git branch feature-branch
```

Yeni oluşturulan branşa geçmek için "git checkout" komutu kullanılır. git checkout feature-branch yazıldığında, HEAD güncellenir ve geliştirici "feature-branch" bağlamında çalışır. Bir örnek şöyle olabilir:

```bash
git checkout feature-branch
```

Alternatif olarak, Git 2.23 tek bir adımda yeni bir branş oluşturmak ve ona geçmek için daha kullanışlı bir yol sunmuştur: git checkout -b feature-branch. Bu komut dalı oluşturur ve aynı anda ona geçer. Örneğin:
```bash
git checkout -b feature-branch
```

### Branş geçmişini yönetme ve değişiklikleri birleştirme:

Branşlar, geliştiricilerin belirli özellikler veya hata düzeltmeleri üzerinde çalışabilecekleri izole ortamlar olarak işlev görür. Bir branş üzerindeyken, geliştiriciler değişiklikler yapabilir, bunları kaydedebilir ve ana branştan veya diğer branşlardan bağımsız olarak branşın kayıt geçmişini oluşturabilirler.

Bir branştaki değişiklikler tamamlandığında ve entegrasyon için hazır olduğunda, birleştirme devreye girer. Birleştirme, bir branşta yapılan değişiklikleri başka bir branşa birleştirme işlemidir. Bir branşta (ör. “feature-branch”) yapılan değişiklikleri ana branşa birleştirmek için, geliştiriciler ana branşta iken git merge feature-branch komutunu çalıştırabilirler. Bu işlem, “feature-branch” branşındaki değişiklikleri ana branşa entegre ederek commit geçmişlerini birleştirir.

<img alt="Git branching and merging infographic" src="../../../images/Part-03/branching-and-merging.png" />

### Merge çakışmalarının işlenmesi:

Merge çatışmaları, Git birleştirme işlemi sırasında kaynak branş (örneğin, “feature-branch”) ile hedef branş (örneğin, main branch) arasında çakışan değişikliklerle karşılaştığında ortaya çıkar. Çatışmalar genellikle aynı kod satırlarının iki branşta farklı şekillerde değiştirilmesi durumunda ortaya çıkar.

Merge çakışmalarını gidermek için, geliştiriciler çakışan satırları manuel olarak çözmelidir. Git, çakışan dosya içinde çakışan bölümleri gösteren işaretler sağlar ve geliştiriciler, istenen değişiklikleri seçmek için dosyayı düzenlemelidir. Çakışmaları manuel olarak çözdükten sonra, geliştiriciler dosyayı kaydeder ve değişiklikleri ekleyip commit ederek merge işlemini tamamlar. Git, çakışmayı çözülmüş olarak işaretler ve merge işlemini tamamlar.

Çakışmaların çözülmesi zor olduğu durumlarda, geliştiriciler Git'in merge araçlarından yardım alabilir veya ekip üyeleriyle işbirliği yaparak uygun çözümler bulabilirler.

# Sonuç:

Git branşları, kod gelişimini yönetmek ve yazılım geliştirmede işbirliğini kolaylaştırmak için vazgeçilmez araçlardır. Branşları kullanarak, geliştiriciler ana kod tabanını etkilemeden farklı özellikler veya hata düzeltmeleri üzerinde aynı anda çalışabilirler. Branşlar, bağımsız geliştirme ve değişikliklerin izolasyonuna olanak tanır; bu değişiklikler hazır olduğunda ana branşa birleştirilebilir.

Branş oluşturma, geçiş, geçmiş yönetimi ve çakışma çözümü konularını net bir şekilde anlayan geliştiriciler, Git branşlarını etkili bir şekilde kullanarak yapılandırılmış ve verimli bir geliştirme süreci sürdürebilirler. Git branşlarını benimseyen yazılım geliştirme ekipleri, üretkenliği artırabilir, paralel çalışmayı mümkün kılabilir ve nihayetinde yüksek kaliteli kodlar sunabilirler.