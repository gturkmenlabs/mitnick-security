# Ghost in the Wires — 14: You Tap Me, I Tap You

## Bölüm odağı
Telefon hattı izlemesine ilişkin karşılıklı erişim iddiaları. Bu bölüm birinci kişinin anı anlatısıdır; olaylar ve görüşler yazara atfedilmelidir.

## Uygulama ilkesi
Telefon sistemleri ve izleme yetkilerini ayrıcalık, denetim ve kayıtla koru.

## Kaynaktan örnek
Telefon test ve izleme sistemlerine erişmeye ilişkin yazarın anlatımı yer alır.

## Karar ve uygulama
Bakım sistemlerinde hesap verebilir hesap, görev kapsamı ve erişim denetimi uygula. Kimlik doğrulama ile işlem yetkisini ayrı ele al; doğrulanamayan talepleri bilinen destek kanalına yönlendir.

## Sınır
Bu kısa not bölümün ayrıntılı okumasının yerine geçmez. Tarihsel uygulamaları güncel standartlara karşı değerlendir. Kaynak: İngilizce PDF, dosya sayfaları 109–118.

## Kaynak incelemesinden

Anlatıcı, farklı telefon şirketi çalışanlarının bir arıza ve bakım hikâyesinin farklı parçalarına yanıt verdiklerini, böylece güvenlik birimindeki bir görevlinin gördüğü teknik değişikliklere dayanarak arayana güvendiğini iddia eder. Öyküde ayrıca cihazların üretici varsayılan kimlik bilgilerinin değiştirilmediği belirtilir. Gerçek bir teknik olayın meydana gelmesi, onu bildiren kişinin kimliğini doğrulamaz.

**Uygulama:** Bakım kayıtlarını ve sorumlu ekipleri bağımsız doğrula; bağlantı kesme veya değiştirme işlemlerini onay ve kayıtla sınırla; varsayılan kimlik bilgilerini hizmete almadan kaldır. Olay kanıtı ile kişinin yetkisini ayrı doğrula. Anlatı, özel iletişimi izleme iddiaları içerir; bunu yetkisiz izleme için bir yöntem rehberi olarak kullanma.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

* **Trafik tartışmasında araç sahibinin bulunması** — Anlatıya göre yazar, trafikte tartıştığı sürücünün plakasını kullanarak kamu kurumu çalışanından adres, ardından mobil operatörden telefon numarasını elde etmiştir. Kurumsal müşteri gizliliği ve veri paylaşım denetimlerinin işletilmemesi, kişisel iletişim verilerinin üçüncü şahıslara sızdırılmasına yol açmıştır.
* **Santral görevlileri üzerinden devre izleme zinciri** — Kitaba göre yazar, şirket mühendisi kimliğine bürünerek teknik arıza çözme bahanesiyle farklı santral operatörlerini sırayla devre takibi yapmaya yönlendirmiştir. Geri arama teyidinin yönlendirilmiş bir dahili hatla aşılması ve operatörlerin talep sahibinin kurumsal yetkisini bağımsız kanallardan doğrulamaması kontrol mekanizmalarını işlemez kılmıştır.
* **Saha teknisyenlerinden yetki kodlarının toplanması** — Anlatıcı, sevk merkezinden acil durum bahanesiyle nöbetçi listesini almış; ardından teknisyenleri veritabanı güncelleme bahanesiyle arayarak kullanıcı kimliklerini (UUID) ve teknisyen kodlarını temin etmiştir. Çalışanların kurumsal görünümlü rutin talepleri sorgulamadan yanıtlaması ve yetki doğrulamasının yapılmaması kritik erişim kodlarının ifşasına sebep olmuştur.
* **Güvenlik biriminden dinleme hatlarının tespiti** — Yazar, santral bakım personeli rolüyle şirket güvenlik departmanını arayarak ekipman taşıma gerekçesiyle izleme kutularını geçici olarak devre dışı bıraktırmış, ardından bağlantı testi bahanesiyle dinlenen hatları doğrudan güvenlik görevlisinden öğrenmiştir. Güvenlik biriminin santral içi müdahaleleri çift taraflı teyit etmeden hassas operasyonel verileri paylaşması güvenlik açığı oluşturmuştur.
* **İzleme donanımlarına varsayılan şifreyle erişim** — Anlatıya göre yazar, santral görevlisine arıza testi bahanesiyle hattı kestirdikten sonra izleme cihazlarına uzaktan bağlanmış ve üretici varsayılan PIN kodlarını kullanarak yasal dinlemelere erişim sağlamıştır. Cihazların fabrika çıkışlı kimlik bilgilerinin değiştirilmemiş olması ve oturum açmada çok faktörlü kimlik doğrulamasının bulunmaması kontrolü tamamen etkisiz bırakmıştır.

## Yazarın önerdiği karşı önlemler

* **Geri arama denetimlerinde yönlendirme kontrolü**: Geri arama (callback) güvenlik mekanizması uygulanırken aranan dahili hattın harici bir numaraya veya cep telefonuna çağrı yönlendirme yapıp yapmadığı sistem düzeyinde kısıtlanmalı ve doğrulanmalıdır. (çıkarım)
* **Varsayılan kimlik bilgilerinin değiştirilmesi**: İzleme ve ağ donanımları dahil olmak üzere altyapıya kurulan tüm cihazların fabrika çıkışlı varsayılan PIN ve parolaları devreye alınmadan önce mutlaka değiştirilmeli ve güçlü kimlik denetimi uygulanmalıdır. (çıkarım)
* **Yetki kodlarının ve kimlik bilgilerinin korunması**: Teknisyen kodları, kullanıcı tanıtıcıları (UUID) veya oturum açma anahtarları sözlü iletişimle talep eden kişilere aktarılmamalı; bu tür veriler yalnızca merkezi ve doğrulanmış kimlik sistemleri üzerinden işlenmelidir. (çıkarım)
* **Kritik hat müdahalelerinde çift onay ve iş emri teyidi**: Santral çerçevelerinde fiziksel bağlantı sökme, devre taşıma veya hat kesme gibi operasyonlar telefonla gelen beyanlara göre değil, onaylı resmi iş emirleri ve biletleme kayıtları üzerinden yürütülmelidir. (çıkarım)
* **Yasal izleme süreçlerinin gizliliği ve bilgi ayrımı**: Telefon şirketi güvenlik birimleri yürüttükleri izleme faaliyetlerine ilişkin detayları ve hedef hat bilgilerini teyit edilmemiş personele açıklamamalı; teknik personel ile operasyon personeli arasında görev ayrılığı korunmalıdır. (çıkarım)
* **Müşteri verilerine erişimde en az yetki ilkesi**: Kamu ve telekomünikasyon kayıtlarındaki abone bilgilerine erişim yetkisi sınırlandırılmalı, harici taleplerde sıkı kimlik doğrulama yapılmalı ve tüm sorgulama işlemleri geriye dönük denetim için kayıt altına alınmalıdır. (çıkarım)

## Okuma kapsamı

Bölüm metninin tamamı eksiksiz okunmuş olup, bölüm başındaki şifreli epigraf dışında metin bozukluğundan kaynaklanan herhangi bir belirsiz alan bulunmamaktadır.
