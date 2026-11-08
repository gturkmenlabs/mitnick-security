# Ghost in the Wires — 03: Original Sin

## Bölüm odağı
Telefon şirketi, kişisel bilgiler ve erken sistem erişimleri. Bu bölüm birinci kişinin anı anlatısıdır; olaylar ve görüşler yazara atfedilmelidir.

## Uygulama ilkesi
Arayanın iddia ettiği görev, kişisel verilerin açıklanması için yeterli kanıt değildir.

## Kaynaktan örnek
Yazar telefon şirketinin güvenlik görevlisiyle karşılaşmayı ve ardından bazı sistemlere eriştiğini anlatır.

## Karar ve uygulama
Kimlik doğrulama ve kişisel bilgi erişimini sadece telefonla beyan edilen unvana bağlama. Kimlik doğrulama ile işlem yetkisini ayrı ele al; doğrulanamayan talepleri bilinen destek kanalına yönlendir.

## Sınır
Bu kısa not bölümün ayrıntılı okumasının yerine geçmez. Tarihsel uygulamaları güncel standartlara karşı değerlendir. Kaynak: İngilizce PDF, dosya sayfaları 25–34.

## Bölümün ayrıntılı okuması

- Anlatıcı, kurumsal bir çalışanın kimliğine bürünerek geliştirici sisteminde hesap oluşturulduğunu ve erişim elde edildiğini anlatır. Buradaki savunma dersi, yeni hesap oluşturma ve ayrıcalık atamasının yalnız telefonla bildirilen kimliğe dayanmamasıdır.
- Bir başka vaka, teknik destek ve veri kaybı korkusunu ilişkilendirir. Yazarın anlatımında sistem yöneticisi, sözde acil yardım talebi üzerine yönetici erişimi sağlar. Kurum, destek talebini ayrı kanaldan doğrulayıp hizmet sağlayıcıya geçici ve denetlenebilir erişim vermelidir.
- Sonraki olaylar, birden fazla kişinin erişimi ve soruşturmayı içerir. Yazar bazı zarar iddialarına itiraz eder; onun yorumunu bağımsız olarak doğrulanmış sonuca dönüştürme.

## Uygulama sınırı

Güvenlik incelemesinde teşvik edici aciliyet, iddia edilen rol, talep edilen yetki ve doğrulanan kanalı ayrı ayrı kaydet. Erişim elde edilmesi ile sonra yaşanan zararın kime atfedileceği farklı kanıt sorularıdır.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **DMV sorgu kodu ve kolluk kimliği manipülasyonu** — Anlatıya göre yazar, polis memuru ve ardından idari personel rollerine bürünerek California DMV'nin kolluk kuvvetlerine özel telefon hattını ve sisteme erişim sağlayan yetkilendirme kodunu temin etmiştir. Hassas kişisel verilere erişimde personelin yalnızca arayanın sözlü beyanına ve statik bir talep koduna güvenmesi, geri arama veya resmi kanaldan doğrulama işletilmemesi nedeniyle kontrol mekanizması işlememiştir.
- **Çağrı yönlendirici (diverter) istismarı ve şebeke izlemesi** — İşletmelerin mesai dışı çağrı yönlendirme cihazlarındaki mantıksal bir açık kullanılarak yetkisiz dış aramalar ve sosyal mühendislik süreçleri için geri arama hatları ayarlanmıştır. Cihazlarda harici aktarımları kısıtlayan bir denetim bulunmaması istismara zemin hazırlamış, ancak operatörün şebeke trafiğini dinleyip izlemesi sonucunda yetkisiz kullanım tespit edilerek hat sonlandırılmıştır.
- **Fiziksel tabela değişikliğiyle sahte hat aboneliği** — Hizmeti feshedilen anlatıcı, kapı numarasını fiziksel olarak değiştirip telefon şirketine yeni bir daire eklendiğini bildirmiş ve uydurma bir kimlikle ("James Bond") yeni telefon hattı açtırmıştır. Şirketin adres ve altyapı güncellemelerini resmi tapu veya idari kayıtlar yerine yalnızca müşteri beyanına ve yerindeki fiziki tabelaya göre yapması kontrolü boşa çıkarmıştır.
- **DEC "The Ark" sisteminde geliştirici kimliğine bürünme** — Anlatıcı, sistem üreticisinin santralini arayıp baş geliştirici Anton Chernoff kimliğiyle sistem yöneticisinden silinen test hesabının açılması bahanesiyle ayrıcalıklı hesap ve çevirmeli ağ parolası almıştır. Kitaba göre yönetici, kritik yetkilere sahip hesap ve parola tanımlama işlemini kurumsal bir doğrulama kanalı yerine yalnızca isim aşinalığına ve telefon beyanına güvenerek onaylamıştır.
- **Bloodstock Research yetkisiz erişimi ve federal soruşturma** — Tanıdık bir kullanıcının yasal müşteri hesabı üzerinden şirketin sistemine girilerek işletim sistemi düzeyinde yetki yükseltme yapılmıştır. Müşteri hesaplarında asgari yetki ve rol kısıtlamalarının bulunmaması ilk sızmayı kolaylaştırmış; ancak olağan dışı saatlerde yapılan oturumların sistem izleme süreçlerince fark edilmesiyle vaka FBI'a intikal etmiştir.
- **U.S. Leasing veri kaybı korkutmasıyla yönetici parolası temini** — Anlatıcı, üreticinin teknik destek personeli kimliğiyle sistem yöneticisini arayarak kritik bir işletim sistemi hatası nedeniyle veri kaybı yaşanacağı bahanesiyle uzaktan yama yapmak için yönetici parolasını almış ve arka kapı yerleştirmiştir. Korku ve aciliyet hissinin yetkili servis teyidi refleksini bastırması kontrolün çökmesine yol açmış; anlatıya göre bu yetkiler daha sonra üçüncü bir kişi tarafından sistem dosyalarını silmek amacıyla kötüye kullanılmıştır.
- **UCLA laboratuvarında harici hat köprüleme ve fiziki yakalanma** — Dış aramalara kapalı üniversite bilgisayar laboratuvarındaki dahili hat, operatör yardımıyla harici ağa bağlanarak uzaktaki sistemlere sızmak amacıyla kullanılmıştır. Santral ve uç nokta düzeyindeki kısıtlamaların hat köprülemeye imkân tanıması yetkisiz erişimi mümkün kılmış, ancak laboratuvardaki şüpheli hareketlerin fark edilip bildirilmesi sonucu şahıs kampüs polisi tarafından fiziki olarak yakalanmıştır.

## Yazarın önerdiği karşı önlemler

- **Geri arama ile kimlik ve yetki teyidi (çıkarım)**: Telefonla gelen hassas bilgi veya sistem erişimi taleplerinde, arayan kişinin beyan ettiği kurumun veya birimin resmi kayıtlı dahili numarası üzerinden geri arama yapılmadan hiçbir işlem yürütülmemelidir.
- **Kritik yetki ve hesap tanımlamalarında ikili kontrol (çıkarım)**: Sistem yöneticisi düzeyinde ayrıcalıklı hesap oluşturma, parola sıfırlama veya uzaktan erişim yetkilendirmesi tek bir sözlü beyanla değil; kayıtlı biletleme ve bağımsız yönetici onayı süreçleriyle gerçekleştirilmelidir.
- **Korku ve aciliyet manipülasyonuna karşı standart prosedürler (çıkarım)**: "Veri kaybı", "acil güvenlik yaması" veya "kolluk soruşturması" gibi panik yaratan dış aramalarda personel yetki aşımı yapmamalı, önceden tanımlanmış eskalasyon ve teyit protokollerini tavizsiz işletmelidir.
- **Kasıtlı yanlış bilgi tuzağına karşı doğrulama disiplini (çıkarım)**: Saldırganın hedefi düzeltmeye sevk ederek doğru veriyi söyletme taktiğine karşı, çalışanlar kendilerine sunulan hatalı yetkilendirme kodlarını düzeltmek yerine karşı taraftan bağımsız ve tam doğrulama talep etmelidir.
- **Altyapı ve adres değişikliklerinde resmi veri doğrulaması (çıkarım)**: Hizmet sağlayıcılar, yeni hat tahsisi veya adres güncelleme taleplerinde yalnızca müşteri beyanına veya fiziki tabelalara güvenmemeli; mülkiyet ve resmi adres kayıtlarıyla çapraz kontrol yapmalıdır.
- **Fiziksel uç nokta ve santral kısıtlamalarının denetimi (çıkarım)**: Kurum ve okul laboratuvarlarındaki dahili santral hatları harici hat aktarımlarına karşı teknik olarak sıkılaştırılmalı, terminallerdeki şüpheli kullanım senaryoları fiziki ve mantıksal izlemeyle denetlenmelidir.
- **Ayrıcalıklı erişim bilgilerinin kontrolsüz paylaşılmaması (çıkarım)**: Sistemlere sağlanan yönetim yetkileri ve parolalar kişisel notlarda tutulmamalı veya üçüncü şahıslarla paylaşılmamalı; her kullanıcı için ayrı, geçici ve denetlenebilir oturum ilkeleri uygulanmalıdır.

## Okuma kapsamı

Metnin tamamı okunmuş olup metin bozukluğu veya anlamı belirsiz kılan herhangi bir eksiklik bulunmamaktadır.
