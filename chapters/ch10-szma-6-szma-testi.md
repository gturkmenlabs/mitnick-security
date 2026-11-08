# Sızma 6: Sızma testi

## Temel fikir
Yetkili testlerin değeri yalnızca erişim elde etmekte değil, iş etkisini ve kontrol eksiklerini anlamaktadır.

## Uygulama
Yazılı yetki, kapsam, süre, yasaklı işlemler, bildirim ve durdurma koşullarını önceden belirle; sonuçları kanıt ve düzeltme önerileriyle raporla.

## Kaçınılacak hata
Belirsiz kapsamla test yapmak veya gösterişli başarıyı risk azaltımıyla karıştırmak.

## Çalışılmış örnek
Test öncesi bir irtibat kişisi ve olay halinde durdurma yolu belirlenir.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Güvenlik danışmanlarının test öyküleri test koşullarının, iletişimin ve değerlendirilen gerçek riskin önemini gösterir.

## Kontrol adımları
Test öncesinde hedefleri ve yetkili varlıkları yazılı belirle; fiziksel giriş, veri toplama ve operasyonel etki sınırlarını kararlaştır; acil durdurma irtibatı ata; bulguları düzeltmeye bağla.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 151–174; Türkçe çevirinin 6. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Newton’da satın alma testi** — Anlatıya göre bir IT danışmanlık şirketi, l0pht’yi satın almadan önce ücretli sızma testi yaptırdı; Mudge, şirketin belgelerini ve iletişimini kapsayan geniş yetki aldı. Satın alma görüşmesi ile test ayrılmadığı ve heyet ekibi tanımadığı için çalışma müzakere istihbaratına dönüştü.
- **Newton’da teknik sızma** — Anlatıya göre ekip, güvenlik duvarındaki kaynak kapısına dayalı varsayılan kuralı aşarak iç hizmetlere ulaştı; düşük yetkili hesabın yazabildiği web yapılandırması, yeniden başlatmada daha yüksek yetki sağladı. Dışa giden bağlantıların izlenmemesi ve yanlış dosya sahiplikleri kalıcı erişimin fark edilmesini geciktirdi.
- **Çöp ve tailgating** — Anlatıya göre ekip, çöpe atılmış bir masada uçak biletleri, el kitapları ve iç belgeler buldu; ayrıca çalışanların arkasından güvenli kapılardan geçti. Atık imhası, fiziksel denetim ve yabancıyı kibarca durdurma alışkanlığı yeterli olmadığı için bu yol açık kaldı.
- **Sesli mesaj kutuları** — Anlatıya göre telefon hattı taraması, varsayılan veya zayıf PIN’li sesli mesaj kutularını buldu; yöneticilerin satın alma konuşmaları dinlendi. PBX ve sesli mesaj politikası parola gücünü, varsayılanları ve erişim denetimini kapsamadığı için hassas konuşmalar korunamadı.
- **Biotech’te ortak alan prizi** — Anlatıya göre Dustin Dykes, toplantı odasının bulunduğu ortak alandaki canlı ağ prizinden iç ağa bağlandı ve fark edilmemek için kablosuz bir erişim cihazı bıraktı. Ortak alanın iç ağdan yalıtılmaması, kullanılmayan prizlerin kapatılmaması ve izinsiz cihaz denetiminin olmaması erişimi kolaylaştırdı.
- **Biotech’te zayıf parolalar** — Anlatıya göre aynı ağdaki kırk kadar Windows makinesinde yönetici parolasının boş veya tahmin edilebilir olması, tek makineden etki alanına yayılmayı sağladı; kırılan parola özetleriyle etki alanı yöneticiliğine ulaşıldı. Düz ağ, yerel ve etki alanı hesaplarının ortak parolası ve zayıf politika nedeniyle ilaç güvenliği dosyaları ile çalışan verileri açığa çıktı.
- **Biotech’te sahte rozet ve alarm** — Anlatıya göre ekip, şirket logosundan hazırladığı sahte rozetle güvenlik görevlisini geçti; okuyucunun kabul etmediği rozete rağmen görevli kapıyı açtı, alarm da yanlış alarm bahanesiyle savuşturuldu. Bir yöneticinin masasına bırakılan kayıt cihazı iki hafta bulunmayınca, fiziksel giriş ve cihaz denetiminin birlikte zayıf olduğu görüldü.
- **Biotech’te sensör ve sorgulama eksikliği** — Anlatıya göre ekip, çıkış kapılarındaki ısı/momentum sensörlerini dışarıdan yanıltarak kilit açtırdı; büyük ekipmanla ve rozetsiz dolaşan üyelere rağmen kimse durdurmadı. Fiziksel güvenliğin yalnızca cihaza değil, çalışanların sorgulama alışkanlığına ve düzenli denetime de bağlı olduğu görüldü.

## Yazarın önerdiği karşı önlemler

- Güvenlik duvarı kurallarını düzenli gözden geçirin; kaynak kapısına güvenmeyin, yalnızca gerekli hizmetlere izin verin.
- Dosya ve dizin izinlerini en az yetkiyle sınırlayın; sunucu süreçlerinin yazabildiği yapılandırma alanlarını daraltın.
- Yönetim trafiğinde açık metin yerine SSH gibi şifreli protokoller kullanın.
- Sesli mesaj ve PBX’te varsayılan PIN’leri, dahili veya ATM numarasını yasaklayan güçlü parola politikası uygulayın.
- Ortak alanlardaki kullanılmayan ağ prizlerini kapatın veya yalıtın; gerekiyorsa erişim öncesi kimlik doğrulama isteyin.
- Tailgating’e karşı çalışanlara yabancıyı kibarca durdurmayı, rozet sormayı ve gerekirse güvenliğe eşlik etmeyi öğretin.
- Elektronik okuyucuyu tek başına yeterli görmeyin; görevlileri başarısız rozet ve alarm durumlarında olayı sorgulamaları için eğitin.
- Yöneticileri şüpheli iç davranışları fark etme konusunda eğitin; kitap, güvenlik politikası olan kurumların bile bu eğitimi ihmal edebildiğini belirtir.

## Okuma kapsamı

Kaynağın eldeki tamamı okundu; ancak metin çıkarımındaki harf aralığı ve karakter bozulmaları nedeniyle bazı ürün adları, unvanlar ve cümle bağlantıları belirsiz kaldı.
