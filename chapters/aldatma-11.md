# Aldatma Sanatı — 11: Teknolojiyi ve toplum mühendisliğini birleştirmek

**Kaynak:** Türkçe PDF, dosya sayfaları 293–332. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Teknik zayıflıklar ile çalışanların yönlendirilmesi aynı zincirde birleşebilir.

## Ne zaman ve nasıl kullanılır?
İnsan kaynaklı istekleri ve teknik erişim yollarını birlikte modelle; kimlik bilgilerini koru; ayrıcalıkları sınırla ve anormal işlemleri izle.

## Çalışılmış örnek
Telefonla bakım talebi yapılır; görevli kimliği doğrular ve bakım işlemini yetkili sistem üzerinden yürütür. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
İnsan eğitimi veya teknik sertleştirmeden sadece birinin yeterli olduğunu düşünmek.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Tutukevi hattı manipülasyonu** — Kitaptaki anlatıya göre Johnny Hooker, tutuklu suç ortağıyla gizlice görüşebilmek amacıyla resmi kurum yetkilisi ve arıza teknisyeni rollerine bürünerek telefon şirketinden savunma hattındaki gelen arama engelini kaldırtmış, diğer cezaevi görevlilerinden de hücre birimi bilgisini almıştır. Telefon şirketinin geçerli bir iş emri olmaksızın yalnızca yardımseverlik refleksiyle hat parametrelerini değiştirmesi ve cezaevi görevlilerinin arayanın kimliğini doğrulamadan dahili bilgi paylaşması güvenlik denetimini tamamen işlevsiz kılmıştır.
- **Mesai sonrası temizlikçi üzerinden ofise sızma** — Anlatıya göre avukat Ned Racine, hisse fiyatlarını etkileyecek gizli şirket belgelerini kopyalamak için mesai bitiminde takım elbiseli görünümü ve şirket kartvizitiyle temizlik görevlisini anahtarını içeride unuttuğuna ikna ederek binaya girmiştir. Taşeron temizlik personelinin dış görünüşe aldanıp kimlik teyidi yapmaksızın yetkisiz kişileri içeri almaması yönünde eğitilmemesi ve ofis çalışanının parolasını ekrana iliştirilmiş not kâğıdında saklaması koruma mekanizmasını devre dışı bırakmıştır.
- **Güvenlik yarışmasında konsol manipülasyonu** — Yazarın kendi deneyimi olarak aktardığı olayda, uçbirim tabanlı erişim koruması sağladığı iddia edilen bir güvenlik yazılımı, stant görevlisinin sorularla meşgul edilmesi ve donanım kabinindeki basit kilidin açılarak konsol bağlantı kablosunun harici uçbirime aktarılmasıyla aşılmıştır. Üretici ekibin yalnızca mantıksal erişim denetimine güvenerek fiziksel donanımı zayıf bir kilitle savunmasız bırakması ve stant alanını gözetimsiz kılması denetimi boşa çıkarmıştır.
- **Sunucu bilgisi sızdırma ve parola zinciri** — Kitaptaki kurgusal anlatıya göre İvan adlı saldırgan, hedef yazılımın kaynak kodunu barındıran sunucuların adını teknik bakım bahanesiyle şirket içi telefon görüşmeleri yaparak proje liderinden öğrenmiş; ardından sözlük ve kaba kuvvet teknikleriyle elde ettiği hesap yetkilerini diğer sunucularda denemiştir. Kritik altyapı bilgilerinin kimlik doğrulaması yapılmadan telefonda paylaşılması, çalışanların tahmin edilebilir sözlük sözcüklerini parola seçmesi ve aynı parolayı birden fazla sunucuda ortak kullanması sistemin ele geçirilmesine yol açmıştır.

## Yazarın önerdiği karşı önlemler

- **İş emri ve süreç disiplini:** Yetkilendirme veya resmi bir hizmet emri bulunmayan hiçbir hat veya sistem ayarı değişikliği çalışanlarca iyi niyetle dahi yapılmamalı; kuralların esnetilmesini önleyecek caydırıcı denetim mekanizmaları uygulanmalıdır.
- **Bağımsız kimlik doğrulama:** Yüz yüze gerçekleşmeyen her türlü istekte arayanın kimliği bağımsız kanallardan teyit edilmeli; kimlik kesinleşene kadar kamuya açık olmayan hiçbir operasyonel bilgi (sunucu adı, personel konumu vb.) verilmemelidir.
- **Destek ve temizlik personelinin eğitimi:** Taşeron veya kadrolu temizlik ekiplerine mesai saatleri dışında yabancılara kapı açmama, şirket çalışanı izlenimi veren kişileri içeri almama ve refakatsiz geçişlere izin vermeme kuralları açıkça benimsetilmeli, bu hususlar hizmet sözleşmelerine yazılmalıdır.
- **Fiziksel sızma ve açıklık denetimleri:** Güvenlik açıklarını ve temizlik saatlerindeki fiziksel riskleri tespit etmek amacıyla belirli aralıklarla uzman kuruluşlara kontrollü fiziksel içeri girme testleri yaptırılmalıdır.
- **Parola karmaşıklığı ve hesap kilitleme:** Tahmin edilebilir sözlük sözcüklerinin veya kişisel bilgilerin parola yapılması engellenmeli; art arda gelen başarısız giriş denemelerinde hesap kilitleme mekanizmaları devreye alınmalı ve zayıf parola özet algoritmaları kapatılmalıdır.
- **Çalışma alanı ve fiziksel donanım güvenliği:** Parolaların not kâğıtlarına yazılarak ekranlara yapıştırılması önlenmeli; kritik sunucular, konsol terminalleri ve kablo bağlantıları kolay açılabilen kilitler yerine yüksek güvenlikli muhafazalarda kilit altında tutulmalıdır.

## Okuma kapsamı

Metin çıkarımındaki yoğun harf ve sözcük ayrımı bozukluklarına rağmen bölümün tamamı okunmuş, anlatılan vakalar ile yazarın önerileri bağlam bütünlüğü içinde eksiksiz biçimde kavranmıştır.
