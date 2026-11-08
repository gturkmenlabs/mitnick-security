# Aldatma Sanatı — 12: İşe yeni girenlere saldırılar

**Kaynak:** Türkçe PDF, dosya sayfaları 333–359. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Yeni çalışanlar kurumun bilgi sınıfları, rol sınırları ve istisna süreçlerini henüz tanımayabilir.

## Ne zaman ve nasıl kullanılır?
İlk erişimden önce rol odaklı eğitim ver; yeni çalışanlara açık doğrulama ve danışma yolları sun; ayrıcalıkları ihtiyaca göre ver.

## Çalışılmış örnek
Yeni çalışan bir yönetici adı kullanılarak gelen beklenmedik talebi, işe giriş eğitiminde öğrendiği kanaldan teyit eder. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Deneyimsiz çalışanı bilgi değerini kendiliğinden anlamaya bırakmak.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Güvenlik görevlisi aracılığıyla arka kapı yerleştirme** — Kitaptaki anlatıya göre saldırgan, bir stajyeri film senaryosu bahanesiyle manipüle ederek içeriden teknik bilgi almış; ardından gece nöbetindeki güvenlik görevlisini araç arızası ve acil durum bahanesiyle kandırarak kritik sisteme uzaktan komut girdirmiştir. Görevlinin bilgi güvenliği eğitimi almamış olması ve fiziksel erişim yetkisine sahip olduğu hâlde komutların doğuracağı riskleri öngörememesi kurumsal kontrolün işlemesini engellemiştir. Saldırgan bu sayede fiziksel giriş yapmadan kurum içi personeli aracı olarak kullanmış ve işletim sistemi dağıtımına arka kapı yerleştirmiştir.
- **Sahte satıcı desteğiyle uzaktan erişim yetkisi alma** — Anlatıya göre saldırgan, teknik destek görevlisini arayıp yetkili yazılım satıcısı rolüne bürünmüş ve kritik veri kaybını önleme gerekçesiyle acil yama yüklenmesi bahanesiyle sisteme uzaktan erişim kimlik bilgilerini istemiştir. Dış satıcıların kimliğini doğrulayacak resmî bir prosedürün bulunmaması ve personelin aciliyet ile korku baskısıyla kimlik bilgilerini doğrudan paylaşması nedeniyle kontrol mekanizması devreye girmemiştir. Böylece saldırgan, hiçbir fiziksel müdahale gerekmeden doğrudan teknik personel üzerinden uzaktan erişim sağlamıştır.
- **Yeni çalışana casus yazılım kurdurma** — Kitaba göre saldırgan, insan kaynaklarından kart yenileme bahanesiyle yeni başlayan personelin listesini almış; ardından şirket yöneticisinin adını kullanarak henüz kurumu tanımayan yeni bir sekreterden yönetici bilgisayarına meşru görünümlü bir casus yazılım dosyasını açtırmıştır. Yeni çalışanın hiyerarşik otoriteye itaat etme ve göze girme isteği, bilgi güvenliği kurallarını bilmemesi ve sistemlerde casus yazılımlara yönelik tespit denetimlerinin eksikliği istismara zemin hazırlamıştır. Bu yöntemle saldırgan, yönetici ofisinde bulunmadığı sırada hedef sisteme sessizce casus yazılım yerleştirerek ticari müzakere bilgilerini ele geçirmiştir.

## Yazarın önerdiği karşı önlemler

- **Yetkisiz bilgisayar kullanımını yasaklayan temel kural**: Çalışanların tanımadıkları kişilerin taleplerini yerine getirmek için bilgisayar sistemlerini kullanmaları şirket politikasıyla kesin olarak yasaklanmalı; başka birinin cihazında işlem yapılması yalnızca kimlik doğrulaması ve yönetici onayıyla sınırlandırılmalıdır.
- **Güvenlik kuralını uygulayan personele yönetim desteği**: Çalışanlar üst düzey bir yönetici kimliği öne sürülse dahi şahsen tanımadıkları kişilere doğrudan yardım etmemeleri konusunda eğitilmeli; yönetim, güvenlik protokollerine uymak adına yöneticilere itiraz eden personeli cezalandırmak yerine desteklemelidir.
- **Fiziksel güvenlik personeline bilgi güvenliği eğitimi**: Tüm tesise kilit ve anahtar erişimi bulunan güvenlik görevlileri ile benzer personele yalnızca fiziki güvenlik değil, kendilerine yönelebilecek sosyal mühendislik taktiklerini ve bilgi güvenliği risklerini tanıma eğitimi verilmelidir.
- **Teknoloji satıcıları için belirlenmiş irtibat kişileri**: Şirketteki her teknoloji sağlayıcısıyla temas kuracak belirli kurumsal sorumlular tanımlanmalı; diğer çalışanların dış satıcılardan gelen doğrudan bilgi veya donanım/yazılım değişiklik taleplerine yanıt vermesi engellenmelidir.
- **Casus yazılımlara karşı çift düzeyli koruma**: Standart antivirüslerin ticari casus yazılımları zararlı olarak görmeyebileceği dikkate alınarak sistemlerde özel casus yazılım tespit programları kullanılmalı, düzenli taramalar yapılmalı ve çalışanlar şüpheli indirmeler ile e-posta eklerine karşı bilinçlendirilmelidir.
- **Ekran ve oturum kilitleme zorunluluğu**: Çalışanların masalarından kısa süreli ayrılmalarında dahi cihazlara yetkisiz fiziksel erişimi engellemek amacıyla şifreli ekran koruyucu veya oturum kilitleme mekanizmaları zorunlu kılınmalıdır.

## Okuma kapsamı

Metin çıkarımındaki yoğun harf ve sözcük ayrımı bozukluklarına rağmen kaynağın tamamı okunmuş, anlatılan üç ana vaka ile yazarın önerdiği karşı önlemler bağlam kaybı olmaksızın bütünüyle anlaşılmıştır.
