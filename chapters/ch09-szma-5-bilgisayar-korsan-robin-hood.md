# Sızma 5: Bilgisayar korsanı Robin Hood

## Temel fikir
Kurum içinde güvenilir görünen kaynaklar ve erişim yolları kötüye kullanılabilir.

## Uygulama
Açıkta kalan sistemleri ve hassas bilgileri envanterle; erişim yetkilerini ve olay kayıtlarını gözden geçir; dışardan erişilebilir yüzeyi sınırla.

## Kaçınılacak hata
Ünü veya iddia edilen niyeti, yetki ve güvenilirliğin kanıtı saymak.

## Çalışılmış örnek
Güvenlik ekibi erişim zincirini ve gerçekten erişilebilen veriyi değerlendirir.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Adrian Lamo vakasında kamuya açık kayıtlar ve alan adı bilgileriyle birlikte erişim yollarının ortaya çıkması tartışılır. Yazarın etik ve zarar hesabına ilişkin değerlendirmesi kendi görüşüdür.

## Kontrol adımları
Kamuya açılması gereken bilgilerle iç ağ kayıtlarını ayır; DNS bölge aktarımını yalnız yetkili sunuculara sınırla; ifşa edilen iletişim bilgilerini kimlik doğrulama yerine kullanma.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 125–150; Türkçe çevirinin 5. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Kurtarma bahanesi** — Anlatıya göre Lamo, polisin dikkatini çektiğinde sorgulanmak yerine mahsur kalan bir kedi için yardım isteyerek odağı değiştirdi. Dış görünüşe dayalı şüphe, yardım talebi karşısında işlemedi; bu, sonraki sosyal çerçeveleme yaklaşımının erken örneği olarak sunulur.
- **Excite@Home açık proxy ve destek sistemi** — Kitaba göre şirketin yanlış yapılandırılmış açık proxy sunucusu, iç destek sayfalarına kimlik doğrulaması olmadan erişim sağladı. Adresi bilenin çalışan sayıldığı varsayımı yüzünden müşteri parolaları ve destek kayıtları açıkta kaldı.
- **Dial-up kullanıcıları ve açık paylaşımlar** — Anlatıya göre ters DNS sorguları ve öngörülebilir adlandırma, çalışanların dial-up makinelerini ortaya çıkardı; parolasız paylaşımlar iç ağa kapı açtı. Meşru görünen ticari uzaktan yönetim yazılımı, imza tabanlı kötü amaçlı yazılım denetimini atlattı.
- **Unutulmuş ama ağa bağlı sunucu** — Kitaba göre kullanımdan kaldırılan ama ağdan ayrılmayan eski bir makine içeri giriş için yetti. Envanter ve kullanımdan kaldırma süreci işlemediği için kimsenin bakmadığı sistem açık kaldı.
- **MCI WorldCom** — Anlatıya göre açık proxy sunucularından iç ağa giren Lamo, iki aylık keşfin ardından insan kaynakları sistemine ulaştı. Kamuya açık kimlik ve doğum tarihi bilgileriyle parola sıfırlama mümkündü; tek kimlik bilgisinin kurum genelinde geçerli olması zayıflığı büyüttü.
- **Microsoft sipariş sayfası** — Kitaba göre kimlik doğrulaması istemeyen ve sahipliği belirtilmeyen bir sipariş sayfası, müşteri işlem bilgilerini dışarıya açtı. Denetim, sayfanın gizli olduğu varsayımına dayandığı için erişim kontrolü sağlanamadı.
- **The New York Times** — Anlatıya göre herkese açık kayıtlar, port taraması ve e-posta başlığındaki iç IP sızıntısı keşif zincirini başlattı; unutulmuş eski bir iç site, serbest metin kabul eden arama arayüzü ve eski sürüm işbirliği veritabanı zinciri tamamladı. Kısa, kişisel bilgilerden türetilen ve her sistemde aynı olan parolalar erişimin kurum geneline yayılmasını kolaylaştırdı.
- **AOL tedarikçisi** — Kitaba göre bir telekomünikasyon tedarikçisini telefonla arayan Lamo, yalnızca doğru numarayı bilmesi sayesinde güvenilir sayıldı ve ağ topolojisi bilgilerine ulaştı. Kimlik bağımsız olarak doğrulanmadı; arayanın içeriden olması gerektiği varsayımı yeterli görüldü.

## Yazarın önerdiği karşı önlemler

- **Herkese açık kayıtları küçültün.** Whois benzeri dizinlerde yalnızca santral numarası ve genel e-posta adresi bulundurun; santral görevlilerini bilgi taleplerini ayırt edecek şekilde eğitin. Departman adresleri ve çalışan adları, kullanıcı adı ve parola tahmini için ipucu verir.
- **Alan adı kayıt bilgilerini sınırlayın.** Kitap, iletişim bilgilerinin gizlenebildiği kayıt hizmetlerini önerir; amaç veriyi tümüyle yok etmek değil, saldırganın işini zorlaştırmaktır.
- **İç ve dış DNS'i ayırın.** Dışarıya yalnızca kamuya açık kayıtları sunan ayrı bir sunucu kullanın; iç ana bilgisayar adları dışarıya sızmasın, donanım ve işletim sistemi bilgisi veren HINFO kayıtları yayımlanmasın.
- **Bölge aktarımını kısıtlayın.** Aktarım yalnızca güvenilir ikincil sunuculara izinli olsun; güvenlik duvarı 53 numaralı TCP portunu varsayılan olarak kapatsın. (güncel yorum: bu önlemler bugün de standart denetim maddeleri arasındadır.)
- **Adlandırmayı ve e-posta başlıklarını temizleyin.** İç makinelere işlevini açıkça söyleyen adlar vermeyin, iç adları dış DNS kayıtlarından çıkarın; SMTP sunucusu dışarı giden iletilerdeki iç IP ve ana bilgisayar bilgisini filtrelesin.
- **Proxy'leri ve kurulumları denetleyin.** Proxy yalnızca iç arayüzde dinlesin, özel IP aralıkları kullanılsın, dışa erişim HTTP/HTTPS ile sınırlansın; kullanıcıların farkında olmadan kurduğu proxy'ler dahil yetkisiz servisler düzenli taranmalı ve yapılandırma sınanmalıdır.

## Okuma kapsamı

Bölüme ait kaynak metnin tamamı okundu; ancak PDF çıkarımındaki harf düşmeleri ve bozulmalar nedeniyle bazı cümlelerdeki ayrıntılar ve geçiş ifadeleri belirsiz kaldı.
