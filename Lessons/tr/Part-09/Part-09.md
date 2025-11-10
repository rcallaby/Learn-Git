# Github ve Codespaces  

Yazılım geliştirme dünyasında, iş birliği ve sürüm kontrolü, projelerin düzenli bir şekilde yönetilmesini ve kod organizasyonunun sağlanmasını mümkün kılan temel unsurlardır. Popüler bir web tabanlı barındırma hizmeti olan GitHub, geliştiricilerin projeler üzerinde birlikte çalışma biçimini dönüştürmüştür. GitHub ile birlikte, Microsoft’un Codespaces hizmeti, güçlü ve kullanışlı bir bulut tabanlı geliştirme ortamı sunmaktadır. Bu makale, yeni başlayanlar için GitHub ve Codespaces’ı etkili bir şekilde kullanarak sürüm kontrolü ve iş birliği içinde kod yazmayı öğrenmelerine rehberlik edecektir.  

## GitHub ile Çalışmaya Başlama  

### 1.1 Kayıt Olma  
GitHub’a katılmak için [github.com](https://github.com) adresini ziyaret edin ve e-posta adresinizle ücretsiz bir hesap oluşturun. Katkılarınızda sizi tanımlayacak bir kullanıcı adı seçin.  

### 1.2 Depo (Repository) Oluşturma  
Hesabınıza giriş yaptıktan sonra, sağ üst köşedeki “+” simgesine tıklayın ve “Yeni depo (New repository)” seçeneğini seçin. Depoya bir ad verin, isteğe bağlı olarak bir açıklama ekleyin ve deponun herkese açık (public) mı yoksa özel (private) mi olacağını belirleyin. Herkese açık depolar herkes tarafından görüntülenebilirken, özel depolar yalnızca davet edilen iş birlikçileri tarafından erişilebilir.  

### 1.3 Depoyu Klonlama  
Mevcut bir depo üzerinde çalışmak için onu yerel makinenize klonlamanız gerekir. GitHub’daki ilgili depoyu açın ve “Kod (Code)” düğmesine tıklayın. HTTPS veya SSH yöntemlerinden birini seçerek bağlantıyı kopyalayın ve terminalinizde `git clone <URL>` komutunu kullanarak depoyu indirin.  

### 1.4 Dallar (Branch) Oluşturma  
Dallar, değişiklikleri izole etmek ve yeni özellikleri ana kod tabanına dahil etmeden önce test etmek için kullanılır. GitHub’da “Branch” açılır menüsüne tıklayın, yeni dalın adını girin ve Enter tuşuna basın. Artık yeni dal üzerinde çalışmaya başlayabilirsiniz.  

### 1.5 Değişiklik Yapma ve Commit Etme  
Depoyu klonladıktan ve yeni bir dal oluşturduktan sonra kod üzerinde değişiklik yapmaya başlayabilirsiniz. Seçtiğiniz kod düzenleyiciyi kullanarak dosyaları düzenleyin. Değişiklikleri kaydetmek için önce `git add <dosya_adı>` komutuyla aşamaya alın, ardından `git commit -m "Açıklayıcı commit mesajı"` komutunu kullanarak değişiklikleri kaydedin.  

### 1.6 Değişiklikleri Gönderme (Push)  
Yaptığınız değişiklikleri GitHub deposuna göndermek için `git push origin <dal_adı>` komutunu kullanın. Bu komut, mevcut dalınızın güncellenmesini sağlar.  

### 1.7 Pull Request (PR) Oluşturma  
Değişikliklerinizin ana kod tabanına dahil edilmesini istiyorsanız, bir "Pull Request (PR)" açmanız gerekmektedir. GitHub’daki deponuza gidin, “Pull requests” sekmesine tıklayın ve ardından “New pull request” seçeneğini seçin. Yaptığınız değişiklikleri içeren dalı seçin, bir başlık ve açıklama ekleyin ve “Create pull request” düğmesine basın. Takım arkadaşlarınız değişikliklerinizi gözden geçirebilir ve onaylarlarsa ana dala birleştirebilirler.  

## GitHub Codespaces’a Giriş  

### 2.1 Codespaces Nedir?  
GitHub Codespaces, doğrudan tarayıcınız üzerinden erişebileceğiniz, bulut tabanlı bir entegre geliştirme ortamıdır (IDE). Codespaces sayesinde, bağımlılıklar veya yapılandırmalarla uğraşmadan hızla tutarlı bir geliştirme ortamı oluşturabilirsiniz.  

### 2.2 Codespace Oluşturma  
Bir Codespace oluşturmak için, GitHub’daki deponuza gidin ve “Kod (Code)” düğmesine tıklayın. Açılan menüde “Codespaces” sekmesini göreceksiniz. “Yeni Codespace (New Codespace)” seçeneğini seçin ve GitHub, gerekli tüm araçlar ve eklentiler önceden yüklenmiş bir sanal makine oluşturacaktır.  

### 2.3 Codespace Ortamında Çalışma  
Codespace oluşturulduktan sonra, tarayıcı tabanlı bir IDE’ye yönlendirileceksiniz. Burada, tıpkı yerel bir kod düzenleyicisinde olduğu gibi kod yazabilir, düzenleyebilir ve çalıştırabilirsiniz. Terminal erişimi sayesinde commit yapabilir, değişiklikleri itebilir ve tüm Git işlemlerini gerçekleştirebilirsiniz.  

### 2.4 Codespaces ile İş Birliği  
Codespaces, ekip üyeleri arasında kesintisiz iş birliği imkanı sağlar. Takım arkadaşlarınızı Codespace’inize davet edebilir ve gerçek zamanlı olarak birlikte kod yazabilir, inceleyebilir ve düzenleyebilirsiniz.  

### 2.5 Codespaces ve Yerel Geliştirme Karşılaştırması  
Codespaces, yerel geliştirme ortamına kıyasla birkaç önemli avantaj sunar. Farklı makinelerde geliştirme ortamı kurma ihtiyacını ortadan kaldırır ve ekip üyeleri arasındaki uyumluluk sorunlarını azaltır.  

GitHub ve Codespaces, sürüm kontrolü ve iş birliği içinde kod geliştirme süreçlerini dönüştürerek, geliştiricilere her ölçekteki projelerde daha verimli ve etkili çalışma imkanı sunmaktadır. Bu başlangıç kılavuzunu takip ederek, GitHub’ı kolayca kullanmaya başlayabilir, depo oluşturabilir, değişiklikler yapabilir ve Codespaces ile verimli bir şekilde iş birliği içinde çalışabilirsiniz. Bu güçlü araçları keşfedin ve geliştirme sürecinizin daha verimli, üretken ve keyifli hale gelmesini sağlayın.