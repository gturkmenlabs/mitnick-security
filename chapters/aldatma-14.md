# Aldatma Sanatı — 14: Sanayi casusluğu

**Kaynak:** Türkçe PDF, dosya sayfaları 388–421. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Kaynak kodu ve iş sırları, çalışanların dosya iletme ve erişim kararlarından etkilenir.

## Ne zaman ve nasıl kullanılır?
Hassas varlıkları belirle; erişimi ve dosya paylaşımını sınırla; alıcıyı ve iş gerekçesini doğrula; olağan dışı aktarımları incele.

## Çalışılmış örnek
Sıradan adlı bir dosya kurum içi gibi görünen bir adrese istenir. Görevli dosya sınıfını ve alıcının yetkisini teyit eder. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Dosya adı veya iç ağ görünümünü içeriğin ve alıcının güvenli olduğuna kanıt saymak.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Yedek saklama şirketinden bant sızdırma** — Bir dedektif ekibi, aleyhine toplu dava açılan şirketin savunma hukukçularına ait yedekleme bantlarını ele geçirmek amacıyla üçüncü taraf saklama şirketinin ofisine gece fiziksel olarak sızmış ve yetkili teslimat kütüğüne sahte bir isim eklemiştir. Ertesi gün bu sahte kimlikle arayıp kurye yönlendirerek şifrelenmemiş bantları teslim almış, verileri kopyalayıp kasetleri iade etmiştir. Üçüncü taraf sağlayıcının gevşek fiziksel güvenliği, parolasız yerel işletim sistemi ve verilerin şifrelenmeden saklanması nedeniyle denetim mekanizması tamamen işlemez hale gelmiştir.
- **Yüz yüze sahte iş ortağı kurgusu** — Bir sanayi casusu, üst yöneticisinin şehir dışında olduğunu önceden öğrendiği bir teknoloji şirketine şık ve güvenilir bir kurumsal ortak kılığıyla bizzat gitmiş, lobi görevlisini ve kilit çalışanları etkileyerek öğle yemeğine çıkarmıştır. Yemekte çalışanlardan proje ayrıntılarını topladıktan sonraki gün yöneticinin adıyla arayıp acil durum bahanesiyle kaynak kodunun genel bir ücretsiz e-posta adresine iletilmesini istemiştir. Çalışanların yüz yüze oluşturulan güvene aldanması, alıcı e-posta adresinin şirket dışı niteliğini sorgulamaması ve yönetici teyidini bağımsız kanaldan almaması kontrollerin çökmesine neden olmuştur.
- **Kurum içi basamaklandırma (birdirbir) ile kaynak kodu kaçırma** — İki öğrenci, intikam amacıyla bir yazılım şirketinin denizaşırı geliştirme merkezini arayarak sunucu çökmesi ve sistem yöneticisinin öfkesi bahanesiyle yardım istemiş ve kaynak kodunun şirketin başka bir şubesindeki herkese açık FTP alanına aktarılmasını sağlamıştır. Ardından diğer şubedeki operatörü arayarak ağ arızası bahanesiyle bu masum adlı dosyayı harici bir hedef IP'ye yönlendirterek hedef makineye sızdırmıştır. Çalışanların kurum içi transfer görünümüne güvenmesi, talep sahibinin yetkisini doğrulamaması ve zararsız dosya adı nedeniyle verinin niteliğini araştırmaması istismarı mümkün kılmıştır.

## Yazarın önerdiği karşı önlemler

- **Yedeklerin uçtan uca şifrelenmesi:** Fiziksel bantlarda veya çevrim içi saklanan tüm şirket verileri şifrelenmeli; şifreleme ve geri yükleme prosedürlerinin çalıştığı düzenli olarak denetlenmelidir.
- **Hizmet sağlayıcıların güvenlik denetimi:** Verilerin emanet edildiği üçüncü taraf saklama ve arşiv firmalarının kendi fiziksel güvenlik, kimlik doğrulama ve veri koruma standartlarının kurum standartlarıyla eşdeğer olduğu kontrol edilmelidir.
- **Kriptografik anahtar yönetimi:** Şifreleme anahtarları ve parolalar kasa veya kilit altında korunmalı; tek bir personelin ayrılması veya iş göremez hale gelmesi riskine karşı en az iki kişi süreci bilmeli ve anahtara erişimi olan biri işten ayrıldığında anahtarlar derhal değiştirilmelidir.
- **Şahsen tanınmayan kişilere dosya gönderim yasağı:** Gönderilecek hedef kurumun dahili ağında görünse dahi, yönetim onayı bulunmadıkça şahsen tanınmayan ve kimliği teyit edilmeyen kişilere dosya iletilmemelidir.
- **Fiziksel varlık ve yüz yüze etkileşim şüphesi:** Saldırganların sahte kimlik kartları veya kartvizitlerle bizzat ofise gelebileceği unutulmamalı; dış görünüş ve profesyonel tavır kimlik doğrulamanın yerine geçmemelidir.
- **Dosya aktarım taleplerinde bağımsız doğrulama:** Şirket dışı adreslere (özellikle genel web posta servislerine) veya FTP alanlarına hassas dosya ve kaynak kodu aktarımı talepleri, talimatı verdiği iddia edilen makamdan bağımsız bir kanalla doğrulanmadan yerine getirilmemelidir.

## Okuma kapsamı

Kaynak metindeki yoğun harf ve sözcük ayrımı bozukluklarına rağmen bölümün tamamı okunmuş, vakalar ve yazarın güvenlik önerileri belirsizlik kalmaksızın çözümlenmiştir.
