# Aldatma Sanatı — 16: Şirket bilgi güvenliği kuralları önerileri

**Kaynak:** Türkçe PDF, dosya sayfaları 447–569. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Yazılı politika, bilgi sınıflandırması, hesaplar, fiziksel güvenlik ve iletişim gibi alanlarda somut süreçlere dönüşmelidir.

## Ne zaman ve nasıl kullanılır?
Kuralları varlık ve iş akışlarına göre uyarla; sorumluları ata; kimlik doğrulama, yetki, parolalar, e-posta, satıcı ve olay bildirimini kapsa; düzenli gözden geçir.

## Çalışılmış örnek
Beklenmeyen bir e-posta eki ve sonraki telefon talebi, bilinen kanaldan teyit edilmeden işleme alınmaz. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Eski bir politika listesini bağlam veya güncel standart kontrolü olmadan aynen uygulamak.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar
* **Microsoft kaynak kodu sızıntısı** — Kitapta aktarıldığına göre saldırganlar, evden/uzaktan çalışan bir şirket personelinin bilgisayarına bulaştırdıkları Truva atı üzerinden kurumun güvenilir geliştirme ağına sızmış ve kaynak kodlarını çalmıştır. Uzaktan bağlanan uç noktalarda kişisel güvenlik duvarı ve güncel zararlı yazılım korumasının bulunmaması, ağ güvenlik kontrollerinin aşılmasına yol açmıştır.
* **Çöpten borsa ve içeriden bilgi sızıntısı** — Anlatıya göre bir sermaye piyasası aracı kurumu çalışanı, kurum çöplerini karıştırarak içeriden öğrenenlerin ticaretine dair gizli şirket içi belgeleri ele geçirmiştir. Hassas evrakın çapraz kâğıt öğütücüden geçirilmeden atılması ve çöplerin şirket alanı dışındaki denetimsiz noktalara bırakılması fiziksel bilgi koruma kontrolünü işlemez kılmıştır.
* **Bütil merkaptan ile sahte acil tahliye** — Sanayi casuslarının ve saldırganların binaya girmek veya odalarda gözetimsiz kalabilmek için zararsız ancak kokulu gaz salarak sahte tahliye alarmı verdikleri taktik aktarılır. Güvenlik görevlilerinin tahliye kargaşasında tuvalet ve odaları tam denetlememesi, saldırganların içeride kalarak sistemlere ve belgelere erişmesine olanak tanımıştır.
* **Santral ve danışma üzerinden güven devşirme** — Saldırganın danışma görevlisine kendi adına not bıraktırıp ardından kurum çalışanını arayarak ana santral numarasını geri arama referansı göstermesi senaryosudur. Görevlinin kimlik sormadan not alması ve hedeflenen çalışanın santralden gelen aktarımı sorgulamadan güvenilir sayması kurumsal doğrulama mekanizmasını devre dışı bırakmıştır.

## Yazarın önerdiği karşı önlemler
* **Dört düzeyli veri sınıflandırması ve varlık sahipliği:** Kurum bilgileri Gizli, Özel, Dahilî ve Genel olarak sınıflandırılmalı; her bilgi varlığı için bir "bilgi sahibi" atanarak saklama, dağıtım ve etiketleme süreçleri yazılı kurallarla belirlenmelidir.
* **Üç aşamalı kimlik ve yetki doğrulama:** Bilgi veya donanım işlemi talep eden kişinin kimliği (arayan numaraya güvenmek yerine rehberden geri arama, ses tanıma veya token ile), şirketteki güncel iş durumu ve bilme gereksinimi (need-to-know) teyit edilmeden işlem yapılmamalıdır.
* **Ayrıcalıklı hesap ve yardım masası denetimi:** Parola sıfırlama, hesap açma ve yetki artırma talepleri mutlaka yazılı/dijital imzalı yönetici onayıyla karşılanmalı; tüm varsayılan üretici parolaları değiştirilmeli ve en düşük yetki ilkesi uygulanmalıdır.
* **Uzaktan çalışanlar için sıkılaştırılmış uç nokta güvenliği:** Ağ dışındaki kullanıcılar için ince istemci (thin client), VPN, kişisel güvenlik duvarı ve otomatik güncellenen antivirüs zorunlu tutulmalı; harici faks ve modem hatlarındaki dışa arama yönlendirmeleri engellenmelidir.
* **Merkezî olay bildirim hattı ve erken uyarı:** Şüpheli aramaların ve toplum mühendisliği girişimlerinin tek merkezde toplanacağı kolay hatırlanır bir hat tahsis edilmeli; sürmekte olan saldırılarda risk altındaki birimlere hızla kurum içi uyarı geçilmelidir.
* **Fiziksel güvenlik ve güvenli imha prosedürleri:** Tesis girişlerinde unvana göre renk kodlu yakalıklar ve refakatçi zorunluluğu uygulanmalı; hassas basılı evraklar çapraz öğütücülerle, manyetik ortamlar ise geri getirilemez biçimde imha edilmelidir.
* **Periyodik farkındalık eğitimleri ve tatbikatlar:** Tüm çalışanlara işe girişte ve yılda en az bir kez tazeleyici bilgi güvenliği eğitimi verilmeli; kurallara uyumu ölçmek için önceden haber verilerek düzenli sosyal mühendislik delme testleri yapılmalıdır.

## Okuma kapsamı
Metnin tamamı taranmış olup harf arası boşluk ve sözcük bölünmesi bozukluklarına rağmen yazarın güvenlik politikası maddeleri ve kuralları bütünüyle anlaşılabilmektedir; anlam kaybına yol açan bir belirsizlik bulunmamaktadır.
