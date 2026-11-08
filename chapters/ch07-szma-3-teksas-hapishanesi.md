# Sızma 3: Teksas hapishanesi

## Temel fikir
İçeriden fiziksel erişim ve paylaşılan hesaplar bireysel sorumluluğu ve güvenlik sınırlarını zayıflatır.

## Uygulama
Kişiye özgü hesaplar kullan; oturumları kilitle; fiziksel erişimleri sınırlayıp gözden geçir; ayrıcalıkları iş ihtiyacına göre ver.

## Kaçınılacak hata
Paylaşılan kimlik bilgileri ile işlemlerin kime ait olduğunun anlaşılacağını varsaymak.

## Çalışılmış örnek
Ortak çalışma alanında her kullanıcı kendi hesabıyla işlem yapar ve ayrılırken oturumunu kilitler.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Cezaevi ortamındaki vaka, fiziksel yakınlık ve hesap kullanımına ilişkin kontrol eksikliklerini inceler. Yazar ortak hesapların sorumluluğu belirsizleştirdiğini ve açık oturumların riski artırdığını vurgular.

## Kontrol adımları
Kişiye özgü hesap, ekran kilidi, erişim kayıtları ve fiziksel bölge sınırını birlikte uygula. İstisna gerekiyorsa gerekçe, onay ve sona erme zamanı kaydet.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 74–97; Türkçe çevirinin 3. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Mutfağa sokulan donanım** — Kitaba göre William, mutfak işini "kalenin anahtarı" sayıp yemek karşılığında ayrıcalık ve malzeme sağladı; parçalar el arabalarıyla ve bir gardiyanın hediyesiyle içeri girdi. Denetim, mahkumun kurduğu sistemlerin gözden geçirilmemesi ve personelin kişisel ilişkiyle kural dışına çıkması yüzünden işlemedi.
- **"Yüzbaşı için çalışıyorum" bahanesi** — William bakım personelinden ağ kablosu edindi ve kanalların açılmasını sağladı; kimse bu yetki iddiasını doğrulamadı. Yetkinin çapraz kontrol edilmemesi, fiziksel altyapıya erişimi fiilen serbest bıraktı.
- **Memurun verdiği hesap bilgisi** — Anlatıya göre bir memur, bağlanamadığı bilgisayarı kurdursun diye mahkuma kullanıcı adı ve parolasını verdi. "Mahkumlar ağa çıkamaz" varsayımı, kimlik bilgisinin paylaşılmasını ve hesabın sahibinden başkasınca kullanılmasını engellemedi.
- **Unutulmuş telefon prizleri** — Danny, kimsenin izlemediği kullanılmayan hatları bularak kendi bağlantısını kurdu; bir ara hattı fakslarla paylaşınca meşgul şikayetleri ortaya çıktı. Hat ve priz envanterinin tutulmaması, kullanım dışı altyapıyı görünmez bir giriş noktasına dönüştürdü.
- **Kutuların altındaki sunucu** — İndirdiklerini kendi makinesinde tutmamak için odasındaki bir bilgisayarı depolama sunucusu olarak kullandı. Mahkum alanındaki cihazların envanteri ve denetimi olmadığından bu düzenek fark edilmedi.
- **Personel masalarının izlenmesi** — İki mahkum, uzaktan yönetim yazılımıyla başka bilgisayarları izleyip personelin hesap bilgilerini ve ne zaman uzakta olacağını öğrendi; yazılımın iz bırakmayacak biçimde değiştirilmesi fark edilmeyi geciktirdi. Yazılım bütünlüğü denetimi ve oturum gözetimi yoktu.
- **İç hattan dışarı çıkış** — Kurumun uzak erişim hizmeti, iç telefon hattından gelen bağlantıya güvendi; mahkumlar önce izindeki personelin, sonra satın alınan bir hesabın kimliğiyle dışarı çıktı. Ağ bölümlendirmesi ve hesap sahipliği denetimi eksikti.
- **Görülüp de kanıtlanamayan ihlal** — Bir gardiyan ekranda hareket eden imleci gördü, bir başkası meşgul telefon hattından şüphelendi; ikisi de kanıt bulamadı. Olay sonrası kayıt ve kanıt üretmeyen kontrol, şüpheyi eyleme dönüştüremedi.

## Yazarın önerdiği karşı önlemler

- **Hesap verilebilirlik:** Ortak hesap ve parola paylaşımı tamamen yasaklanamıyorsa bile teşvik edilmemeli; işlemlerin kime ait olduğu izlenebilmeli. (Güncel yorum: kişiye özgü hesaplar ve çok faktörlü doğrulama bu ilkenin bugünkü karşılığıdır.)
- **Ekran kilidi ve çok hedefli ortam:** Çalışanlar masadan ayrılırken oturumu kilitlemeli; kitap bunun IT tarafından merkezi yapılandırmayla zorunlu kılınmasını önerir.
- **Parola yönetimi:** Kurumun ürettiği tahmin edilebilir desenler yerine, kullanıcının belirlediği ve kolay tahmin edilemeyen parolalar kullanılmalı.
- **Fiziksel erişim ve ziyaretçi denetimi:** BIOS parolası, oturum kilidi, kimlik kontrolü, giriş kayıtları, kamera ve kartlı geçiş; kayıtlar düzenli olarak gözden geçirilmeli.
- **Boş iş istasyonları ve ağ prizleri:** Kullanılmayan prizler devre dışı bırakılmalı, boşalan odalardaki cihazlar güvenli duruma alınmalı.
- **Personel gözetimi:** İşten çıkarılan ya da görevi değişen kişilerin erişimi önceden sınırlandırılmalı; yoğun veri kopyalama ve taşınabilir medya kullanımı izlenmeli.
- **Yetkisiz donanım ve yazılım denetimi:** Onaysız cihaz yasağı, gerektiğinde USB portlarının kapatılması; yetkisiz kablosuz erişim noktası, tuş kaydedici ve yazılım için düzenli tarama, yazılım envanteri ve bütünlük denetimi.
- **Görevler ayrılığı ve en az yetki:** Kritik işlemler ikinci bir kişi tarafından doğrulanmalı; kullanıcılar ve programlar yalnızca gereken yetkiyle çalışmalı.

## Okuma kapsamı

Kaynağın bu bölümünün tamamı okundu; yalnızca OCR kaynaklı harf, ad ve sayı bozuklukları (örneğin "Darmy" yazımı ve bazı ölçü/süre ifadeleri) nedeniyle birkaç ayrıntı belirsiz kaldı.
