# Ghost in the Wires — 08: Lex Luthor

## Bölüm odağı
DEC kaynak kodu, soruşturma ve yazarın iddialara itirazları. Bu bölüm birinci kişinin anı anlatısıdır; olaylar ve görüşler yazara atfedilmelidir.

## Uygulama ilkesi
Kaynak koduna erişimi ve aktarımı sınırla; yazarın suçlama değerlendirmesini onun görüşü olarak belirt.

## Kaynaktan örnek
Yazar DEC kaynak koduna yönelik erişimi ve soruşturmada ileri sürülen bazı iddialara itirazını anlatır.

## Karar ve uygulama
Kod erişimlerini en az yetkiyle sınırla; hukuki iddiaları tek anlatıdan kesinleştirme. Kimlik doğrulama ile işlem yetkisini ayrı ele al; doğrulanamayan talepleri bilinen destek kanalına yönlendir.

## Sınır
Bu kısa not bölümün ayrıntılı okumasının yerine geçmez. Tarihsel uygulamaları güncel standartlara karşı değerlendir. Kaynak: İngilizce PDF, dosya sayfaları 64–78.

## Bölümün ayrıntılı okuması

- DEC geliştirme ortamına ilişkin anlatıda, teknik bir operatörün anlayıp onaylamadığı bir işlemle yetkili oturumun başka bir bağlantıya aktarılabildiği ileri sürülür. İnsanların sadece parola vermekle değil, yetkili oturumlarında bilinmeyen işlemler yapmakla da erişim aktarabileceğini değerlendir.
- Yazar, olağandışı ağ trafiğinin ve disk kullanımının yöneticilerin dikkatini çektiğini; parolaların değiştirilmesinin, saldırganın kontrol ettiği uç noktalar temizlenmediği için sorunu tek başına çözmediğini anlatır. Olay müdahalesinde erişimi kesmek, uç noktaları temizlemek, sırları yenilemek ve tekrar erişimi izlemek birlikte planlanmalıdır.
- Bölüm, gözaltı ve tecrit koşulları, anlaşma süreci ve evliliğin bitişini de yazarın bakış açısından aktarır. Parasal zarar hesaplarına ve iddialara itirazı, bağımsız bir mahkeme bulgusu gibi sunulmamalıdır.

## Vaka üzerinden karar

Bir hesap parolası değiştirildikten kısa süre sonra yeniden kötüye kullanılıyorsa yalnız parolayı tekrar değiştirmek yeterli olmayabilir. Hesapla kullanılan uç noktalar, etkin oturumlar, ayrıcalıklı hesaplar ve güvenilir kayıtlar birlikte incelenir; bulgulara göre kontrollü iyileştirme yapılır.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **DEC VMS sistemine operatör üzerinden yetkisiz oturum aktarımı** — Anlatıya göre yazar, kurum içi geliştirici kimliğine bürünerek operasyon merkezini aramış ve operatörden harici bir terminale ayrıcalıklı süreç bağlayan bir komut çalıştırmasını istemiştir. Operatörün komutun yetki devri riskini bilmemesi ve şirket içi kimlik doğrulama kontrollerinin işletilmemesi nedeniyle sistem güvenliği aşılmıştır.
- **Kaynak kod sızdırma ve tespit sonrası kalıcılık** — Saldırganlar DEC ağından elde ettikleri kaynak kodları harici üniversite sunucularına aktarmış; sistem yöneticileri gece trafiği ile disk doluluğu anomalilerini fark edip parolaları sıfırlasa da izinsiz erişim sürmüştür. Müdahale sürecinde yalnızca parolaların değiştirilmesi, fakat saldırganların kontrolündeki uç noktalardaki tuş kaydedicilerin ve arka kapı yamalarının temizlenmemesi savunmayı etkisiz kılmıştır.
- **Fiziksel kapı şifresinin ele geçirilmesi ve açık konsol erişimi** — Anlatıya göre yazar, bilgisayar odasının dijital kapı kodunu cüzdanda unutulmuş bir kâğıttan temin etmiş ve komşu şirketteki ağ izleme konsoluna doğrudan erişmiştir. Fiziksel kilit kodlarının kâğıda yazılıp açıkta bırakılması ve kritik ağ izleme terminallerinde (Snoopy) oturumların kilitlenmeden gözetimsiz tutulması yerel erişim engellerini işlevsiz kılmıştır.
- **Cezaevi telefon kısıtlamasının cihaz manipülasyonuyla aşılması** — Yazar, tecritteyken yalnızca onaylı numaraları arama kuralını, hat kapatma mandalını basılı tutup tuşlama seslerini gizleyerek harici numaraları manuel aramak suretiyle atlatmıştır. Görevlinin fiziksel takibi bulunmasına karşın tuş takımının donanımsal veya sistemsel olarak kısıtlanmamış olması denetimi yetersiz bırakmıştır.
- **Telesekreter erişim sinyallerinin sosyal mühendislikle temini** — Yazar, telesekreter kayıtlarını uzaktan dinlemek amacıyla mağaza görevlisine kumandasını kaybeden bir müşteri hikâyesi anlatmış ve personelden farklı uzaktan kontrol tonlarını telefona dinletmesini sağlamıştır. Satış personelinin sahiplik doğrulaması yapmadan cihaz kontrol frekanslarını dışarı aktarması, uzaktan erişim güvenliğini hükümsüz kılmıştır.

## Yazarın önerdiği karşı önlemler

- **Ayrıcalıklı komut taleplerinde kimlik ve yetki doğrulama (çıkarım)**: Operatörler, telefon veya mesajla gelen kurum içi taleplerde arayanın kimliğini resmî kanallardan teyit etmeden oturum devri veya süreç başlatma gibi yetkili komutları kesinlikle yürütmemelidir.
- **Olay müdahalesinde uç nokta temizliği ve bütüncül denetim (çıkarım)**: Sistem ihlallerinde yalnızca hesap parolalarını değiştirmek kalıcılığı engellemez; klavye dinleyicisi barındıran uç noktalar temizlenmeli, oturum açma programları (Loginout vb.) doğrulanmalı ve uyuyan ayrıcalıklı hesaplar taranmalıdır.
- **Ağ ve depolama anomalilerinin izlenmesi (çıkarım)**: Gece saatlerinde görülen beklenmedik bant genişliği kullanımı, ani disk dolulukları ve harici ağlara yönelik toplu veri aktarımları alarm mekanizmalarıyla izlenmeli ve şüpheli oturumlar otomatik olarak sınırlandırılmalıdır.
- **Fiziksel kimlik bilgisi ve oturum güvenliği (çıkarım)**: Kapı şifreleri veya sistem parolaları kâğıtlara not edilmemeli; kritik müşteri veya ağ trafiğini izleme yetkisine sahip konsollar açık oturumla gözetimsiz bırakılmamalı, otomatik ekran kilidi işletilmelidir.
- **Destek ve satış kanallarında donanım güvenliği (çıkarım)**: Donanımlara veya servislere ait kontrol frekansları, sıfırlama kodları ya da bypass yöntemleri, sahipliği doğrulanmamış üçüncü taraflarla hiçbir kanal üzerinden paylaşılmamalıdır.

## Okuma kapsamı

Bölüm metninin (İngilizce kaynak) tamamı eksiksiz okunmuş olup, içeriğin anlaşılmasını engelleyen herhangi bir metin bozukluğu veya belirsizlik bulunmamaktadır.
