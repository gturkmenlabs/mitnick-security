# Sızma 7: Banka güvenliği

## Temel fikir
Finansal sistemlerde güven ve yetki zinciri, erişim sağlayan insan ve süreçleri de kapsar.

## Uygulama
İşlemleri ve ayrıcalıklı erişimi bağımsız doğrulama, ayrık görevler ve izleme ile koru; kimlik bilgisinin yeterli olup olmadığını sorgula.

## Kaçınılacak hata
Kurumsal veya finansal bir sistemin doğal olarak güvenli olduğunu varsaymak.

## Çalışılmış örnek
Hassas işlem için çağrıyı başlatanın iddiası dışında onay ve kayıt aranır.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Banka örnekleri, finansal sistemin kurumsal itibarıyla gerçek erişim ve işlem kontrollerinin aynı şey olmadığını gösterir.

## Kontrol adımları
Yetkili kullanıcı, talep edilen işlem ve işlem limiti için ayrı kontroller uygula; işlem kayıtlarını ve istisnaları gözden geçir; hassas işlemlerde bağımsız onay değerlendir.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 175–190; Türkçe çevirinin 7. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Peropgie bankası ve Juhan** — Kitaba göre 23 yaşındaki Estonyalı Juhan, bankanın etkileşimli soru-cevap sayfasının kaynak kodunu incelerken sunucudaki parola dosyasını işaret eden gizli bir form alanı fark etti; sunucu, gönderilen girdinin nereden geldiğini doğrulamadığı için bu değişiklik kabul edildi ve şifrelenmiş parola dosyası tarayıcıda göründü. Juhan dosyayı indirip sözlük sözcüklerine dayanan bir parola tahmin yöntemiyle kısa sürede zayıf parolaları çözdü ve yönetici yetkisi kazandı. Kontrollerin işlememesinin nedeni, istemci tarafındaki gizli alanlara güvenilmesi ve parola politikasının sözlük kelimelerine izin vermesiydi.

- **Juhan'ın ifşası ve şirketin tutumu** — Anlatıya göre Juhan sisteme daha fazla girmeden durdu, durumu işverenine bildirdi ve bankanın haberdar edilmesini sağladı; cezalandırılmak yerine açığın kapatılması için görevlendirildi. Kitapta Juhan, şirketlerin kendilerine açık bildiren kişileri dava etmek yerine onlarla çalışmasının daha akıllıca olduğunu savunuyor; yazar bu görüşü Adrian Lamo davasıyla ilişkilendirerek tartışıyor.

- **Gabriel'in keşif aşaması** — Kitaba göre Kanada'da yaşayan genç Gabriel, hangi ağ adresi bloklarının hangi kuruluşlara verildiğini gösteren açık listelerde "banka" ve "hükümet" gibi sözcükleri aradı ve bir bankanın adres aralığını buldu. Ardından bankanın uzaktan erişim hizmeti sunduğunu ve bu hizmetin zayıf yapılandırıldığını tespit etti. Bu aşamada kontrolsüzlük, kurumun dışarıdan görülebilen hizmet envanterinin ve erişim noktalarının yeterince daraltılmamış olmasıydı.

- **Varsayılan parolalar ve düz ağ** — Gabriel, değiştirilmemiş varsayılan yönetici parolasına sahip bir yönlendiriciye ulaştı ve güvenlik duvarına uzaktan bağlantıya izin veren bir kural ekledi; kimlik doğrulamasının ardından bankanın iç ağından bir adres aldı. Ağ tek bir düz segmentten oluştuğu için tek bir sistemin ele geçirilmesi diğer tüm sistemlere köprü oldu. Üstelik sunucuda, dışarıdan gelen güvenlik danışmanlarının hazırladığı ve bilinen açıkları listeleyen rapor duruyordu; kurum denetim yaptırmayı yeterli koruma sanmıştı.

- **AS/400 ve uygulama el kitapları** — Anlatıya göre Gabriel, aşina olmadığı ana sisteme varsayılan yönetici parolasıyla girdi; etki alanı sunucusunda bankanın uygulama kullanım kılavuzlarını bulup indirdi. Bu belgeler, hangi ekranların hangi işlevi gördüğünü adım adım anlatarak yetki kazanmış bir kullanıcının bilmesi gerekenleri doğrudan sağladı. Kontrol zafiyeti, varsayılan hesap parolalarının korunması ve hassas işletim belgelerinin erişilebilir paylaşımda tutulmasıydı.

- **Tuş kaydedici ve etki alanı yöneticisi avı** — Gabriel, uzaktan erişim sunucusuna gizli bir tuş kaydedici yerleştirdi ve yönetici oturumlarını bekleyerek kimlik bilgilerini topladı. Ardından yönetici oturumunda sessizce çalışacak bir betiği başlangıç klasörüne yerleştirdi ve etki alanı yöneticisi oturum açtığında parola özetlerini topladı; kısa ve basit parolalar hızla çözüldü. Kitaba göre bankada sürekli çalışan kötü amaçlı yazılım denetimi yoktu ve parolalar tahmin edilebilir düzeydeydi.

- **Havale yetkisi ve sonuç** — Kitaba göre Gabriel, eğitim belgeleri sayesinde para transferi işlevlerine, müşteri hesabı görüntüleme ve ATM kayıtlarına erişebilecek duruma geldi; banka çalışanlarının yetkilerine denk bir konuma ulaştı. Anlatıya göre parayı almadı ve sisteme zarar vermedi; fiziksel güvenlik belgelerinin ayrıntılı, bilişim güvenliği belgelerinin ise yok denecek kadar zayıf olduğunu gözlemledi.

## Yazarın önerdiği karşı önlemler

- Web uygulamalarında güvenli kodlama kuralları uygulanmalı; kullanıcı girdisinin sunucu tarafına taşıdığı etki sınırlandırılmalı, sabit dosya adları ve sabitler tercih edilmeli.
- Hizmet hesaplarının (kitapta örnek olarak anılan sistem hizmeti hesabı) kişilere atanmaması, son kullanım zamanlarının denetlenmesi; yetkisiz yönetici ve grup yetkilerinin, son oturum açma kayıtlarının düzenli incelenmesi; olağandışı saatlerde belirlenen parolaların izinin sürülmesi.
- Etkileşimli oturum açma yalnızca iş saatleriyle sınırlandırılmalı.
- Kablosuz, çevirmeli, Internet ve kurum dışı ağlardan gelen tüm oturum açma/kapama olayları kayıt altına alınıp denetlenmeli.
- Yetkisiz tuş kaydedicileri saptamaya yönelik yazılımlar kullanılmalı (kitapta adı geçen tespit aracı örnek gösteriliyor).
- Güvenlik güncellemelerinin kurulumunda dikkatli olunmalı; kitap, bazı ortamlarda otomatik güncellemenin uygun olabileceğini belirtiyor.
- Uzaktan denetim yazılımlarıyla erişilen sistemler ile Terminal Services/Citrix türü oturumlar ayrıntılı biçimde denetlenmeli; saldırganlar bu hizmetleri daha az fark edilmek için tercih edebiliyor.
- Derinlemesine savunma uygulanmalı: dış denetim tek başına yeterli değildir, ağın ve ağ içindeki tüm sistemlerin yönetilmesi gerekir.

## Okuma kapsamı

Bölümün tamamı (7–7.5 ve notlar) okundu; Türkçe çıkarımdaki harf aralığı bozulmaları ve kısalmış cümle başları (kişi adlarının "Juhan/Juhaii/Jiihan", banka adının "Peropgie" biçiminde tutarsız yazılması gibi) nedeniyle birkaç özel ad ve cümle geçişi belirsiz kaldı, ancak olay örgüsü ve karşı önlem listesi bütün olarak izlenebildi.
