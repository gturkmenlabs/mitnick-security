# Sızma 2: Teröristler işbaşında

## Temel fikir
Bilinmeyen açık olasılığı, yalnızca yama uygulamaya dayanan savunmayı eksik bırakır.

## Uygulama
İnternete açık servisleri hassas ağlardan ayır; erişimleri kısıtla; ana makine ve ağ olaylarını izle; ihlal sonrası etkiyi sınırla.

## Kaçınılacak hata
Çevre duvarının tüm saldırıları durduracağını varsaymak.

## Çalışılmış örnek
Genel erişimli bir sunucu ele geçirilse bile iç sistemlere erişimi ayrı kontroller kısıtlar.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Bölümde aktarılan ağ ihlallerinden yazar, kamuya açık servislerin güvenlik açığına rağmen iç varlıklara erişimin ayrı sınırlanması gerektiği sonucunu çıkarır.

## Kontrol adımları
Dışa açık sistemleri hassas iç sistemlerden ayır; yalnız gereken ağ akışlarını aç; kayıtları güvenli yerde sakla; olay belirtilerine göre araştırma ve müdahale yap.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 48–73; Türkçe çevirinin 2. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Khalid Ibrahim'in ağı** — Kitaba göre sohbet odalarında takma adlarla dolaşan bir kişi, kendisini Pakistanlı militan bir gruba bağlı eski hacker diye tanıtıp gençlere para karşılığı devlet ve askeri sistemleri hedefletti; kimliği hiçbir zaman bağımsız doğrulanmadı.
- **neOh'un ilk görevleri** — Bir üniversitenin öğrenci veritabanı 1000 dolar karşılığında istendi; neOh, öğrencilerle sohbet ortamında kurduğu ilişki sayesinde kullanıcı adı ve parola topladı, çoğu hesapta ikisi aynıydı. Ardından verilen atom araştırma merkezinde makineler ağdan yalıtılmıştı; vaat edilen para hiç ödenmedi.
- **Lockheed Martin ve Boeing** — Lockheed'te yalnızca dış çevre bölgesine kadar ilerleyebildi, iç ağa geçemedi. Boeing'de yamalanmamış bir servisten yararlanıp ağ trafiğini dinledi; parola ve şifrelenmemiş eklerden uçak çizimleri çıktı; kitaba göre kırılma noktası yama eksikliği ve şifresiz e-postaydı.
- **Comrade'nin savunma sistemine yaklaşması** — Savunma kurumuna ait, dışarıdan erişilemeyen bir sisteme ulaştı; makine listesinde binlerce sunucu ve çok sayıda ayrıcalıklı hesap gördü, birkaç gün sonra tutuklandı. İç topolojinin tek bir dosyada açık durması ve sistemin erişilebilir olması koruma sağlamadı.
- **Chameleon'un çeki** — Hükümet ağlarının topoloji haritası karşılığında 1000 dolarlık çek aldı ve bozdurdu; iki hafta sonra FBI sorguladı, haritayı vermediğini söyledi. Anlatıya göre çekin kaynağı bile aydınlanmadı; yabancı bağlantılı ödemeleri izleyen bir kontrol yoktu.
- **SavecOre'un sahte ajanı** — Anlatıya göre "FBI'da amcam var" diyen birinden dokunulmazlık vaadi alan genç, bıraktığı numarayı aradığında kendini Washington'da ajan olarak tanıtan ama belirgin Pakistan aksanı taşıyan biriyle konuştu. Genç, bunun çocukların ihbar edip etmeyeceğini yoklayan kişi olduğu sonucuna vardı; iddia edilen kimlik hiç doğrulanmadı.
- **Beyaz Saray baskını** — Anlatıya göre site bakım sırasında varsayılan ayarlarla çalışırken bir grup genç içeri sızdı; form betiğindeki girdi denetimi eksiğinden yararlanıp sunucuya komut çalıştırttı, ardından yetki yükseltti ve e-posta sunucusuna ulaştı. Yapılandırma, girdi doğrulama ve yama aynı anda çöktü; olay ancak izleme aracı ve bir ihbarla fark edildi.
- **Eligible Receiver ve hapishane teklifi** — 1997 ve 2003 tatbikatlarında "kızıl takım" kısa sürede ulusal sistemlere girip elektrik dağıtımını kontrol edebildi. Yazar, yargılanmayı beklerken bir uyuşturucu baronunun hapishane sistemine girip kendisini kaçırması için büyük para önerdiğini ve bu teklifi reddettiğini aktarıyor.

## Yazarın önerdiği karşı önlemler

- **Yama yönetimi** — Ürünleri güncel sürümde tut; kimin takip edeceğini tanımlayan resmî bir süreç kur, ilgilileri haberdar et ve işi aksatmadıkça yamayı hemen uygula.
- **Derinlemesine savunma** — Sıfır gün açıkları kaçınılmaz sayılmalı; web, posta ve DNS gibi kamuya açık sistemler DMZ'ye alınıp hassas iç ağdan ayrılmalı, böylece bir katman düşse de iç ağ korunmalı.
- **İzleme** — Ağ ve makineler ihlal sonrası davranışlar için gözlenmeli: parola denemeleri, arka kapı, güvenliği gevşeten yapılandırma değişiklikleri, log ve dosya oynanması; bunları haber veren araçlar kurulmalı.
- **Güçlü kimlik doğrulama** — Statik ve varsayılan parola yerine güçlü parola artı tek kullanımlık kod, sertifika, akıllı kart veya biyometri; maliyet ve zahmet, korunan varlığın değerine göre tartılmalı.
- **Etik eğitimi** — Bilgisayar etiği ilkokuldan itibaren verilmeli; yazarın aktardığı ankette öğrencilerin %48'i arkadaşının parolasını ele geçirmeyi önemsiz buluyordu.
- **Muhatabı okumak** — Anlatı düzeyindeki öneri: bir hacker'ın söylediklerinin içeriği kadar tonu ve tutarlılığı da dinlenmeli; bu, iddianın güvenilirliğini anlamaya yardım eder.

## Okuma kapsamı

Kaynağın tamamı okundu; ancak PDF metin çıkarımındaki harf aralığı bozulmaları ve eksik karakterler yüzünden bazı takma adlar, unvanlar ve sayılar belirsiz kaldı.
