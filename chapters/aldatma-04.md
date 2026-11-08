# Aldatma Sanatı — 04: Güven uyandırmak

**Kaynak:** Türkçe PDF, dosya sayfaları 62–86. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
İnandırıcı bir kimlik, samimiyet veya kurum bilgisi karşı tarafta gerçek yetki bulunmasa bile güven hissi yaratabilir.

## Ne zaman ve nasıl kullanılır?
Duygusal güven ile doğrulanabilir kimliği ayır; kurum rehberinden geri ara; gerekiyorsa yetkiyi ilgili bilgi sahibi üzerinden teyit et.

## Çalışılmış örnek
Kurum içinden olduğunu söyleyen ve doğru terimleri kullanan arayan, bağımsız bir kaynaktan teyit edilene kadar hassas bilgi alamaz. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Kandırılmayı zekâ eksikliği sayıp sistem tasarımını ve iş akışını ihmal etmek.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

* **Borç tahsilatı için video kiralama zincirinin aranması (Doyle Lonnegan vakası)** — Anlatıya göre saldırgan, tahsil edilemeyen bir kumar borcunu hedefin kredi kartından tahsil edebilmek amacıyla video kiralama zincirindeki bir çalışanı arayarak başka bir şubenin yöneticisi kimliğine bürünmüştür. Haftalar süren dostane ve sıradan telefon sohbetleriyle güven ilişkisi kurduktan sonra, altyapı arızasını bahane ederek hedefin sistemde kayıtlı kart bilgilerini telefon üzerinden almıştır. Şubeler arası kimlik teyidi yapılmaması ve hassas müşteri verilerinin yalnızca sözlü meslektaş beyanına dayanılarak paylaşılması kontrolün işlemesini engellemiştir.
* **Restoran bahsi ve hızlı kart numarası ele geçirme (Henry vakası)** — Anlatıda bir genç, babasına kredi kartı verilerinin mağazalarda güvende olmadığını kanıtlamak amacıyla yakındaki bir şubeden mağaza yöneticisinin adını ve kodunu öğrenip babasının kayıtlı olduğu şubeyi arar. Sistem arızası ve hatta bekleyen müşteri aciliyeti bahanesini öne sürerek dakikalar içinde babasının adresi, telefon numarası ve kart bilgilerini sözlü olarak elde eder. Çağrı merkezleri veya şubeler arasında bağımsız geri arama mekanizmasının olmaması ve kart bilgilerine erişimde herhangi bir maskeleme bulunmaması kontrol zaafına yol açmıştır.
* **Taahhütsüz promosyon telefonu edinme** — Bir şahıs, operatörün uzun süreli abonelik şartına takılmadan bir sentlik promosyon cihazını alabilmek için zincir mağazanın bir şubesinden nöbetçi satış temsilcisinin adını öğrenmiştir. Ardından diğer şubeyi bu personelin adıyla arayarak satışı ve sözleşmeyi yaptığını ancak stok kalmadığını iddia etmiş, yönlendirdiği alıcıya faturanın kesilip cihazın teslim edilmesini sağlamıştır. Mağazalar arasında resmi sipariş/stok transfer sistemi yerine şifahi meslektaş ricasına itimat edilmesi nedeniyle yetki kontrolü aşılmıştır.
* **Kolluk veri tabanı el kitabıyla sicil sorgulatma (USBM/FBI kılavuzu vakası)** — İnternete sızan ulusal suç bilgi sistemi (USBM) kılavuzunu ele geçiren arayan, dahili sorgu formatlarını ve polis jargonunu öğrenerek yerel emniyet birimini aramıştır. Sistem arızası teyidi bahanesiyle hedef kişi hakkında sorgulama komutu çalıştırtmış ve şahsın dolandırıcılık sabıkasını teyit ettirmiştir. Kurum içi teknik terimleri bilmenin otomatikman yetkili personel sayılması yanılgısı ve rütbe/hiyerarşi algısının sorgulamayı engellemesi kontrolün çökmesine neden olmuştur.

## Yazarın önerdiği karşı önlemler

* **Kredi kartı verilerini saklamaktan kaçınma ve şifreleme:** Şirketler müşteri kart numaralarını dosyalarda tutma uygulamasından vazgeçmeli; zorunlu hallerde ise bu veriler güçlü şifreleme, erişim sınırlamaları ve maskeleme kurallarıyla korunmalıdır *(güncel yorum: PCI-DSS standartları ve tokenizasyon altyapıları)*.
* **Kurum genelinde farkındalık eğitimi:** Sosyal mühendislik eğitimleri yalnızca teknik personele değil, danışma, vezne ve kurye personeli dahil kurumdaki tüm çalışanlara verilmeli; telefonda dostane veya yetkili konuşan kişilerin gerçekte kurum dışı saldırganlar olabileceği öğretilmelidir.
* **Bilgi varlıklarının sınıflandırılması ve risk analizi:** Kurumdaki tüm bilgi varlıkları hassasiyet, önem ve değer derecelerine göre tasnif edilmeli; saldırganların bu varlıkları hedef alırken kullanabileceği aldatma yöntemleri önceden modellenmelidir.
* **Personel için zihinsel kontrol mekanizmaları:** Çalışanlar tanımadıkları birinden gelen bilgi veya işlem talebinde "Bu bilgiyi şirketin en büyük düşmanına verirsem ne olur?" ve "Benden yapılması istenen işlemin olası etkilerinin farkında mıyım?" sorularını sormaya teşvik edilmelidir.
* **Unvan ve otoriteyi bağımsız kanaldan doğrulama:** Kurum içi unvan, rütbe veya teknik terminoloji bilgisinin sorgusuz güven doğurmasının önüne geçilmeli; çalışanların kurum rehberinden geri arama yaparak kimliği teyit etmesi zorunlu kılınmalıdır.
* **İntranet ve harici ağ sınırlarının düzenli denetimi:** Hassas el kitapları, süreç dokümanları ve veri tabanı komutlarının dikkatsizlik sonucu arama motorlarına veya internete sızıp sızmadığı periyodik olarak taranmalı, proxy ve ağ yapılandırmaları sürekli kontrol edilmelidir.

## Okuma kapsamı

Kaynağın tamamı okunmuş olup, Türkçe metin çıkarımındaki yoğun harf ve sözcük arası boşluk bozulmalarına karşın anlatının anlam bütünlüğünü bozan veya belirsiz kalan bir bölüm bulunmamaktadır.
