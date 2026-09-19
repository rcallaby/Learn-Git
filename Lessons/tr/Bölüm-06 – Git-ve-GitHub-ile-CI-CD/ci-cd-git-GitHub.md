# **Git ve GitHub ile Sürekli Entegrasyon ve Dağıtım**

## Git ve GitHub’ı CI/CD boru hatlarıyla entegre etme

Sürekli Entegrasyon/Sürekli Dağıtım (CI/CD), modern yazılım geliştirmede yüksek kaliteli kodun üretime teslim sürecini kolaylaştıran hayati bir uygulamadır. Git ve GitHub’ı CI/CD boru hatlarıyla entegre ederek geliştiriciler, uygulamaların derlenmesini, test edilmesini ve dağıtılmasını otomatikleştirebilir; böylece daha hızlı geliştirme döngüleri, tutarlı sürümler ve ekip üyeleri arasında gelişmiş iş birliği sağlanır. Bu makale, Git ve GitHub’ı CI/CD boru hatlarıyla nasıl entegre edeceğinize dair kapsamlı bir rehber sunacak ve süreci göstermek için pratik örnekler içerecektir.

## CI/CD boru hatlarını anlama
CI/CD boru hatları, geliştiricilerin kod değişikliklerini otomatik olarak derlemesine, test etmesine ve üretime dağıtmasına olanak tanıyan otomatikleştirilmiş iş akışlarıdır. Boru hattı, değişiklikler depoya (repository) gönderildiğinde tetiklenir; böylece yeni kodun sürekli olarak entegre edilmesi, test edilmesi ve teslim edilmesi sağlanır. Amaç, hataları erken yakalamak, manuel müdahaleleri azaltmak ve geliştirme verimliliğini artırmaktır.

### Git ve GitHub ile CI/CD boru hatlarının kurulumu
- **Adım 1: Bir CI/CD aracı seçme**  
Birçok CI/CD aracı mevcuttur: Jenkins, Travis CI, CircleCI, GitLab CI/CD ve GitHub Actions. Projenizin gereksinimlerine en uygun olanı ve Git ile GitHub ile sorunsuz entegre olanı seçin.

- **Adım 2: Depo kurulumu**  
Uygulama kodunuzun Git ile sürüm kontrolü altında olduğundan ve bir GitHub deposunda barındırıldığından emin olun. CI/CD aracı, boru hattını tetiklemek için kodu depodan alacaktır.

- **Adım 3: CI yapılandırması**  
CI/CD boru hattını tanımlamak için deponuzda bir yapılandırma dosyası oluşturun. GitHub Actions için yapılandırma dosyası genellikle `.github/workflows/ci.yml` şeklindedir.

- **Adım 4: CI iş akışını tanımlama**  
CI yapılandırma dosyasında, boru hattı tetiklendiğinde yürütülecek adımları tanımlayın. Yaygın adımlar arasında deponun kontrol edilmesi (checkout), derleme ortamının kurulması, bağımlılıkların yüklenmesi ve testlerin çalıştırılması yer alır.

- **Adım 5: Örnek GitHub Actions CI iş akışı:**

```
name: Continuous Integration

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '14.x'

      - name: Install Dependencies
        run: npm install

      - name: Run Tests
        run: npm test

```

### CD (Sürekli Dağıtım) uygulama

**Adım 1: Dağıtım yapılandırması**  
CD iş akışını tanımlamak için `.github/workflows/deploy.yml` gibi bir dağıtım yapılandırma dosyası oluşturun. Bu dosya, uygulamanın üretim ortamına dağıtılması için gereken adımları içermelidir.

**Adım 2: CD iş akışı**  
Dağıtım yapılandırma dosyasında, uygulamayı dağıtmak için gerekli adımları tanımlayın. Bu adımlar uygulamanın derlenmesini, artefaktların oluşturulmasını, geçici (staging) ortama dağıtılmasını ve nihayet üretime dağıtılmasını içerebilir.

**Adım 3: Ortam sırları (secrets)**  
Güvenli dağıtım için hassas bilgileri (örneğin API anahtarları, parolalar) deponuzda şifreli sırlar olarak veya CI/CD aracının ortam değişkenlerinde saklayın.

**Adım 4: Örnek GitHub Actions CD iş akışı**

```
name: Continuous Deployment

on:
  push:
    branches:
      - main

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '14.x'

      - name: Install Dependencies
        run: npm install

      - name: Build Application
        run: npm run build

      - name: Deploy to Production
        run: |
          # Add commands here to deploy the built application to the production environment


```

### Git ve GitHub’ın CI/CD ile entegrasyonu için en iyi uygulamalar
a. **Dal koruması kullanın**: GitHub deponuzda dal koruma kuralları ayarlayarak yalnızca onaylanmış ve testleri geçen kodun ana (main) dala birleştirilmesini sağlayın.

b. **Çekme isteği (pull request) incelemelerinden yararlanın**: Kod kalitesi ve doğruluğunu sağlamak için çekme isteklerinde kod incelemesi zorunlu kılın.

c. **Yüksek kapsamlı testler uygulayın**: Uygulamanızın farklı yönlerini kapsayan kapsamlı testler yazın ve yüksek test kapsamı hedefleyin.

d. **CI/CD boru hatlarını izleyin**: Olası sorunları veya darboğazları belirlemek ve çözmek için CI/CD boru hatlarınızı sürekli izleyin.

e. **Bağımlılıkları düzenli olarak güncelleyin**: Güvenlik açıklarından kaçınmak ve en son özelliklerden yararlanmak için bağımlılıklarınızı güncel tutun.

Git ve GitHub’ı CI/CD boru hatlarıyla entegre etmek, modern yazılım geliştirmede temel bir uygulamadır. Bu rehberde verilen adımları ve örnekleri izleyerek uygulamalarınızın derlenmesini, test edilmesini ve dağıtılmasını otomatikleştirebilir; daha hızlı geliştirme döngüleri, gelişmiş kod kalitesi ve daha verimli, iş birliğine dayalı bir geliştirme iş akışı elde edebilirsiniz. Geliştirme sürecinizi kolaylaştırmak ve yüksek kaliteli yazılımı güvenle teslim etmek için CI/CD’nin gücünü benimseyin.

## Otomatik test ve kod kalitesi kontrolleri

Otomatik test ve kod kalitesi kontrolleri, modern yazılım geliştirme iş akışlarının ayrılmaz parçalarıdır. Geliştiriciler, Git ve GitHub’dan yararlanarak kod değişikliklerinin belirtilen standartları karşıladığından ve gerileme (regression) oluşturmadığından emin olmak için otomatik test ve kod kalitesi kontrolleri uygulayabilir. Bu makale, Git ve GitHub kullanarak otomatik test ve kod kalitesi kontrollerinin nasıl kurulacağına dair ayrıntılı bir rehber sunacak ve pratik örnekler içerecektir.

### Otomatik test ve kod kalitesi kontrollerinin faydaları
Otomatik test ve kod kalitesi kontrolleri birçok avantaj sağlar:

a. **Gelişmiş kod kalitesi**: Otomatik kontroller kodlama standartlarını ve en iyi uygulamaları zorunlu kılarak tutarlı ve sürdürülebilir kod sağlar.

b. **Erken hata tespiti**: Otomatik testler, geliştirme sürecinin erken aşamalarında hataları yakalayarak hatalı kodun dağıtılma olasılığını azaltır.

c. **Daha hızlı geliştirme döngüsü**: Test ve kod kalitesi kontrollerinin otomatikleştirilmesi geliştirme sürecini kolaylaştırarak genel verimliliği artırır.

d. **Dağıtımlara güven**: Otomatik kontroller sayesinde geliştiriciler, kod değişikliklerini üretime dağıtmadan önce güven kazanır.

### Git ve GitHub’da otomatik test uygulama

**Adım 1: Test senaryoları yazma**  
Geliştiriciler, uygulamanın çeşitli yönleri için birim testleri, entegrasyon testleri ve uçtan uca testleri kapsayan test senaryoları yazmalıdır. Bu test senaryoları, uygulama koduyla birlikte Git deposunda saklanmalıdır.

**Adım 2: CI/CD ile entegrasyon**  
Git deponuzu GitHub Actions, Travis CI veya CircleCI gibi bir Sürekli Entegrasyon (CI) hizmetiyle entegre edin. Bu entegrasyon, depoda değişiklik gönderildiğinde testlerin otomatik olarak çalıştırılmasını sağlar.

**Adım 3: Otomatik testler için yapılandırma**  
Test iş akışını tanımlamak için bir yapılandırma dosyası oluşturun (örneğin GitHub Actions için `.github/workflows/tests.yml`). Bu dosya test ortamını, bağımlılıkları ve testleri çalıştıracak komutları belirtmelidir.

**Adım 4: Test için örnek GitHub Actions iş akışı:**
```
name: Automated Tests

on:
  push:
    branches:
      - main

jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '14.x'

      - name: Install Dependencies
        run: npm install

      - name: Run Unit Tests
        run: npm test


```

### Git ve GitHub’da kod kalitesi kontrolleri

- **Adım 1: Lint (kod denetimi)**  
Linter’lar kodu olası hatalar, stil sorunları ve kodlama standartlarına uygunluk açısından analiz eder. Popüler linter’lar arasında JavaScript için ESLint, Ruby için RuboCop ve Python için Pylint yer alır. Projeniz için ilgili linter’ları kurun ve yapılandırın.

- **Adım 2: Statik kod analizi**  
Derinlemesine kod kalitesi kontrolleri gerçekleştirmek için SonarQube veya CodeClimate gibi statik kod analizi araçlarını entegre edin. Bu araçlar karmaşık kodu, kod kokularını (code smells) ve olası güvenlik açıklarını tespit eder.

- **Adım 3: Kod biçimlendirme**  
Prettier veya Black gibi araçlarla tutarlı kod biçimlendirmesini zorunlu kılın. Kod biçimlendirme kontrolleri temiz ve okunabilir bir kod tabanı sağlar.

- **Adım 4: Kod kalitesi kontrolleri için örnek GitHub Actions iş akışı:**

```
name: Code Quality Checks

on:
  pull_request:
    branches:
      - main

jobs:
  code_quality:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '14.x'

      - name: Install Dependencies
        run: npm install

      - name: Run Linter
        run: npm run lint

      - name: Static Code Analysis
        run: npm run analyze


```

### Otomatik test ve kod kalitesi kontrolleri için en iyi uygulamalar

a. **Kapsamlı test senaryoları yazın**: Sağlam test için kenar durumlarını ve farklı senaryoları kapsayın.

b. **Her çekme isteğinde testleri çalıştırın**: Birleştirmeden önce kod kalitesini sağlamak için çekme isteklerinde kontroller uygulayın.

c. **Çekme isteği incelemeleriyle entegre edin**: Çekme isteklerini onaylamadan önce testlerin ve kod kalitesi kontrollerinin geçmesini zorunlu kılın.

d. **Test kapsamını izleyin**: Kod tabanının kritik bölümlerinin test edildiğinden emin olmak için yüksek test kapsamı hedefleyin.

e. **Kod kalitesi araçlarını düzenli olarak gözden geçirin ve güncelleyin**: Linter’larınızı, statik analiz araçlarınızı ve test kütüphanelerinizi güncel tutun.

Otomatik test ve kod kalitesi kontrolleri, sağlıklı ve güvenilir bir kod tabanı sürdürmek için çok önemlidir. Git ve GitHub iş akışınıza otomatik test ve kod kalitesi kontrollerini entegre ederek hataları erken yakalayabilir, kodlama standartlarını zorunlu kılabilir ve yüksek düzeyde kod kalitesi sağlayabilirsiniz. Bu rehberde belirtilen adımları izlemek ve en iyi uygulamalara bağlı kalmak, geliştirme ekibinizin yazılımı güvenle oluşturmasına ve teslim etmesine yardımcı olacak; sonuç olarak verimliliği artıracak ve son kullanıcı deneyimini iyileştirecektir.

## Git ve GitHub Actions kullanarak uygulamaları dağıtma

Günümüzün hızlı tempolu geliştirme ortamında uygulamaları verimli ve güvenli bir şekilde dağıtmak çok önemlidir. Popüler sürüm kontrol sistemi Git ile güçlü bir otomasyon aracı olan GitHub Actions birleştirilerek dağıtım süreci kolaylaştırılabilir. Bu makale, Git ve GitHub Actions kullanarak uygulamaları dağıtma adımlarını pratik örneklerle birlikte anlatacaktır.

### Git ve GitHub deposunun kurulumu
Başlamak için uygulamanızın kaynak kodunun barındırıldığı GitHub üzerinde bir Git deposuna ihtiyacınız vardır. Henüz oluşturmadıysanız şu adımları izleyin:

- **Adım 1**: GitHub’a giriş yapın ve sayfanın sağ üst köşesindeki “+” işaretine tıklayın.

- **Adım 2**: Açılır menüden “New repository” (Yeni depo) seçeneğini seçin.

- **Adım 3**: Bir depo adı ve açıklama girin; herkese açık (public) veya özel (private) depo seçeneğini belirleyin.

- **Adım 4**: Depoyu bir README ile başlatın veya boş oluşturun. Ardından “Create repository” (Depo oluştur) düğmesine tıklayın.

### Uygulamanızı hazırlama
Bu rehber amacıyla HTML, CSS ve JavaScript ile oluşturulmuş basit bir web uygulaması varsayalım. Uygulama kodunuzun önceki adımda oluşturduğunuz GitHub deposunda saklandığından emin olun.

### Dağıtım yapılandırmasını tanımlama
Uygulamanızı GitHub Actions ile otomatik olarak dağıtmak için deponuzda bir dağıtım yapılandırma dosyası tanımlamanız gerekir. Bu dosya, GitHub Actions’a uygulamanızı nasıl derleyip dağıtacağını bildirir. Bu örnekte Node.js tabanlı bir dağıtım kullanacağız; ancak kendi teknoloji yığınınıza uyarlayabilirsiniz.

#### `.github/workflows/deploy.yml` adlı bir dosya oluşturun ve şu içeriği ekleyin:

```
name: Deploy Application
on:
  push:
    branches:
      - main

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '14.x'

      - name: Install Dependencies
        run: npm install

      - name: Build Application
        run: npm run build

      - name: Deploy to Server
        run: |
          # Add commands here to copy the built application to your server or cloud platform


```

### Dağıtım yapılandırmasının açıklaması
Dağıtım yapılandırma dosyasının temel bileşenlerini inceleyelim:

- **on**: GitHub Action’ın ne zaman tetikleneceğini belirtir. Bu örnekte ana (main) dala push yapıldığında tetiklenir.

- **jobs**: Action tetiklendiğinde yürütülecek işlerin listesini içerir. Burada `deploy` adlı tek bir iş vardır.

- **runs-on**: İşin çalışacağı işletim sistemini belirtir. Ubuntu-latest kullanılmaktadır.

- **steps**: Sırayla yürütülecek bir dizi adımı içerir. Bu adımlar deponun kontrol edilmesi, Node.js’in kurulması, bağımlılıkların yüklenmesi, uygulamanın derlenmesi ve sunucuya dağıtılması gibi görevleri gerçekleştirir.

#### Uygulamanın dağıtılması
Dağıtım yapılandırması ayarlandıktan sonra, ana dala değişiklik gönderdiğinizde uygulamanız otomatik olarak dağıtılacaktır. Bu, sürekli dağıtım iş akışını mümkün kılar; manuel müdahaleyi azaltır ve dağıtımlarda tutarlılık sağlar.

## Dağıtımları izleme ve geri alma

Sürekli izleme ve sürüm kontrolü, modern yazılım geliştirme uygulamalarının temel bileşenleridir. Yaygın olarak kullanılan sürüm kontrol sistemi Git, yalnızca kod tabanınızdaki değişiklikleri izlemeye yardımcı olmakla kalmaz, aynı zamanda uygulamaları izleme ve geri alma sürecini de kolaylaştırır. Bu makalede Git’te uygulamaları izleme ve geri alma kavramlarını ele alacak, yazılım sürümlerinizi etkili bir şekilde yönetmeniz için ayrıntılı adım adım bir rehber ve örnekler sunacağız.

## Git’te izleme ve geri almayı anlama
Git’te izleme, uygulamanızın durumunu takip etmeyi ve çeşitli metrikler ile performans göstergelerini gözlemlemeyi içerir. Üretim ortamınızda ortaya çıkabilecek sorunlardan veya beklenmeyen davranışlardan haberdar olmanızı sağlar. Geri alma ise uygulamanın önceki bir duruma döndürülmesi, sorunlara yol açan değişikliklerin geri alınması ve istikrarın yeniden sağlanması anlamına gelir.

### Git’te izleme uygulama
Uygulamanızı Git kullanarak izlemek için şu adımları izleyebilirsiniz:

- **Adım 1: Uygulamanızı sürümleme**  
Uygulama kodunuzun Git ile sürüm kontrolü altında olduğundan emin olun. Bu, izleme ve geri almanın temelidir. Her sürümün net bir şekilde tanımlanması için benzersiz bir etiket (tag) veya dalı olmalıdır.

- **Adım 2: Sürekli Entegrasyon ve Sürekli Dağıtım (CI/CD)**  
Dağıtım sürecini otomatikleştirmek için CI/CD boru hatları uygulayın. CI/CD, kod değişikliklerinin üretime dağıtılmadan önce kapsamlı şekilde test edilmesini sağlar. Ayrıca sürümlerin otomatik olarak etiketlenmesine yardımcı olur.

- **Adım 3: Günlük tutma ve hata izleme**  
Uygulamanıza günlük tutma (logging) ve hata izleme araçlarını entegre edin. Bu, uygulama günlüklerini ve hatalarını yakalayıp analiz etmenizi sağlayarak sorunları gerçek zamanlı olarak belirlemenize yardımcı olur.

- **Adım 4: İzleme araçlarının entegrasyonu**  
Uygulamanıza Prometheus, Grafana veya New Relic gibi izleme araçlarını entegre edin. Bu araçlar performans, kaynak kullanımı ve uygulamanın sağlığı hakkında içgörüler sunabilir.

- **Adım 5: Uyarı ve bildirim**  
Kritik sorunları ekibinize bildirmek için uyarı ve bildirim sistemlerini yapılandırın. Uyarılar önceden tanımlanmış eşiklere veya hata kalıplarına göre tetiklenebilir.

### Git’te uygulamaları geri alma
Git’te uygulamaları geri almak, sorunlu bir sürümde yapılan değişiklikleri geri almayı ve uygulamayı kararlı bir duruma döndürmeyi içerir. Etkili bir şekilde geri almak için şu adımları izleyebilirsiniz:

- **Adım 1: Sorunu belirleme**  
Bir sorun ortaya çıktığında, kök nedeni belirlemek için izleme araçlarından, günlüklerden ve hata izleme sistemlerinden bilgi toplayın.

- **Adım 2: Önceki sürümü kontrol etme**  
Son bilinen kararlı sürüme karşılık gelen commit veya etiketi Git ile kontrol edin. Bu, aşağıdaki komutla yapılabilir:
```
git checkout <tag_or_commit>

```
- **Adım 3: Yeni bir sürüm oluşturma**  
Önceki kararlı duruma döndükten sonra, geri almanın uygulandığını belirtmek için uygun bir etiket veya sürüm numarasıyla yeni bir sürüm oluşturun.

- **Adım 4: Geri alınan sürümü test etme**  
Sorunun çözüldüğünden emin olmak için geri alınan sürümü kapsamlı şekilde test edin. Test sürecini otomatikleştirmek için CI/CD boru hatları kullanılabilir.

- **Adım 5: Geri alınan sürümü dağıtma**  
Geri alınan sürüm kararlı kabul edildikten sonra, CI/CD boru hattınızı kullanarak üretim ortamına dağıtın.

### Git’te izleme ve geri alma için en iyi uygulamalar

Uygulama performansını ve sağlığını düzenli olarak izleyerek sorunları erken yakalayın.  
Her sürümün dağıtımdan önce kapsamlı şekilde test edildiğinden emin olmak için CI/CD boru hattınıza otomatik testler ekleyin.  
Her sürümü net bir şekilde tanımlamak için anlamlı etiketler veya sürüm numaraları kullanın.  
Her sürümde yapılan değişiklikleri takip etmek için ayrıntılı bir değişiklik günlüğü (changelog) tutun.  
Önemli olaylardan sonra post-mortem incelemeleri yaparak bunlardan ders çıkarın ve izleme ile geri alma süreçlerinizi iyileştirin.