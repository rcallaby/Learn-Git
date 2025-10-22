# Uzak Depolar ile İş Birliği Yapma

- [Uzak depoları ayarlama (GitHub, GitLab, Bitbucket)](#uzak-depolari-ayarlama-github-gitlab-bitbucket)
- [GitHub](#github)
- [GitLab](#gitlab)
- [Bitbucket](#bitbucket)
- [Uzak depolara değişiklikleri gönderme ve çekme](#uzak-depolara-degisiklikleri-gonderme-ve-cekme)
- [Birleştirme Çakışmalarını Yönetme](#birlestirme-cakismalarini-yonetme)
- [En İyi Uygulamalar](#en-iyi-uygulamalar)

## Uzak Depoları Ayarlama (GitHub, GitLab, Bitbucket)

Yazılım geliştirme dünyasında, sürüm kontrol sistemleri kod depolarını yönetmede, iş birliğini kolaylaştırmada ve ekip üyeleri arasında sorunsuz bir çalışma akışı sağlamada kritik bir rol oynar. GitHub, GitLab ve Bitbucket gibi platformlarda barındırılan uzak depolar, geliştiricilere kodlarını merkezi bir konumda saklama, yönetme ve paylaşma olanağı sunar. Bu makalede, her bir platformda uzak depo oluşturma sürecini adım adım ele alacağız.

### GitHub
GitHub, Git tabanlı sürüm kontrolü için en popüler web tabanlı barındırma platformlarından biridir. GitHub’da uzak depo oluşturma adımları şu şekildedir:

#### Adım 1: GitHub Hesabı Oluşturma
Henüz bir hesabınız yoksa, [github.com](https://github.com/) adresine giderek bir GitHub hesabı oluşturun.

#### Adım 2: Yeni Bir Depo Oluşturma
Giriş yaptıktan sonra, GitHub panosunun sağ üst köşesindeki "+ Yeni" düğmesine tıklayın. Depoya bir ad verin, isteğe bağlı bir açıklama ekleyin ve deponun herkese açık (public) mi yoksa özel (private) mi olacağını seçin.

#### Adım 3: Depoyu Başlatma
Depo oluşturulduktan sonra, isteğe bağlı olarak bir README dosyası ile başlatma seçeneğiniz vardır. README dosyası, projeniz hakkında temel bilgiler sağlar ve iş birliği yapanlar için başlangıç noktası görevi görür.

#### Adım 4: Depoyu Klonlama (İsteğe Bağlı)
Depo ile yerel bilgisayarınızda çalışmak istiyorsanız, şu komutu kullanarak klonlayabilirsiniz:

```bash
git clone <repository_url>
```

### GitLab
GitLab, geniş özellik yelpazesi sunan başka bir popüler Git depo yöneticisidir. GitLab üzerinde uzak depo oluşturmak için şu adımları takip edebilirsiniz:

#### Adım 1: GitLab Hesabı Oluşturma
[gitlab.com](https://gitlab.com/) adresine giderek bir hesap oluşturun.

#### Adım 2: Yeni Bir Proje Oluşturma
Giriş yaptıktan sonra, panodaki "Yeni Proje" düğmesine tıklayın. Projeye bir ad verin, isteğe bağlı bir açıklama ekleyin ve görünürlüğünü (herkese açık, dahili veya özel) seçin.

#### Adım 3: Depoyu Başlatma
GitHub’a benzer şekilde, bir README dosyası ile depoyu başlatma seçeneğiniz vardır.

#### Adım 4: Depoyu Klonlama (İsteğe Bağlı)
Depoyu yerel bilgisayarınıza klonlamak için şu komutu kullanabilirsiniz:

```bash
git clone <repository_url>
```

### Bitbucket
Atlassian tarafından sahip olunan Bitbucket, Git depolarını barındıran başka bir yaygın platformdur. Bitbucket’te uzak bir depo oluşturmak için şu adımları takip edin:

#### Adım 1: Bitbucket Hesabı Oluşturma
[bitbucket.org](https://bitbucket.org/) adresine giderek bir Bitbucket hesabı oluşturun.

#### Adım 2: Yeni Bir Depo Oluşturma
Giriş yaptıktan sonra, Bitbucket panosundaki "Depo oluştur" düğmesine tıklayın. Depoya bir ad verin, isteğe bağlı bir açıklama ekleyin ve erişim seviyesini belirleyin (herkese açık veya özel).

#### Adım 3: Depo Türünü Seçme
Bitbucket, Git veya Mercurial arasında seçim yapmanıza olanak tanır. "Git"i seçin.

#### Adım 4: Depoyu Başlatma
GitHub ve GitLab gibi, README dosyası ile başlatabilirsiniz.

#### Adım 5: Depoyu Klonlama (İsteğe Bağlı)
Yerel bilgisayarınıza depoyu klonlamak için şu komutu kullanabilirsiniz:

```bash
git clone <repository_url>
```

GitHub, GitLab ve Bitbucket kullanarak uzak depolar oluşturmak, sürüm kontrol sistemleriyle çalışan her geliştiricinin bilmesi gereken temel bir beceridir. Bu makaledeki adımları takip ederek, uzak depolarınızı kolayca oluşturabilir, başlatabilir ve ekip arkadaşlarınızla iş birliği yaparak projelerinizi geliştirmeye başlayabilirsiniz.

---

## Uzak Depolara Değişiklikleri Gönderme ve Çekme

Sürüm kontrol sistemleri, ekiplerin kod değişikliklerini etkili bir şekilde yönetmesini sağlayan temel araçlardır. Git, geliştiricilere aynı proje üzerinde eş zamanlı çalışabilmeleri için uzak depolara değişiklik gönderme (push) ve çekme (pull) işlemlerini yapma imkanı tanır.

### Uzak Depoyu Anlamak
Uzak depo, geliştiricilerin projelerinin kodunu sakladıkları paylaşılan merkezi bir konumdur. Ekip çalışmasında her üyenin bilgisayarında yerel bir depo bulunur ve uzak depo, değişikliklerin senkronize edilmesini sağlayan merkezi referans noktasıdır.

### Değişiklikleri Uzak Depoya Gönderme
Değişiklikleri uzak depoya göndermek, yerel deponuzdaki kod değişikliklerini uzak depoya aktarma işlemidir.

#### Adım 1: Değişiklikleri Yerel Olarak Commit Etme
Değişiklikleri göndermeden önce, yapılan değişiklikleri commit etmek gerekir:

```bash
git commit -m "Değişiklik açıklaması"
```

#### Adım 2: Uzak Depoyu Doğrulama
Uzak depoları kontrol etmek için şu komutu kullanabilirsiniz:

```bash
git remote -v
```

#### Adım 3: Değişiklikleri Gönderme
Commit edilen değişiklikleri uzak depoya göndermek için şu komutu kullanın:

```bash
git push <remote_name> <branch_name>
```

Örnek:

```bash
git push origin main
```

---

### Uzak Depodan Değişiklikleri Çekme
Uzak depodan değişiklikleri çekmek, uzak depodaki en güncel değişiklikleri yerel deponuza almak anlamına gelir.

#### Adım 1: Yerel Değişiklikleri Commit Etme
Çakışmaları önlemek için değişiklikleri commit etmeniz önerilir.

#### Adım 2: Değişiklikleri Fetch Etme
Uzak depodaki değişiklikleri almak için şu komutu kullanabilirsiniz:

```bash
git fetch origin
```

#### Adım 3: Değişiklikleri Birleştirme
Değişiklikleri yerel dalınıza (branch) birleştirmek için:

```bash
git merge origin/main
```

---

### Birleştirme Çakışmalarını Yönetme
Birleştirme sırasında çakışma oluşursa:

1. Çakışma içeren dosyaları açın.
2. Çakışma işaretlerini (**<<<<<<<, =======, >>>>>>>**) bulun.
3. Çakışmayı manuel olarak çözün ve işaretleri kaldırın.
4. Çakışmaları çözdükten sonra commit işlemi yapın:

```bash
git commit -m "Çakışmalar çözüldü"
```

---

### En İyi Uygulamalar
- **Her zaman önce çek (pull) sonra gönder (push).**
- **Küçük ve açıklayıcı commit mesajları yazın.**
- **Yeni özellikler için ayrı branch kullanın.**
- **Kod incelemelerini teşvik edin.**
- **Sürekli Entegrasyon (CI) araçları kullanın.**

Uzak depolara değişiklikleri göndermek ve çekmek, Git ile iş birliği yapmanın temel unsurlarındandır. Bu süreçleri anlamak ve en iyi uygulamaları takip etmek, ekipler arasında sorunsuz bir geliştirme süreci sağlar.