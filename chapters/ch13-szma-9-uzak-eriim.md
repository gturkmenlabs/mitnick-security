# Sızma 9: Uzak erişim

## Temel fikir
Güvenilen uzak istemcinin ele geçirilmesi, kurumsal ağ sınırını dolaylı olarak aşabilir.

## Uygulama
Uç noktaları koru; uzak erişimde güçlü kimlik doğrulama uygula; gereksiz servisleri filtrele; ağ güvenini ve erişimi sınırla.

## Kaçınılacak hata
Merkez ağını korurken dizüstü ve ev bilgisayarlarını kontrol dışında bırakmak.

## Çalışılmış örnek
Uzaktan bağlanan cihazın durumu ve hesabın yetkisi ayrı ayrı değerlendirilir.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Londra merkezli bir test vakasında geçici erişim çözümünün kalıcı hale gelmesi ve uzaktaki güvenilir istemcinin güvenliği ele alınır.

## Kontrol adımları
Geçici değişikliklere son kullanma tarihi ve sorumlu ata; uzak istemcileri koru; yalnız gizli veya alışılmadık bağlantı noktasına güvenme; ihlal edilen bir cihazdan sonraki erişimleri değerlendir.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 230–253; Türkçe çevirinin 9. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Hedefin seçilmesi ve keşif** — Kitaba göre Louis ile Brock, adı dışında hiçbir şey bilmedikleri, para ve tutuklu taşımacılığı yapan bir Avrupa şirketini hedef aldı. Şirketin dışa açık web sitesi, posta sunucusu ve IP kayıt kurumu kayıtları, kurumun yapısını haritalamaya yetti; dil engeli çeviri araçlarıyla aşıldı. İşlemeyen kontrol, kurumun dışarıdan görünen bilgi yüzeyinin sınırlandırılmamış olmasıydı.
- **Yüksek numaralı bağlantı noktasındaki cihaz** — Yoğun bir tarama sonunda alışılmadık bir yüksek numaralı bağlantı noktasında, beklenen üreticiye ait olmayan bir cihaz bulundu. Cihazın yönetici hesabı hâlâ varsayılan parolayla korunuyordu; varsayılan kimlik bilgileri hiç değiştirilmemişti.
- **Kalıcılaşan geçici çözüm** — Bir teknikerin acil ihtiyaç için kurduğu konsol bağlantısı sökülmemiş, cihaz güvenlik duvarının arkasından erişilebilir kalmıştı. Anlatıya göre kimse bu geçici düzenin farkına varmadı; yapılandırma denetimi ve değişiklik takibi yoktu.
- **Kendi tünelini açma girişimi** — Saldırganlar, meşru hizmeti kesintiye uğratmadan VPN cihazında kendilerine ayrı bir tünel tanımlayamadı. Cihazın yapısı buna izin vermedi; yapılandırma bütünlüğü burada beklenmedik biçimde işe yarayan tek kontrol oldu.
- **Kısa süreli bağlantıların yakalanması** — Saha görevlileri VPN'e yalnızca kısa aralıklarla bağlanıyordu. Bu pencerelerden birinde, bir dizüstünde kimlik doğrulaması zayıf bırakılmış uzaktan kontrol yazılımı görüldü; istemci uç noktası sertleştirilmemişti.
- **İstemciden alınan kimlik bilgileri** — Ele geçirilen dizüstündeki kayıtlı çevirmeli bağlantı bilgileri, VPN erişimini tek bir statik parolaya indirgiyordu. Saldırganlar meşru kullanıcı gibi oturum açtı; ikinci bir doğrulama katmanı yoktu.
- **İç ağdaki eski yazılım** — DMZ'den iç ağa geçildiğinde, yamaları uygulanmamış eski bir web sunucusu bulundu. Bilinen bir kodlama açığı üzerinden komut çalıştırma ve yetki yükseltme mümkün oldu; yama yönetimi ve iç ağın sertleştirilmesi eksikti.
- **Yerel ve alan yöneticisi parolasının aynı olması** — Kitaba göre bir yönetici, yerel yönetici hesabıyla alan yöneticisi hesabına aynı parolayı vermişti. Bu tekrar sayesinde saldırganlar uygulama sunucusunda tam denetim kazandı; parayı ve tutuklu sevkini yönlendirebilecek konuma geldiler, ancak anlatıya göre bunu kullanmayıp bulgularını şirkete rapor ettiler.

## Yazarın önerdiği karşı önlemler

- Geçici çözümlerin kalıcı hâle gelmesini engelle: ağ geçidi yapılandırmalarını düzenli aralıklarla, fiziksel ya da mantıksal olarak denetle; açık bağlantı noktalarının güvenlik politikasıyla uyumunu sürekli izle.
- "Gizlilikle güvenlik" yaklaşımını reddet: bir bağlantı noktasının alışılmadık ya da yüksek numaralı olması onu korumaz; güvenilmeyen ağlardan gelen erişim, hangi noktada olursa olsun engellenmelidir.
- Sistemler devreye alınmadan önce bütün varsayılan parolaları değiştir; bu, teknik bilgisi sınırlı kişilerin bile bildiği bir açıktır.
- İstemci uç noktalarını kapsam içine al: kurum ağına bağlanacak dizüstü ve ev bilgisayarlarının belirli bir güvenlik düzeyini karşılamasını zorunlu kıl, uyum sağlamayan istemcilerin erişimini reddet.
- Uzak erişimde güçlü kimlik doğrulama kullan: dinamik parolalar, akıllı kartlar, token ya da dijital sertifikalar; statik parolayla yetinme (güncel yorum: bugün bu öneri çok faktörlü kimlik doğrulama ve koşullu erişim olarak uygulanır).
- Gereksiz servisleri filtrele: gerek güvenilmeyen ağlardan gerekse DMZ gibi yarı güvenilir bölgelerden gelen giriş ve çıkış bağlantılarını belirli ana makinelere ve servislere göre sınırlayan kural kümeleri oluştur.
- Derinlemesine savunma kur ve yamaları güncel tut: yalnızca sınır güvenlik duvarına güvenmek, kilitle korunan bir odada açıkta bırakılan değerli eşyaya benzer; iç sistemleri de sertleştir ve modeli düzenli olarak sına.
- Saldırı tespiti ve denetim kayıtlarını etkinleştir; kimlik doğrulama bilgilerini başka hizmet sunmayan, hesap sayısı en az olan ayrı bir ana makinede sakla.

## Okuma kapsamı

Bölümün tamamı (9.1–9.4) okundu; ancak şirketin ve cihazların kimliği anlatıda gizlendiği ve metin Çince çeviri üzerinden aktarıldığı için bazı teknik ayrıntılar ile yer yer bozulan harf aralıkları belirsiz kaldı.
