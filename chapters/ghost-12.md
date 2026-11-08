# Ghost in the Wires — 12: You Can Never Hide

## Bölüm odağı
Güvenlik uzmanı ve Eric hakkında bilgi arayışı. Bu bölüm birinci kişinin anı anlatısıdır; olaylar ve görüşler yazara atfedilmelidir.

## Uygulama ilkesi
Rol yapma ve kişisel fırsat iddiaları karşısında bilgi talebini bağımsız doğrula.

## Kaynaktan örnek
Yazar bir uzmanla temas kurma ve Eric hakkında daha fazla bilgi edinme çabalarını anlatır.

## Karar ve uygulama
Beklenmedik mesleki fırsat veya içeriden bilgi iddiası karşısında kimliği ayrı kanaldan doğrula. Kimlik doğrulama ile işlem yetkisini ayrı ele al; doğrulanamayan talepleri bilinen destek kanalına yönlendir.

## Sınır
Bu kısa not bölümün ayrıntılı okumasının yerine geçmez. Tarihsel uygulamaları güncel standartlara karşı değerlendir. Kaynak: İngilizce PDF, dosya sayfaları 96–103.

## Kaynak incelemesinden

Yazar, güvenlik araştırmacısı Neill Clift'e tanıdığı bir şirket çalışanı gibi ulaştığını; konuşmadaki bir tutarsızlığın ve sesinin ayrı bir kaynaktan karşılaştırılmasının şüpheyi artırdığını anlatır. Başka bir öyküde eski bir üretici çalışana ulaşılması, şirket içi gibi görünen bir geri arama numarası ve teknik terimlerin bir araya getirilmesiyle bilgi istendiğini söyler. İsim, iç hat görünümü ve konu bilgisi tek başına kimlik doğrulama değildir.

**Uygulama:** Güvenlik açığı veya teknik mimari bilgisi için isteyen kişinin doğrulanmış kimliğini, erişim yetkisini ve alıcı kanalını ayrı kontrol et. Geri arama numarası üzerinde değişiklik yapılabiliyorsa bunu da koruma kapsamına al. Teknik ayrıntılar tarihsel sistemlere ilişkindir; karşı önlem değerlendirmesinde güncel mimariyi incele.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

* **VMS güvenlik açıkları arayışı** — Anlatıya göre yazar, telekomünikasyon operatöründen gizli numarasını elde ettiği bağımsız araştırmacı Neill Clift'i arayarak kendisini DEC şirketinde çalışan gerçek bir VMS yazılım mühendisi olarak tanıtmış ve güvenlik açığı ayrıntılarını istemiştir. İşe alım fırsatı ve teknik kılavuz vaadiyle güven telkin edilmeye çalışılmış, ancak görüşmedeki bir tutarsızlık üzerine araştırmacının kayıtlı bir mülakat kasetinden yazarın sesini teşhis etmesiyle girişim engellenmiştir.
* **SAS protokol belgelerinin eski geliştiriciden sızdırılması** — Anlatıya göre yazar, hat dinleme yeteneği sağlayan telekomünikasyon altyapısının (SAS) iletişim protokollerini temin etmek amacıyla sistemin geliştiricisi olan ve kapanmış şirketin eski baş mühendisine ulaşmıştır. Kendisini gerçek bir telekom mühendisi olarak tanıtıp şirket içi santral yönlendirmesi ve teknik jargonla güven sağlamış; karşı tarafın kurumsal yetki ve kimlik teyidi yapmaması nedeniyle teknik dokümanlar harici bir faks ve posta kutusuna aktarılmıştır.
* **Kiralık posta kutusu tahsisinde kimlik kontrolünün aşılması** — Anlatıya göre yazar, taklit ettiği mühendis adına gönderilen dokümanları alabilmek amacıyla posta kutusu kiralama acentesinden doğrulanmamış kimlikle kutu tahsis ettirmiştir. Cüzdanının çalındığı ve kimlik belgelerini beklediği bahanesiyle aciliyet hissi oluşturulmuş; ticari işletmenin müşteri kazanma güdüsü ve istismara açık iyi niyeti nedeniyle yasal kimlik ibrazı kuralı işletilmemiştir.
* **SAS geri arama güvenliğinin atlatılması** — Anlatıya göre hatta uzaktan ses erişimi sağlayan donanım birimi, yalnızca belleğindeki önceden yetkilendirilmiş numaraları geri arayacak şekilde tasarlanmış bir güvenlik denetimine sahipti. Yazar, dış arama hattını önceden meşgul edip sahte çevir sesi taklidi ile sistemin çağrıyı harici hatta bağlamasını sağlamış; doğrulama tasarımının yalnızca aranan numara listesine dayanıp hat bütünlüğünü ve fiziksel sinyali doğrulamaması kontrolü boşa çıkarmıştır.
* **Fiziksel hat ve santral manipülasyonuyla arayan numara tespiti** — Anlatıya göre yazar, telefon numarasını gizleyen bir tanıdığının iletişim bilgilerini öğrenmek için bir iş merkezinin telefon dağıtım panosundaki kabloları gizlice ofis hattına bağlamış ve santral yönetiminden arayan numara gösterme özelliğini yetkisizce etkinleştirmiştir. Hedefe çağrı cihazı üzerinden yem bir numara bırakılarak geri araması sağlanmış; bina içi fiziksel hatların sahipsizliği ve santral konfigürasyon yetkisinin kötüye kullanılması hedefin numarasını açığa çıkarmıştır.
* **Hat Tahsis Merkezinden (MLAC) abone adresi temini** — Anlatıya göre yazar, telefon şirketinin hat tahsis birimini arayarak kendisini sahada çalışan bir teknisyen olarak tanıtmış ve elde ettiği bir numaranın kablo bilgileri ile abonenin açık adresini talep etmiştir. Saldırgan rastgele bir teknisyen kodu uydurmuş ve kurum içi terminolojiyi ustalıkla kullanmış; operatörün iletilen personeli veritabanından teyit etmeden doğrudan bilgi paylaşması kontrol zafiyetine yol açmıştır.

## Yazarın önerdiği karşı önlemler

* **Bağımsız kanaldan kimlik ve ses teyidi:** Kurum dışından gelen veya olağandışı teknik bilgi talep eden kişilerin kimliği yalnızca beyanlarına ya da arayan numara görüntüsüne göre doğrulanmamalı, bağımsız ve güvenilir kanallar üzerinden çapraz teyit sağlanmalıdır. (çıkarım)
* **Hassas doküman ve mülkiyet paylaşımında sıkı kontrol:** Eski çalışanlar veya harici danışmanlar, şirket içi teknik mimari veya protokol dokümanlarını talep eden kişilere resmi onay ve doğrulanmış şirket e-postası haricinde (faks, kargo vb.) kesinlikle bilgi aktarmamalıdır. (çıkarım)
* **Hizmet sözleşmelerinde istisnasız kimlik doğrulaması:** Posta kutusu, telekomünikasyon veya benzeri fiziksel/dijital aracı hizmet sağlayıcıları, kayıp veya aciliyet gibi duygusal mazeretlere bakılmaksızın yasal kimlik belgesi ibrazı şartını katı biçimde uygulamalıdır. (çıkarım)
* **Kriptografik ve çok katmanlı geri arama doğrulaması:** Geri arama (call-back) mekanizmaları yalnızca basit hat meşguliyeti veya analog ton algısına güvenmemeli; uç birimler arasında kriptografik el sıkışma ve oturum bütünlüğü kontrolü yapılmalıdır. (çıkarım)
* **Fiziksel dağıtım panoları ve santral erişim güvenliği:** Binalardaki telekomünikasyon dağıtım terminalleri kilit altında tutulmalı ve santral yazılımı konfigürasyon değişiklikleri yetkilendirme ve denetim izine (audit log) bağlanmalıdır. (çıkarım)
* **İç destek ve tahsis merkezlerinde kimlik doğrulama zorunluluğu:** Saha teknisyenleri veya kurum çalışanları kritik veri tabanlarından abone bilgisi talep ettiğinde, sözlü kod beyanı yerine sistem üzerinden iki faktörlü veya dinamik yetki doğrulama mekanizmaları işletilmelidir. (çıkarım)

## Okuma kapsamı

Kaynağın tamamı okunmuştur; yalnızca bölüm başındaki şifrelenmiş kısa epigraf dışında metinde analizi engelleyen bir bozukluk veya belirsizlik bulunmamaktadır.
