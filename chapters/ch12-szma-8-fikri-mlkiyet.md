# Sızma 8: Fikri mülkiyet

## Temel fikir
Kaynak kodu, yedekler ve uygulamalar çevre savunması aşıldıktan sonra da korunmalıdır.

## Uygulama
Hassas ağ segmentlerini ayır; uygulamaları güvenli yapılandır ve gözden geçir; yedekleri, erişimleri ve günlükleri koru.

## Kaçınılacak hata
Güvenlik duvarının izin verdiği uygulama servislerinin güvenli olduğunu varsaymak.

## Çalışılmış örnek
Kaynak kodu deposuna erişim sınırlanır ve anormal indirmeler incelenir.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
İki uzun süreli girişim anlatısında kaynak kodu ve diğer değerli bilgiler hedef alınır; yazar güvenlik duvarına ek olarak uygulama, yedek ve iç ağ kontrollerini tartışır.

## Kontrol adımları
Varlıkları ve veri akışlarını belirle; uygulama güvenliğini ve veri deposu izinlerini değerlendir; yedekleri koru; hassas ağ segmentleri arasındaki erişimi kısıtla.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 191–229; Türkçe çevirinin 8. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Erik'in iki yıllık hedef avı** — Anlatıya göre Erik, elinde olmayan son sunucu yazılımının kaynak kodunu almak için bir yazılım üreticisini aylarca izledi. İlk erişimi, sunucuda açıkta bırakılan yapılandırma dosyalarındaki düz metin veritabanı parolası ve tahmin edilebilir ana makine adlandırması sağladı; yedek sunucunun gereğinden geniş yetkileri yayılmayı kolaylaştırdı. Kontroller işlemedi çünkü parola kalıpları öngörülebilirdi ve yedek sistemler asıl sistemler kadar sıkı korunmuyordu.

- **CEO'nun dizüstü bilgisayarı** — Erik, sabit IP kullanan üst yöneticinin makinesini uzun aralıklarla yoklayarak buldu ve kalıplı ama güçlü görünen bir parolayı tahmin etti. Makinedeki kişisel güvenlik duvarı, tarayıcıya tanınan geniş izin üzerinden atlatıldı. Kontrol işlemedi: güvenlik duvarı tek başına yeterli sayıldı ve ürettiği kayıtlar düzenli okunmadı.

- **Tanılama formu üzerinden komut çalıştırma** — Anlatıya göre bir web tanılama formunun girdiyi doğrulamaması, sunucuda rastgele sistem komutu çalıştırmaya imkân verdi. Geliştiricilerin gece yedeklerini web kökünde bırakması, kaynak kodun dışarı çıkarılmasını kolaylaştırdı. Girdi denetimi ile yedek saklama disiplini birlikte eksikti.

- **Yakalanma ve geri dönüş** — Bir yönetici günlüklerde olağan dışı etkinliği fark edip dosyaları sildi, ancak parola değişikliği, kapsamlı inceleme ve bildirim gibi adımlar atılmadı. Erik bir ay sonra aynı yollardan geri döndü. Kontrol işlemedi: olay müdahalesi yarım kaldı ve erişim yolları kapatılmadı.

- **Şifreli arşivin açılması** — Erik, şifreli kaynak arşivini bilinen düz metin saldırısıyla açtı; arşivdeki bir görsel dosyanın aynı sürümü hedefin halka açık sitesinde korumasız duruyordu. Anlatıya göre bu karşılaştırma kısa sürede arşiv parolasını verdi. Arşiv şifrelemesi tek başına yeterli sanılmıştı.

- **Robert ve e-posta listesi hırsızlığı** — Anlatıya göre Robert, bir abonelik listesi uygulamasının kaynak arşivini yanlış yapılandırılmış bir sunucuda buldu; kurulum betiğindeki doğrulama eksikliğini kullanarak listeleri ele geçirdi ve bunları spam göndericisine verdi. Kurulum dosyalarının sunucuda bırakılması ve betik girdisinin denetlenmemesi belirleyiciydi.

- **Yardım masası uygulamasının değiştirilmesi** — Yanlış yapılandırılmış dosya yayımlama izinleri, uygulama dosyalarının okunup değiştirilmesine imkân verdi. Robert uygulamayı tersine mühendislikle inceledi, girdi denetimini devre dışı bırakıp geri yükledi ve veritabanı sorgusu enjeksiyonuyla yönetici yetkisi aldı. Bütünlük denetimi olmadığı için değişiklik fark edilmedi.

- **Açık yedek paylaşımı ve parola yeniden kullanımı** — Bir yöneticinin korumasız ağ paylaşımındaki kişisel e-posta arşivi, kurum içi yetki haritasını ve düz metin parolaları açığa çıkardı. Aynı parolanın birden çok yerde kullanılması ve okunabilir bir dış parola dosyası, etki alanı yöneticisi düzeyine kadar tırmanmayı sağladı. Yedeklerin ve paylaşımların korunmaması zincirin başlangıcıydı.

## Yazarın önerdiği karşı önlemler

- Güvenlik duvarında yalnızca iş gereksinimi olan servisleri açık tut; durum denetimli güvenlik duvarı kullan ve kural ile günlükleri düzenli olarak yeniden gözden geçir. VPN erişimini istemci IP'siyle sınırlamayı ve paylaşılan anahtar yerine daha güçlü kimlik doğrulamayı değerlendir.
- Veritabanı sunucularını gereksiz yere internete açma, varsayılan portu filtrele ve uzaktan erişim sağlayan genişletilmiş saklı yordamları kapat.
- Süreç, zamanlanmış görev, dosya bütünlüğü, hesap ve günlük denetimlerini düzenli yap; anormal saatlerdeki erişimi ve web günlüklerindeki yetkisiz dosya isteklerini incele.
- Uygulama ve betik dosyalarının bütünlüğünü otomatik araçlarla izle; web yayımlama izinlerini (özellikle FrontPage/WebDAV) sıkı yapılandır.
- Betik, toplu iş dosyası ve kaynak kodda düz metin parola bulundurmayı kurumsal politika düzeyinde yasakla; hassas kaynak kodunu şifreli disklerle koru.
- Parolada öngörülebilir kalıpları yasakla, eski/zayıf parola özetlerinin saklanmasını devre dışı bırak, varsayılan yönetici ve konuk hesaplarını yeniden adlandır, Windows'ta parola önbelleklemesini kapat.
- Hassas bilgi içeren ağ paylaşımlarını ve yedekleri koru; yedeklerin erişilebilirliğini sınırla. Bölünmüş DNS ile iç ana makine adlarının dışarı sızmasını önle.
- Derinlemesine savunma uygula: halka açık sistemleri ayrı ağ segmentlerine taşı ve hassas segmentlere giden trafiği ikinci bir güvenlik duvarıyla filtrele. SQL enjeksiyonuna karşı dinamik sorgu yerine saklı yordam ve ayrı yetkili hesaplar kullan; kurulum betiklerini kurulum sonrası sil.

## Okuma kapsamı

Kaynağın tamamı okundu; ancak Türkçe metin çıkarımındaki harf aralığı bozulmaları ve Çince çeviri kaynaklı isim/araç yazımları (örneğin parola kırma araçlarının adları ve bazı özel adlar) nedeniyle bu ayrıntılarda belirsizlik kaldı.
