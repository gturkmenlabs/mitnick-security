# Aldatma Sanatı — 13: Zekice oynanmış oyunlar

**Kaynak:** Türkçe PDF, dosya sayfaları 360–387. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Birden fazla kanal veya aracı kullanılarak normal görünen geri arama ve iletme adımları kötüye kullanılabilir.

## Ne zaman ve nasıl kullanılır?
İstek sahibinin verdiği numaraya güvenme; önceden kayıtlı numarayı kullan; yönlendirme ve dosya iletimi için alıcıyı ve yetkiyi doğrula.

## Çalışılmış örnek
Tanımadığı kişi kendisine gelen belgeyi başka bir numaraya iletmesini ister; görevli bağımsız teyit olmadan iletmez. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Bir belgenin kurum içine geldiğini görüp son alıcının da yetkili olduğunu varsaymak.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Starbeat Havacılık ve Sahte Arayan Kimliği** — Jack Dawkins adlı saldırgan, PBX santral ayarlarını değiştirerek ekranda New York Genel Müdürlüğü numarasını gösterip finans biriminden Linda'yı arar; Genel Müdür'ün toplantısı gerekçesiyle ve e-postasının çalışmadığını öne sürerek gizli finansal veriler ile Apache projesi tahminlerini faksla ister. Finans görevlisi ekrandaki arayan kimliğine güvenmiş, talep sahibinin yetkisini ve kimliğini bağımsız bir kanaldan doğrulamadan hassas belgeleri iletmiştir.
- **Radyo İstasyonu ve Kişisel Numara Manipülasyonu** — Anlatıya göre yazar, meşguliyeti sebebiyle tanımadığı çağrıları açmayan radyo program yöneticisi David'e ulaşmak amacıyla PBX santrali üzerinden arayan numara bilgisini yöneticinin ev telefonu veya holding numarası olarak göstererek çağrıyı açtırır. Hedef kişi arayan kimliğinde tanıdık veya otorite simgeleyen bir numara gördüğünde çağrıyı sorgulamadan yanıtlamıştır.
- **Kredi Kartı Şirketinde Sesli Mesaj İstismarı** — Kimlik hırsızı Shirley Cutlass, telekomünikasyon birimini arayıp başka bir şube personeli kimliğiyle geçici bir sesli mesaj kutusu ve dahili numara açtırır; ardından müşteri hizmetlerini arayıp teknik sorun bahanesiyle kurbanın finansal bilgilerini bu dahili sesli mesaja bırakmalarını sağlar. Görevliler sesli mesaj tahsisi için yazılı onay aramamış, müşteri hizmetleri de arayanın şirket içi dahili hatta sahip olmasını güvenilirlik için yeterli görmüştür.
- **Rudolfo Gemicilik ve Faks Yönlendirmesi** — Robert Jorday adlı korsan, yönetim sekreteri Janet'ı AR-GE yöneticisi kimliğiyle arayarak modem üzerinden sunucuya bağlanmak için gereken aylık parolanın yazılı olduğu şirket içi notu kaybettiğini söyler ve notun başka bir binadaki danışma faksına (aslında e-postaya yönlendiren sanal faks servisine) fakslanmasını ister. Sekreter yardımseverlik refleksiyle hareket etmiş, belgenin kurum içi bir faks numarasına yönlendirildiğini varsayarak alıcıyı ve talep sahibini teyit etmemiştir.
- **Trafik Mahkemesi Duruşma Ayarlaması** — Hız cezası alan Paul Durea, emniyet celp bürosunu avukat rolüyle arayarak ceza kesen polis memurunun izin ve eğitim takvimini öğrenir; ardından mahkeme kâtibine iş seyahati mazereti sunarak duruşma tarihini memurun eğitimde olacağı güne aldırır. Emniyet celp birimi arayan avukatın yetkisini doğrulamadan memurun takvimini paylaşmış, duruşma günü memur hazır bulunmadığı için dava düşmüştür.
- **Lambeck İmalat ve Sahte İmzalı Yetki Talebi** — Terfi alamayan şirket sekreteri Samantha Gregson, iş arkadaşının parolasını omuz gezintisiyle izleyip öğrenir; ardından yöneticisinin imzasını eski bir evraktan fotokopiyle kopyalayarak BT birimine yetki artırımı talep eden sahte bir faks çeker ve mesai sonrası yeni ürün Cobra 273'ün gizli bilgilerini diskete kaydeder. BT birimi faksla gelen yetki artırımını yöneticiyle bağımsız kanaldan doğrulamamış, ayrıca kullanıcı parolası gözetlemeye karşı fiziksel olarak korunmamıştır.

## Yazarın önerdiği karşı önlemler

- **Arayan kimliği göstergesine güvenmeme:** Ekrandaki arayan numarası (Caller ID) santral ayarlarıyla kolaylıkla değiştirilebildiğinden, kurum dışından gelen çağrılarda kimlik tespiti için asla güvenilir bir veri kabul edilmemelidir.
- **Bağımsız kanal ve geri arama kontrolü:** Hassas bilgi ve işlem taleplerinde arayanın kimliği ve yetkisi, kurum rehberindeki kayıtlı numaradan geri aranarak ya da kişinin yöneticisine danışılarak doğrulanmalıdır.
- **Sesli mesaj ve telefon hizmetlerinde yazılı onay:** Telefon hizmetleri ve sesli mesaj kutusu tahsisleri için yazılı form doldurulması zorunlu tutulmalı; form personelin yöneticisi tarafından onaylanmalı ve yetkili yönetici imzayı teyit etmelidir.
- **Yetki artırımı ve hesap açma kontrolleri:** Yeni hesap açma veya yetki yükseltme talepleri, yalnızca talepte bulunan yöneticinin rehberdeki kayıtlı numarasından doğrudan sözlü onayı ya da dijital imzalı güvenli e-posta doğrulaması alındıktan sonra işleme konmalıdır.
- **Otomatik Numara Tanımlayıcısı (ANI) kullanımı:** Kurum dışı aramalarda kimlik teyidi gerekiyorsa, manipüle edilebilen arayan kimliği yerine telekom şirketinin faturalandırma amacıyla sağladığı ANI verisi tercih edilmelidir.
- **Kişisel sesli mesaj denetimi:** Çalışanlar kendi sesli mesaj kutularını düzenli aralıklarla kontrol etmeli; kendilerine ait olmayan yabancı bir selamlama mesajı ile karşılaştıklarında olası bir toplum mühendisliği müdahalesini bildirmelidir.
- **Tüm personele yönelik savunma bilinci:** Danışma, sekreterya, santral ve idari personel dahil olmak üzere bilgisayar erişimi olsun ya da olmasın tüm çalışanlara eğitim verilmeli; kimliği doğrulanamayan taleplere doğrudan "hayır" diyebilme yetkinliği aşılanmalıdır.

## Okuma kapsamı

Metin çıkarımındaki sözcük ve harf arası boşluk bozulmalarına rağmen bölümün tamamı eksiksiz okunmuş, anlam kaybı veya belirsizlik yaratan bir bölüme rastlanmamıştır.
