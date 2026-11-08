# Sızma 1: Kumarhanelere sızmak

## Temel fikir
Cihazın fiziksel erişim ve tasarım varsayımları, yazılımın işleyişine ilişkin bilgilerin açığa çıkmasına yol açabilir.

## Uygulama
Varlığı ve fiziksel erişim koşullarını belirle; kurcalamaya dayanıklılığı ve bağımsız güvenlik değerlendirmesini tasarım sürecine dahil et.

## Kaçınılacak hata
Karmaşıklığın veya gizli olduğu düşünülen tasarımın tek başına koruma sağlaması.

## Çalışılmış örnek
Donanım ürünü piyasaya sürülmeden önce fiziksel ve yazılım sınırları birlikte gözden geçirilir.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Kitaptaki vaka, oyun makinesi tasarımında öngörülemez olduğu varsayılan sonuçlarla donanımın incelenebilirliği arasındaki ilişkiyi ele alır. Yazar, sistem tasarımcısının saldırganın fiziksel erişim ve inceleme imkânını hesaba katmasını önerir.

## Kontrol adımları
Donanım ve yazılım varsayımlarını listele; fiziksel erişim altında gizli kalan veya tahmin edilebilen durumu değerlendir; kritik rastgelelik gereksinimlerini uzman incelemesine sok. Basit bir bütünlük denetimini tek savunma sayma.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 21–47; Türkçe çevirinin 1. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Fikrin doğuşu** — Kitaba göre dört danışman, Las Vegas’taki bir konferans sırasında video poker makinelerinin bilgisayar temelli olduğunu fark etti; ilk amaçları kazanç değil, sistemin sınırlarını görmekti. Bu aşamada hiçbir teknik kontrol devrede değildi; merak, sistematik incelemeye dönüştü.
- **Aynı model makineye erişim** — Ekip, hedefledikleri modeli sivil piyasadan edinmek için eyalet uygunluk belgesi ve kimlik gösterdi; satıcıların denetimi yüzeysel kaldı. Makinelerin bireysel kullanıma açık olması, saldırganın hedef donanımı rahatça inceleme ortamına taşımasını sağladı.
- **Ürün yazılımının çözümlenmesi** — Ekip, piyasada uzun süredir bulunan bir modelin ROM’undaki kodu inceledi; üretici kodu gizli veya kurcalamaya dayanıklı tutmamıştı. Kitaba göre patent arşivindeki açıklamalar ve eski teknoloji, incelemeyi kolaylaştırdı; güvenlik “kimse bununla uğraşmaz” varsayımına bırakılmıştı.
- **Rastgelelik yanılgısı** — Yazılımın ürettiği sayılar gerçek anlamda rastgele değildi; belirli bir başlangıç durumundan sonraki değerler hesaplanabilir kalıyordu. İki üretecin birleştirilmesi beklenen karmaşıklığı sağlamadı; tasarımcı, algoritmanın karmaşıklığını tek başına yeterli savunma saydı.
- **Gözlenen çıktıdan durum kestirimi** — Ekip, oyun sırasında görünen kartlardan makinenin iç durumunu tahmin edip kazanç anını hesapladı; bu, rastgelelik iddiasının gözlemlenebilir çıktıyla çürütülmesiydi. Denemelerde yüksek isabet elde ettiler; kontrol, üretilen sayıların dışarıdan görülmesini engellemiyordu.
- **Sahada gizlenen cihaz** — Ekip, hesaplamayı kumarhane dışına taşımak yerine bedende saklanan küçük bir cihazla sahada yürüttü; dikkat çeken davranışları azaltmak için gizleme ve zamanlama kullandı. O dönemki gözetim insan davranışına ve görünür işaretlere odaklandığı için cihazın varlığını yakalayamadı.
- **Yakalanma** — Kitaba göre Marco, kazancı ve el hareketleriyle dikkat çekti; ekip içi seyahat kuralını izlemediği için diğerleri durumu geç öğrendi. Kumarhane onu sorguladı ve kayda aldı, ancak açığını kamuya açmamak için cezai süreç başlatmadı; caydırıcılık hukuktan çok gizliliğe dayandı.
- **Üç yıllık faaliyetin sonu** — Ekip aralıklarla yaklaşık üç yıl kazandı; anlatıya göre Alex yaklaşık 300 bin dolar, diğerleri 400–500 bin dolar civarında kazanç elde etti, ancak toplamlar birbirini tutmuyor. Yakalanma riski arttıkça iş sıradan bir uğraşa dönüştü ve ekip faaliyeti bıraktı.

## Yazarın önerdiği karşı önlemler

- Saldırıya dayanıklı chip ürünleri seç; piyasadaki birçok chip’in kurcalanma riski yüksektir.
- Chip’i tek kart üzerine gömülü biçimde paketle; bağımsız parça olarak sökülememesi gerekir.
- Chip’i epoksiyle kapat; üzerine alüminyum tozu ekleyerek ısıtarak sökme girişimini bozacak bir bariyer oluştur.
- BGA paketleme kullan; bağlantıları kenarlarda değil alt yüzeyde tutarak sinyal ölçümünü zorlaştır.
- Chip türü ve üretici bilgilerini sil; bu bilgiler saldırganın inceleme yolunu kısaltmasın.
- Yazılımda checksum veya hash denetimi bulundur; ancak yazar bunun deneyimli saldırganca atlatılabileceğini ve tek başına yeterli olmadığını belirtir.
- Geliştirme sürecine en iyi güvenlik danışmanlarını kat; geliştiricileri güncel tehditlerle eğit ve ürün tesliminden önce güvenlik durumunu doğrula.

## Okuma kapsamı

Kaynağın verilen metninin tamamı okundu; optik karakter bozulmaları bazı cümlelerde ve kazanç toplamlarında belirsizlik bıraktı, ancak ana olay örgüsü ve öneriler izlenebildi.
