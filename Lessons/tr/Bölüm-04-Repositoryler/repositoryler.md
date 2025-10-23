# Uzak Repository'lerle İşbirliği

- [Uzak repository'leri kurma (Github, GitLab, Bitbucket)](#uzak-repositoryleri-kurma-github-gitlab-bitbucket)
- [Github](#github)
- [GitLab](#gitlab)
- [Bitbucket](#bitbucket)
- [Uzak repository'lerden değişiklikleri push ve pull etme](#uzak-repositorylerden-değişiklikleri-push-ve-pull-etme)
- [Birleştirme çakışmalarını yönetme](#birleştirme-çakışmalarını-yönetme)
- [En İyi Uygulamalar](#en-iyi-uygulamalar)

## Uzak repository'leri kurma (GitHub, GitLab, Bitbucket)

Yazılım geliştirme dünyasında, sürüm kontrol sistemleri kod repository'lerini yönetmek, işbirliğini kolaylaştırmak ve ekip üyeleri arasında sorunsuz bir iş akışı sağlamak için çok önemli bir rol oynar. GitHub, GitLab ve Bitbucket gibi platformlarda barındırılan uzak repository'ler, geliştiricilere kodlarını depolamak, yönetmek ve paylaşmak için merkezi bir konum sunar. Bu makalede, bu platformların her birinde uzak repository kurmanın adım adım sürecini inceleyeceğiz.

### GitHub
GitHub, Git kullanarak sürüm kontrolü için en popüler web tabanlı barındırma platformlarından biridir. İşte GitHub'da uzak bir repository kurmanın ayrıntılı bir kılavuzu:

Adım 1: GitHub Hesabı Oluşturma
Eğer zaten bir hesabınız yoksa, github.com adresini ziyaret edin ve bir GitHub hesabı oluşturun.

Adım 2: Yeni Bir Repository Oluşturma
Giriş yaptıktan sonra, GitHub panosunun sağ üst köşesindeki "+ New" butonuna tıklayın. Repository'niz için bir isim, isteğe bağlı bir açıklama belirleyin ve genel veya özel olması gerektiğini seçin.

Adım 3: Repository'yi Başlatma
Repository'yi oluşturduktan sonra, genellikle önerilen bir README dosyası ile başlatma seçeneğiniz vardır. README dosyası, projeniz hakkında temel bilgiler sağlar ve işbirlikçiler için bir başlangıç noktası görevi görür.

Adım 4: Repository'yi Klonlama (Opsiyonel)
Repository ile bilgisayarınızda yerel olarak çalışmak istiyorsanız, Git komutunu kullanarak klonlayabilirsiniz: git clone <repository_url>.

### GitLab
GitLab, kapsamlı bir özellik seti sunan, yaygın olarak kullanılan başka bir web tabanlı Git repository yöneticisidir. İşte GitLab'de uzak bir repository kurmanın yolu:

Adım 1: GitLab Hesabı Oluşturma
gitlab.com adresini ziyaret edin ve hesabınız yoksa bir hesap oluşturun.

Adım 2: Yeni Bir Proje Oluşturma
Giriş yaptıktan sonra, panodaki "New Project" butonuna tıklayın. Bir isim, isteğe bağlı bir açıklama belirleyin ve projeniz için görünürlük seviyesini (genel, dahili veya özel) seçin.

Adım 3: Repository'yi Başlatma
GitHub'a benzer şekilde, repository'yi bir README dosyası ile başlatma seçeneğiniz vardır, bu iyi bir uygulamadır.

Adım 4: Repository'yi Klonlama (Opsiyonel)
Repository ile bilgisayarınızda yerel olarak çalışmak istiyorsanız, Git komutunu kullanarak klonlayabilirsiniz: git clone <repository_url>.

### Bitbucket
Atlassian'a ait olan Bitbucket, Git repository'lerini barındırmak için yaygın olarak kullanılan başka bir platformdur. Bitbucket'ta uzak bir repository kurmak aşağıdaki adımları içerir:

Adım 1: Bitbucket Hesabı Oluşturma
bitbucket.org adresine gidin ve hesabınız yoksa bir Bitbucket hesabı oluşturun.

Adım 2: Yeni Bir Repository Oluşturma
Giriş yaptıktan sonra, Bitbucket panosundaki "Create repository" butonuna tıklayın. Bir isim, isteğe bağlı bir açıklama belirleyin ve repository'nin erişim seviyesini (genel veya özel) seçin.

Adım 3: Repository Türünü Seçme
Bitbucket, Git repository'si veya Mercurial repository'si oluşturma arasında seçim yapmanıza olanak tanır. Repository türü olarak "Git"i seçin.

Adım 4: Repository'yi Başlatma
GitHub ve GitLab gibi, sorunsuz bir başlangıç için repository'yi bir README dosyası ile başlatabilirsiniz.

Adım 5: Repository'yi Klonlama (Opsiyonel)
Repository ile bilgisayarınızda yerel olarak çalışmak istiyorsanız, Git komutunu kullanarak klonlayabilirsiniz: git clone <repository_url>.

GitHub, GitLab ve Bitbucket kullanarak uzak repository'leri kurmak, sürüm kontrol sistemleri ile çalışan herhangi bir geliştirici için temel bir beceridir. Bu makalede sağlanan adım adım kılavuzları izleyerek, uzak repository'lerinizi kolayca oluşturabilir, başlatabilir ve ekip üyelerinizle heyecan verici yazılım projeleri üzerinde işbirliği yapmaya başlayabilirsiniz. GitHub, GitLab veya Bitbucket'ı seçseniz de, her platform geliştirme iş akışınızı kolaylaştırmak ve kod işbirliğini geliştirmek için sağlam bir özellik seti sunar.


## Uzak repository'lerden değişiklikleri push ve pull etme

Sürüm kontrol sistemleri, işbirlikçi yazılım geliştirme için vazgeçilmez araçlardır ve ekiplerin kod değişikliklerini verimli bir şekilde yönetmelerini sağlar. En popüler sürüm kontrol sistemlerinden biri olan Git, geliştiricilerin uzak repository'lerden değişiklikleri push ve pull ederek aynı proje üzerinde eşzamanlı olarak çalışmasına olanak tanır. Bu makalede, değişiklikleri push ve pull etme kavramlarını, önemlerini ve bir ekip içinde sorunsuz işbirliği sağlamak için en iyi uygulamaları inceleyeceğiz.

Uzak Repository'leri Anlamak
Uzak repository, geliştiricilerin proje kodlarını depoladığı ve yönettiği paylaşılan, merkezi bir konumdur. Bir ekipte çalışırken, her üyenin bilgisayarında repository'nin yerel bir kopyası bulunur. Uzak repository, çeşitli geliştiriciler tarafından yapılan değişiklikleri senkronize etmek için merkezi referans noktası görevi görür.

Değişiklikleri Uzak Repository'ye Push Etme
Değişiklikleri push etmek, yerel kod değişikliklerini yerel repository'nizden uzak repository'ye gönderme işlemini ifade eder. Uzak repository'yi ekip tarafından yapılan en son değişikliklerle güncel tutmak önemlidir.

İşte değişiklikleri push etme konusunda adım adım bir kılavuz:

Adım 1: Değişikliklerinizi Yerel Olarak Commit Edin
Değişiklikleri push etmeden önce, değişikliklerinizi yerel olarak commit etmeniz gerekir. Bir commit, yerel repository'nizdeki dosyalarda yaptığınız değişikliklerin bir anlık görüntüsüdür. Yapılan değişiklikleri açıklamak için açıklayıcı bir commit mesajı eklemek önemlidir.

Adım 2: Uzak Repository'yi Doğrulayın
Yerel repository'nizde doğru uzak repository URL'sinin yapılandırıldığından emin olun. Yerel repository'nizle ilişkili uzak repository'leri kontrol etmek için aşağıdaki komutu kullanabilirsiniz:

```
git remote -v
```
Adım 3: Değişiklikleri Push Edin
Commit edilmiş değişikliklerinizi uzak repository'ye push etmek için aşağıdaki komutu kullanın:
```
git push <remote_name> <branch_name>
```
Örneğin:

```
git push origin main
```
Bu komut, yerel "main" branşındaki değişiklikleri "origin" adlı uzak repository'ye push eder.

<img alt="Git branching and merging infographic" src="../../../images/Part-04/push.jpeg" />


Uzak Repository'den Değişiklikleri Pull Etme
Değişiklikleri pull etmek, uzak repository'den en son değişiklikleri alma ve bunları yerel repository'nize entegre etme işlemini ifade eder. Bu, yerel kodunuzun projedeki en son gelişmelerle güncel olmasını sağlar.

Değişiklikleri pull etmek için şu adımları izleyin:

Adım 1: Yerel Değişiklikleri Commit Edin
Değişiklikleri pull etmeden önce, pull işlemi sırasında çakışmaları önlemek için yerel değişikliklerinizi commit etmek en iyisidir.

Adım 2: Değişiklikleri Fetch Edin
Aşağıdaki komutu kullanarak uzak repository'den değişiklikleri fetch edin:

```
git fetch <remote_name>
```
Örneğin:
```
git fetch origin
```
Bu komut, uzak repository'den tüm değişiklikleri, bunları yerel branşınıza otomatik olarak birleştirmeden alır.


Adım 3: Değişiklikleri Merge Edin
Değişiklikleri fetch ettikten sonra, bunları yerel branşınıza merge etmeniz gerekir. Aşağıdaki komutu kullanın:

```
git merge <remote_name>/<branch_name>
```
Örneğin:
```
git merge origin/main
```

<img alt="Git branching and merging infographic" src="../../../images/Part-04/fetch.jpeg" />

Bu komut, uzak "main" branşındaki değişiklikleri yerel branşınıza merge eder.

#### Birleştirme Çakışmalarını Yönetme
Bazen, değişiklikleri pull ederken, aynı kod satırları hem uzak depoda hem de yerel deponuzda değiştirilmişse Git çakışmalarla karşılaşabilir. Bu gibi durumlarda, Git farklılıkları otomatik olarak çözemez ve manuel müdahale gerektirir.

Bir merge çakışmasıyla karşılaştığınızda, çözmek için şu adımları izleyin:

a. Çakışan dosya(lar)ı açın ve çakışan değişiklikleri gösteren çakışma işaretçilerini arayın.

b. İstenen değişiklikleri tutmak ve çakışma işaretçilerini kaldırmak için dosya(lar)ı düzenleyin.

c. Merge'ü tamamlamak için çözülmüş değişiklikleri commit edin.

#### En İyi Uygulamalar
Değişiklikleri push ve pull ederken sorunsuz işbirliği sağlamak için aşağıdaki en iyi uygulamaları göz önünde bulundurun:

Her zaman push etmeden önce pull edin: Değişikliklerinizi push etmeden önce, çakışma olasılığını en aza indirmek için uzak repository'den en son değişiklikleri pull edin.

Sık commit yapın: Küçük, mantıklı commit'ler yapın ve değişikliklerin net bir geçmişini tutmak için anlamlı commit mesajları ekleyin.

Özellik branşları kullanın: Yeni özellikler veya hata düzeltmeleri üzerinde çalışırken, ana geliştirme branşıyla çakışmaları önlemek için ayrı özellik branşları oluşturun.

Kod incelemeleri: Geliştirme sürecinde potansiyel sorunları erken yakalamak için ekip üyeleri arasında kod incelemelerini teşvik edin.

Sürekli Entegrasyon (CI): Kod değişikliklerini ana branşa test etme ve entegre etme sürecini otomatikleştirmek için CI araçlarını uygulayın.

Uzak repository'lerden değişiklikleri push ve pull etmek, işbirlikçi yazılım geliştirmeyi kolaylaştıran Git'teki temel kavramlardır. En iyi uygulamaları izleyerek ve iş akışını anlayarak, ekipler projelerini verimli bir şekilde yönetebilir ve kod değişikliklerinin sorunsuz bir şekilde entegre edilmesini sağlayabilir. Düzenli olarak değişiklikleri push ve pull etmek, uzak repository'yi güncel tutar, çakışmaları en aza indirir ve daha üretken ve uyumlu bir geliştirme sürecine yol açar.

## Branşlar ve pull request'ler kullanarak diğer geliştiricilerle işbirliği yapma

İşbirlikçi yazılım geliştirme, aynı anda farklı özellikler üzerinde çalışan birden fazla geliştiricinin yer aldığı karmaşık ve dinamik bir süreçtir. Bu süreci kolaylaştırmak için Git gibi sürüm kontrol sistemleri, branşlar ve pull request'ler gibi özellikler sağlar. Bu makalede, işbirlikçi geliştirme için branşlar ve pull request'leri kullanmanın önemini inceleyecek ve etkili ekip çalışmasını desteklemek için en iyi uygulamaları keşfedeceğiz.

Branşları Anlamak
Git'te, bir branş bir commit'e işaret eden hafif, taşınabilir bir işaretçidir. Geliştiricilerin, ana geliştirme branşını ('master' veya 'main' olarak adlandırılır) etkilemeden yeni özellikler, hata düzeltmeleri veya deneyler üzerinde çalışmasına olanak tanır. Her branş, bağımsız bir geliştirme hattını temsil eder ve geliştiricilerin değişikliklerini diğerlerinden izole etmelerini ve belirli görevler üzerinde çalışmalarını sağlar.

Branşları kullanmak çeşitli faydalar sunar:

a. Değişikliklerin İzolasyonu: Branşlar, geliştiricilerin değişikliklerini izole etmelerini sağlar ve entegre edilmeye hazır olana kadar diğer geliştiricilerin çalışmalarıyla çakışmaları önler.

b. Paralel Geliştirme: Birden fazla geliştirici farklı branşlar üzerinde aynı anda çalışabilir, bu da ilerlemeyi yönetmeyi ve izlemeyi kolaylaştırır.

c. Özellik Deneyimi: Geliştiriciler, ana kod tabanının kararlılığını etkilemeden yeni fikirleri test etmek için deneysel branşlar oluşturabilir.

Branşlar ile İşbirliği Yapma
Branşları kullanarak işbirliği yapma adımlarını inceleyelim:

Adım 1: Yeni Bir Branş Oluşturun
Herhangi bir yeni işe başlamadan önce, ana branştaki en son koda dayalı yeni bir branş oluşturun. Aşağıdaki komutu kullanın:

```
git checkout -b <branch_name>
```
Örneğin:

```
git checkout -b feature/new-feature
```
Bu komut, "feature/new-feature" adlı yeni bir branş oluşturur ve ona geçer.

Adım 2: Branş Üzerinde Çalışın
Yeni oluşturulan branş üzerinde gerekli kod değişikliklerini yapın ve commit edin. İlerlemenizi takip etmek için düzenli olarak değişikliklerinizi commit edin.

Adım 3: Branşı Uzak Depoya Push Edin
Başkalarıyla işbirliği yapmak için, branşınızı uzak depoya push edin:

```
git push origin <branch_name>
```
Örneğin:

```
git push origin feature/new-feature
```
Bu komut, yerel "feature/new-feature" branşınızı uzak depoya push eder.

Adım 4: Başkalarıyla İşbirliği Yapın
Branşınız uzak depoda olduğunda, diğer geliştiriciler değişikliklerinizi inceleyebilir, geri bildirim sağlayabilir veya hatta aynı branş üzerinde sizinle işbirliği yapabilir.

<img alt="Git branching and merging infographic" src="../../../images/Part-04/push-branch.jpeg" />

## Pull Request'leri Anlamak
Bir pull request (PR), GitHub ve Bitbucket gibi Git barındırma platformlarında yaygın olarak bulunan bir özelliktir. Bir branştan diğerine, genellikle bir özellik branşından ana branşa değişiklikleri birleştirmek için resmi bir taleptir.

### Pull request'leri kullanmak çeşitli faydalar sunar:

a. Kod İncelemesi: Pull request'ler, diğer geliştiricilerin değişiklikleri inceleyebildiği, iyileştirmeler önerebileceği ve kod kalitesini sağlayabileceği bir platform sağlar.

b. Tartışma ve İşbirliği: Geliştiriciler, önerilen değişiklikleri doğrudan pull request içinde tartışabilir, bu da daha iyi kararlar alınmasına ve işbirliğinin teşvik edilmesine yol açar.

c. Sürekli Entegrasyon ve Test: Birçok platform, Sürekli Entegrasyon (CI) araçlarıyla entegrasyona izin vererek, kod kalitesini sağlamak için pull request'ler üzerinde testleri otomatikleştirir.

### Pull Request'ler ile İşbirliği Yapma
İşte pull request'leri kullanarak işbirliği yapma konusunda adım adım bir kılavuz:

Adım 1: Pull Request Oluşturun
Git barındırma platformunda, branşınıza gidin ve "Create Pull Request" butonuna tıklayın. Değişikliklerinizi birleştirmek istediğiniz hedef branşı (genellikle ana branş) seçin.

Adım 2: Değişiklikleri Açıklayın
Pull request'iniz için net ve açıklayıcı bir başlık ve açıklama yazın, yapılan değişiklikleri ve branşın amacını özetleyin.

Adım 3: İnceleyiciler Talep Edin
Pull request'iniz için uygun inceleyicileri seçin. Bunlar genellikle kod tabanına aşina olan ve değerli geri bildirim sağlayabilen diğer geliştiricilerdir.

Adım 4: İnceleyin ve Tekrarlayın
İnceleyiciler değişikliklerinizi inceleyecek, yorumlar bırakacak ve iyileştirmeler önerecektir. Geri bildirimlere açık olun ve kodunuzu projenin standartlarını karşılayana kadar tekrarlayın.

Adım 5: Pull Request'i Merge Edin
Pull request onaylandıktan ve tüm tartışmalar çözüldükten sonra, hedef branşa, genellikle ana branşa merge edilebilir. Değişiklikler artık projenin kod tabanının bir parçasıdır.

#### En İyi Uygulamalar
Branşlar ve pull request'ler kullanarak sorunsuz işbirliği sağlamak için aşağıdaki en iyi uygulamaları göz önünde bulundurun:

a. Açıklayıcı İsimler Kullanın: Branşlara ve pull request'lere, ekip üyelerinin amaçlarını anlamalarını kolaylaştırmak için net ve açıklayıcı isimler verin.

b. Pull Request'leri Küçük Tutun: Belirli bir özellik veya hata düzeltmesine odaklanan pull request'ler oluşturun. Daha küçük pull request'lerin incelenmesi ve yönetilmesi daha kolaydır.

c. Branşları Düzenli Olarak Güncelleyin: Düzenli olarak merge veya rebase yaparak özellik branşlarınızı ana branştan gelen en son değişikliklerle güncel tutun.

d. Kod İncelemelerinden Yararlanın: Kod kalitesini korumak ve bilgi paylaşmak için kod incelemelerini teşvik edin ve başkalarının kodunu incelemeye katılın.

e. CI/CD Pipeline'larını Otomatikleştirin: Pull request'ler tarafından tetiklenen test ve dağıtım süreçlerini otomatikleştirmek için sürekli entegrasyon ve sürekli Dağıtım (CI/CD) pipeline'larını uygulayın.

Branşlar ve pull request'ler kullanarak diğer geliştiricilerle işbirliği yapmak, modern yazılım geliştirmenin temel bir yönüdür. Branşlar, geliştiricilerin özellikler üzerinde bağımsız olarak çalışmasına olanak tanırken, pull request'ler kod incelemesini, geri bildirimi ve ana kod tabanına sorunsuz entegrasyonu kolaylaştırır. En iyi uygulamaları izleyerek ve bu işbirlikçi araçları etkili bir şekilde kullanarak, ekipler üretkenliklerini, kod kalitelerini ve genel proje başarılarını artırabilir.

## Uzak repository'lerdeki çakışmaları çözme

Git ve GitHub, sürüm kontrolünü ve işbirlikçi yazılım geliştirmeyi devrim niteliğinde değiştirmiştir. Ancak, birden fazla geliştirici aynı proje üzerinde eşzamanlı olarak çalıştığında, farklı branşlardan veya fork'lardan değişiklikleri birleştirmeye çalışırken çakışmalar ortaya çıkabilir. Bu çakışmaları verimli bir şekilde çözmek, temiz ve işlevsel bir kod tabanı korumak için gereklidir. Bu makalede, Git ve GitHub kullanarak uzak repository'lerdeki çakışmaları ele alma adımlarını inceleyeceğiz.

Git Çakışmalarını Anlamak:
Çakışmalar, aynı dosya veya kod bölümünde örtüşen değişiklikler nedeniyle Git'in değişiklikleri otomatik olarak birleştiremediğinde meydana gelir. Git çakışan alanları işaretler ve bu çakışmaları manuel olarak çözmek geliştiricinin sorumluluğu haline gelir.

Yerel Bir Branş Oluşturma:
Çakışmaları ele almak için, üzerinde çalışmak istediğiniz uzak repository branşından yeni bir yerel branş oluşturarak başlayın. Aşağıdaki komutu kullanın:
```
git checkout -b my-feature-branch origin/master
```
Bu komut, uzak repository'deki "master" branşından "my-feature-branch" adlı yeni bir branş oluşturur.

Değişiklik Yapma ve Commit Etme:
Şimdi, yerel branşınız üzerinde çalışın ve dosyalarda gerekli değişiklikleri yapın. İşiniz bittiğinde, değişiklikleri commit edin:

```
git add .
git commit -m "Implementing my feature"
```
Uzak Değişiklikleri Pull Etme:
Değişikliklerinizi push etmeden önce, uzak repository'den en son değişiklikleri pull etmek çok önemlidir. Bu, yerel branşınızın güncel olmasını sağlar ve push sırasında çakışma olasılığını azaltır.

```
git pull origin master
```
Çakışmaları Çözme:
Uzaktan değişiklikleri pull ettiğinizde, Git size çakışmalar hakkında bildirimde bulunabilir. Çakışan dosyaları kod düzenleyicinizde açın ve şu gibi bölümler göreceksiniz

Hangi değişiklikleri tutacağınıza veya değiştireceğinize karar vermek için dosyayı manuel olarak düzenleyin. Tüm çakışmaları çözdükten sonra dosyayı kaydedin.

Çözülmüş Dosyaları İşaretleme:
Çakışmaları manuel olarak çözdükten sonra, değiştirilmiş dosyaları stage edin:

```
git add <filename>
```
Çözülmüş Değişiklikleri Commit Etme:
Çakışmaları çözdükten sonra değişiklikleri kaydetmek için yeni bir commit oluşturun:

```
git commit -m "Resolved conflicts"
```
Değişiklikleri Push Etme:
Artık çakışmaları çözdüğünüze göre, yerel branşınızı uzak repository'ye push edin

```
git push origin my-feature-branch
```
Pull Request Oluşturma:
Değişiklikler push edildikten sonra, GitHub'daki repository'yi ziyaret edin ve "my-feature-branch"inizden ana branşa (örneğin, master) bir pull request oluşturun. Bu, ekip arkadaşlarınızın değişikliklerinizi ana kod tabanına birleştirmeden önce incelemesine olanak tanır.

<img alt="Git branching and merging infographic" src="../../../images/Part-04/PR.jpeg" />

İnceleme ve Merge:
Pull request yaptığınız değişiklikleri gösterecek ve ekip üyeleriniz değişiklikleri inceleyebilecektir. Her şey yolundaysa, bir ekip lideri veya bakımcı pull request'i ana branşa merge edebilir.

Git ve GitHub kullanarak uzak repository'lerdeki çakışmaları çözmek, işbirlikçi geliştirmenin ayrılmaz bir parçasıdır. Süreci anlayarak ve bu makalede özetlenen adımları izleyerek, çakışmaları verimli bir şekilde ele alabilir ve temiz ve işlevsel bir kod tabanı koruyabilirsiniz. İşbirlikçi bir yaklaşımı benimsemek ve ekip üyeleri arasında net iletişim, çakışma çözüm sürecini daha da kolaylaştırabilir ve sorunsuz geliştirme iş akışlarını sağlayabilir.