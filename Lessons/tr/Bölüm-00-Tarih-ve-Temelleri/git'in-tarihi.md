# Git'in Tarihçesi ve Temelleri

- [Tanıtım](#tanıtım)
- [Git'i Kim Oluşturdu](#giti-kim-oluşturdu)
- [Git'in Oluşturulma Nedeni](#gitin-oluşturulma-nedeni)
- [Git'e Alternatifler](#gite-alternatifler)
- [Depolama alanlarınızı ücretsiz olarak nerede saklayabilirsiniz?](#depolama-alanlarınızı-ücretsiz-olarak-nerede-saklayabilirsiniz)

# Tanıtım

Git, Linus Torvalds tarafından 2005 yılında oluşturulan dağıtılmış bir sürüm kontrol sistemidir. Git, geçmişi Team Foundation Sürüm Kontrolü, Perforce veya Subversion gibi merkezi sürüm kontrol sistemlerinden (CVCS) temelde farklı bir şekilde temsil eder. Merkezi sistemler, bir depoda her dosya için ayrı bir geçmiş depolar. Git, geçmişi tüm deponun anlık görüntülerinden oluşan bir grafik olarak depolar. Git'te commits olarak adlandırılan bu anlık görüntülerin birden fazla üst öğesi olabilir ve düz bir çizgi yerine bir grafiğe benzeyen bir geçmiş oluşturur. Geçmişteki bu fark inanılmaz derecede önemlidir ve CVCS'ye aşina olan kullanıcıların Git'i kafa karıştırıcı bulmasının ana nedenidir.

Git, bugün öğrenilmesi önemlidir çünkü dünya çapında geliştiriciler ve şirketler tarafından yaygın olarak kullanılmaktadır. Kod değişikliklerini yönetmek ve projelerde diğer geliştiricilerle iş birliği yapmak için olmazsa olmaz bir araçtır. Git, geliştiricilerin kod üzerinde bağımsız olarak çalışmalarına ve daha sonra hazır olduklarında değişikliklerini birleştirmelerine olanak tanır.

## Git'i Kim Oluşturdu?

Git, 2005 yılında Linux ana sisteminin geliştirilmesi için Linus Torvalds tarafından yazılmıştır. O zamandan beri, diğer ana sistem geliştiricileri de ilk geliştirilmesine katkıda bulunmuştur. Junio Hamano, 2005 yılından beri ana sistemin bakımını üstlenmektedir.

## Git'in Oluşturulma Nedeni

Orijinal ekip, onu kullanmak için özgür lisanslarını kaybettikten sonra, eski bir sürüm kontrol sistemi olan BitKeeper'ı artık kullanamadı. O zamanlar, başka hiçbir Kaynak Kontrol Yönetimi (SCM) dağıtılmış bir sistem için özel gereksinimlerini karşılamıyordu. Yeni sistemin hedeflerinden bazıları hız, basit tasarım, doğrusal olmayan geliştirme için güçlü destek (binlerce paralel dal), tamamen dağıtılmış ve Linux çekirdeği gibi büyük projeleri verimli bir şekilde idare edebilme (hız ve veri boyutu) idi.

## Git'e Alternatifler

Git'e Subversion (SVN), Mercurial (Hg) ve Perforce gibi çeşitli alternatifler mevcuttur.

Subversion, CVS'ye benzeyen merkezi bir sürüm kontrol sistemidir. Kullanımı kolay olduğu ve diğer araçlarla iyi bir entegrasyonu olduğu için genellikle kurumsal ortamlarda kullanılır.

Mercurial, Git'e benzeyen dağıtılmış bir sürüm kontrol sistemidir. Git'ten öğrenmesi daha kolay olduğu için genellikle daha küçük projelerde kullanılır.

Perforce, kurumsal ortamlarda sıklıkla kullanılan merkezi bir sürüm kontrol sistemidir. Büyük dosyalar ve ikili dosyalar için iyi bir desteğe sahiptir.

Bu sistemlerin her birinin kendine özgü güçlü ve zayıf yönleri vardır ve hangisinin kullanılacağına karar vermek projenin özel ihtiyaçlarına bağlıdır. Git, kod değişikliklerini yönetmek ve projelerde diğer geliştiricilerle iş birliği yapmak için temel bir araç olduğu için dünya çapında geliştiriciler ve şirketler tarafından yaygın olarak kullanılır. Git, geliştiricilerin kod üzerinde bağımsız olarak çalışmasına ve hazır olduklarında değişikliklerini bir araya getirmesine olanak sağlar.

## Depolama alanlarınızı ücretsiz olarak nerede saklayabilirsiniz?

Git depolarınızı depolayabileceğiniz internet'te birkaç ücretsiz yer var. İşte en popüler olanlardan birkaçı:

- GitHub
- GitLab
- Bitbucket
- SourceForge

Bu hizmetlerin her birinin kendine özgü güçlü ve zayıf yönleri vardır ve hangisinin kullanılacağına karar vermek projenin özel ihtiyaçlarına bağlıdır. GitHub en popüler hizmettir ve dünya çapında geliştiriciler ve şirketler tarafından yaygın olarak kullanılır. Ücretsiz olarak sınırsız genel depo ve sınırlı sayıda özel depo sunar.

GitLab, ücretsiz olarak sınırsız özel depo sunan bir diğer popüler hizmettir. Bitbucket, beş kullanıcıya kadar ücretsiz olarak sınırsız özel depo sunduğu için genellikle küçük ekipler tarafından kullanılan bir hizmettir. SourceForge, uzun zamandır var olan ve genellikle açık kaynaklı projeler için kullanılan bir hizmettir.