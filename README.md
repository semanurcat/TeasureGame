# TeasureGame

Otonom Hazine Avcısı, nesne yönelimli programlama ve veri yapıları bilgisini pekiştirmek ve göstermek amacıyla tasarlanmış bir oyundur. Bu oyunda, otomatik olarak hareket eden bir karakter, rastgele oluşturulmuş haritada yer alan hazineleri ve engelleri aşarak tüm hazineleri en kısa sürede toplamaya çalışır. Oyuncunun amacı, karakterin tüm hazineleri en etkili şekilde toplayabilmesi için verimli bir algoritma kullanmaktır.

## Kurulum ve Yükleme

### Gereksinimler
- Java Development Kit (JDK) 8 veya daha yeni bir sürüm
- Herhangi bir Java IDE'si (örn., IntelliJ IDEA, Eclipse, NetBeans)

### Kurulum Adımları
1. Repoyu klonlayın veya proje dosyalarını indirin.
2. Projeyi tercih ettiğiniz Java IDE'sinde açın.
3. JDK'nın proje ayarlarında doğru şekilde ayarlandığından emin olun.
4. Bağımlılıkların çözülmesi için projeyi derleyin.

## Oyunun Başlatılması

Oyunu başlatmak için `Main` sınıfını çalıştırın. Bu, harita boyutlarını girebileceğiniz ilk pencereyi açacaktır. Map boyutlarını girdikten sonra, "Yeni Harita Oluştur" butonuna tıklayarak yeni bir harita oluşturabilir ve oyunu başlatabilirsiniz.

## Oyun Mekanikleri

- **Harita Oluşturma**: Başlangıçta, kullanıcıdan harita boyutları istenir. Harita, Kış ve Yaz olmak üzere iki temaya ayrılmıştır. Her tema, özel statik ve dinamik engeller içerir.
- **Karakter Hareketi**: Karakter, haritada otomatik olarak hareket eder ve herhangi bir engelle çarpışmadan tüm hazine sandıklarını toplamayı hedefler. Yol bulma algoritması, tüm hazineleri etkin bir şekilde toplamak için en kısa yolu hesaplar.
- **Engeller**: Harita, statik (örn., ağaçlar, dağlar, kayalar) ve dinamik (örn., kuşlar, arılar) engeller içerir. Dinamik engeller belirlenen bir alanda hareket eder ve karakterin yolunu değiştirebilir.
- **Hazineler**: Dört tür hazine sandığı vardır: altın, gümüş, zümrüt ve bronz. Bunları toplamak, karakterin ana hedefidir.

## Mimari ve Uygulama

- **Sınıflar**: Proje, `Character`, `Location`, `Obstacle` gibi birçok sınıfı içerir. Her sınıf, oyunun bir bölümünün işlevselliğinden sorumludur ve nesne yönelimli programlama prensiplerini takip eder.
- **Yol Bulma Algoritması**: En kısa yolu bulma algoritması, projenin kritik bir parçasıdır. Karakterin tüm hazineleri etkin bir şekilde toplayabilmesini sağlar. Bu algoritma, verimliliği ve performansı artırmak için sürekli olarak optimize edilebilir.
- **Grafikler ve Kullanıcı Arayüzü**: Oyun, grafiksel kullanıcı arayüzü için Swing kullanır, haritayı, karakteri, engelleri ve hazineleri gösterir. Haritanın görünümü, tema (Kış veya Yaz) göre değişir.

## Dikkat Edilmesi Gerekenler

- **Assets Klasörü**: Projede kullanılan görseller ve diğer kaynaklar, doğrudan proje dosyaları içinde bulunmaz. Bu nedenle, `assets` klasörünün konumunun IDE'de veya çalıştırma ayarlarınızda doğru şekilde ayarlandığından emin olun. Genellikle bu klasör, projenin kök dizininde bulunur ve oyun içinde doğru yolu referans alacak şekilde konfigüre edilmelidir.

