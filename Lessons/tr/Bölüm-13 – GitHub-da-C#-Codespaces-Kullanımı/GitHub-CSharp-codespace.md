# GitHub'da C# Codespaces Kullanımı  

GitHub Codespaces, geliştiricilerin doğrudan GitHub deposu içinde kod yazmalarını, derlemelerini, test etmelerini ve hata ayıklamalarını sağlayan bulut tabanlı bir geliştirme ortamıdır. Takım üyeleriyle işbirliği yapmayı ve projeler üzerinde çalışmayı, karmaşık kurulum veya yapılandırmaya ihtiyaç duymadan kolaylaştırır. Codespaces ile tarayıcınızdan tam yapılandırılmış bir geliştirme ortamına erişebilir, böylece kodunuz üzerinde her yerden çalışabilirsiniz.  

Bu makalede, GitHub'da C# Codespaces kurulumunu ve kullanımını keşfedeceğiz. Ayrıca, C# geliştirmesinde Codespaces'in pratik kullanımını göstermek için örnekler sunacağız.  

### Ön Koşullar  

C# Codespaces'i kullanmaya başlamadan önce aşağıdakilere sahip olduğunuzdan emin olun:  

- **GitHub hesabı:** Codespaces oluşturmak ve kullanmak için bir GitHub hesabına ihtiyacınız var.  
- **C# projesi:** Codespaces ile çalışmak için bir C# projesi hazırlayın. Yeni bir proje oluşturabilir veya mevcut bir projeyi kullanabilirsiniz.  

### C# Codespace Oluşturma  

1. **GitHub deposuna gidin:** Öncelikle, C# projenizin bulunduğu GitHub deposuna gidin.  
2. **"Code" düğmesine tıklayın:** Depo ana sayfasında, yeşil "Code" düğmesine tıklayarak açılır menüyü görüntüleyin.  
3. **"Open with Codespaces" seçeneğini seçin:** Açılır menüden "Open with Codespaces" seçeneğini seçin. Eğer bu depoda daha önce Codespaces kullanmadıysanız, bir yapılandırma dosyası oluşturmanız istenecektir.  
4. **Codespace’i yapılandırın (gerekliyse):** İlk kez Codespaces kuruyorsanız, `.devcontainer` klasörü içinde bir `devcontainer.json` yapılandırma dosyası oluşturmanız istenir. Bu dosya, geliştirme ortamı ayarlarını (çalışma zamanı, uzantılar, bağımlılıklar vb.) tanımlar.  

C# projesi için örnek bir `devcontainer.json` dosyası:  

```json
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:5.0",
  "extensions": [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [5000]
}
```

Bu örnekte, resmi .NET SDK 5.0 imajı kullanılmış ve C# uzantısı yüklenmiştir.  

### C# Codespaces ile Çalışma  

Codespace’inizi kurduktan sonra, GitHub deponuzdaki "Codespaces" sekmesine tıklayarak ona erişebilirsiniz. Listeden uygun Codespace’i seçip "Connect" düğmesine tıklayarak geliştirme ortamınızı tarayıcıda açabilirsiniz.  

Karşınıza, C# uygulamaları geliştirmek için gerekli tüm araçlarla önceden yapılandırılmış olan, tanıdık bir Visual Studio Code arayüzü çıkacaktır.  

#### Örnek: C# Konsol Uygulaması Oluşturma  

Codespaces kullanarak basit bir C# konsol uygulaması oluşturalım.  

1. **Codespace’e bağlanın:** Yukarıdaki adımları izleyerek Codespace’inize bağlanın.  
2. **Terminali açın:** Visual Studio Code'da "Terminal" menüsüne tıklayın ve "New Terminal" seçeneğini seçerek yeni bir terminal penceresi açın.  
3. **Yeni bir C# konsol uygulaması oluşturun:** Terminalde aşağıdaki komutları kullanarak yeni bir C# konsol uygulaması oluşturun.  

```sh
dotnet new console -n MyConsoleApp
cd MyConsoleApp
```

4. **Kod yazın:** `Program.cs` dosyasını açın ve aşağıdaki kodu ekleyin:  

```csharp
using System;

namespace MyConsoleApp
{
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Merhaba, Codespaces!");
        }
    }
}
```

5. **Uygulamayı derleyin ve çalıştırın:** Aşağıdaki komutları kullanarak C# konsol uygulamanızı derleyin ve çalıştırın.  

```sh
dotnet build
dotnet run
```

Terminalde şu çıktıyı görmelisiniz:  

```
Merhaba, Codespaces!
```

### Codespaces ile İşbirlikçi Geliştirme  

Codespaces’in en büyük avantajlarından biri, işbirlikçi geliştirme desteğidir. Birden fazla ekip üyesi aynı proje üzerinde, kendi Codespace ortamlarında çalışabilir. Bu sayede çakışmalar önlenir ve kod değişikliklerini gözden geçirme ve birleştirme süreci kolaylaşır.  

Her geliştirici kendi dalını oluşturup değişikliklerini yapabilir ve ardından bir **pull request** (çekme isteği) göndererek katkıda bulunabilir. İnceleme yapanlar, bu değişiklikleri içeren Codespace’i açarak doğrudan test edebilirler, bu da gözden geçirme sürecini daha verimli hale getirir.  

GitHub Codespaces, C# geliştiricileri için güçlü bir işbirliği platformu sunar. Bulut tabanlı geliştirme ortamı ve kolay kurulum süreci sayesinde, altyapı ile uğraşmak yerine kod yazmaya odaklanabilirsiniz.  

---

# C# Codespaces İçin GitHub Actions Kullanımı  

### Bir Codespace Yapılandırma Dosyası Oluşturma  

İlk olarak, Codespace ortamınızı yapılandırmak için `.devcontainer/devcontainer.json` dosyasına ihtiyacınız olacak. İşte bir örnek:  

```json
{
  "name": "C# Codespace",
  "image": "mcr.microsoft.com/dotnet/sdk:6.0",
  "extensions": [
    "ms-dotnettools.csharp"
  ],
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "forwardPorts": [80]
}
```

Bu yapılandırma, .NET SDK 6.0 imajını kullanır ve Visual Studio Code için C# uzantısını yükler.  

### Bir GitHub Actions İş Akışı YAML Dosyası Oluşturma  

Ardından, bir **GitHub Actions** iş akışı tanımlamak için `.github/workflows/build.yml` dosyasını oluşturun:  

```yaml
name: Build and Test

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - name: Checkout code
      uses: actions/checkout@v2

    - name: Set up .NET
      uses: actions/setup-dotnet@v2
      with:
        dotnet-version: '6.0.x'

    - name: Restore dependencies
      run: dotnet restore

    - name: Build
      run: dotnet build --configuration Release

    - name: Run tests
      run: dotnet test --configuration Release --no-build
```

Bu iş akışı, `main` dalına yapılan değişikliklerde otomatik olarak çalıştırılır. .NET SDK’yı kurar, bağımlılıkları yükler, projeyi derler ve testleri çalıştırır.  

### Değişiklikleri GitHub'a Yükleme  

- `.devcontainer` ve `.github` klasörlerini C# projenizle birlikte GitHub deposuna gönderin.  
- `main` dalına yapılan her gönderimde, oluşturduğunuz **GitHub Actions** iş akışı otomatik olarak çalıştırılacaktır.  

Bu yapılandırma, projenizin sürekli entegrasyon sürecini otomatik hale getirerek daha verimli bir geliştirme ortamı sağlar.