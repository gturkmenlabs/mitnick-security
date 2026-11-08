# Sızma 4: Hırsızlar ve polisler

## Temel fikir
Yanlış yapılandırmalar, varsayılan ayarlar ve zayıf kimlik doğrulama birbirini güçlendirebilir.

## Uygulama
Sistemleri hizmete almadan güvenlik açısından değerlendir; yapılandırmaları yönet; güçlü kimlik doğrulama ve eğitim uygula.

## Kaçınılacak hata
Kurulumun ilk günündeki doğru ayarların zaman içinde korunacağını varsaymak.

## Çalışılmış örnek
Yeni telefon ve bilgisayar altyapısı kullanım öncesi yapılandırma kontrolünden geçer.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Telefon ve bilgisayar sistemlerine ilişkin vakalarda yapılandırma, varsayılanlar ve kimlik doğrulama birlikte değerlendirilir.

## Kontrol adımları
Kurulumdan önce güvenli yapılandırmayı tanımla; varsayılan kimlik bilgilerini değiştir; ayrıcalıklı erişime güçlü doğrulama uygula ve sonraki değişiklikleri takip et.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 98–124; Türkçe çevirinin 4. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Telefon şebekesine sızma** — Matt ve Costa, telefon şirketinin baz istasyonu çevresindeki atıklardan test numaraları ve cihazlara ait elektronik seri numaraları toplayıp kendi mobil telefonlarının çiplerini yeniden programlayarak bedava görüşme elde etti. Anlatıya göre operatörün test donanımını ve varsayılan ayarlarını denetlememesi bu açığı mümkün kıldı.

- **Mahkeme bilgisayarı** — Otomatik numara taramasıyla buldukları ABD Bölge Mahkemesi sistemine, kullanıcı adı ile parolası aynı olan herkese açık bir varsayılan hesapla girdiler. Kitaba göre sistemin erişim kapısı gerçek bir kimlik doğrulama sunmuyordu; parola dosyasına ve yargıç hesaplarına ulaştılar.

- **Otel zinciri** — Matt, kendini rezervasyon yazılımı firmasının teknisyeni olarak tanıtıp resepsiyonu oyalayarak yazılımın değiştirilmemiş varsayılan yönetici hesabıyla otele girdi. Aynı yazılımı kullanan başka bir otelde de aynı varsayılanlar geçerliydi; sahte adla süit kiralayıp depozitoyu geri istediler.

- **Subsequent üzerinden Boeing** — Mahkeme sistemine yerleştirilen bir truva atı, yazılım satıcısı Subsequent'in makinelerine sızdı; oradan müşteri listesi ve Boeing'e ait hesaplar ele geçirildi. Matt'in anlatımına göre kapatılmayan bir modem oturumu ona başka bir kullanıcının kabuğunu verdi.

- **Boeing'de tespit** — Güvenlik yöneticisi Don Boelling'in ekibi, arka planda çalışan bir parola kırma programını ve kırılmış 26 parolayı fark etti; isimler mahkeme yargıçlarına aitti. Ağ geçidi ve telefon hattı takibiyle saldırganların izi sürüldü; anlatıya göre yönetim sistemleri hemen kapatmak istedi, Boelling kanıt toplamak için izlemeyi sürdürdü.

- **Gözetim ve dinleme** — Federal yetkililer telefon dinleme izni aldı, kampüse yerleştirilen ajanlar Matt'in hareketlerini kaydetti. Costa çevredeki araçları fark etti; ikili önceden kararlaştırdıkları bir kod işaretiyle birbirini uyardı, ancak yine de adım adım izlendiklerini tam olarak anlamadılar.

- **EPA ve tutuklama** — Çevre Koruma Ajansı'nda 600 kadar bilgisayarın aynı root hesabını ve parolasını paylaştığı görüldü. Tutuklamaların ardından ikili, 250 saat kamu hizmeti, beş yıl bilgisayar yasağı ve çoğu Boeing'e olmak üzere 30.000 dolar tazminatla cezalandırıldı.

- **Cezaevi telefon sistemi** — Tutuklu iken adli yardım hattının sesli mesaj sistemini yeniden programlayarak dışarı arama yaptılar ve savunmalarını birlikte kurdular. Bu, denetlenmeyen telefon yapılandırmasının kurum içinde bile kötüye kullanılabildiğini gösterdi.

## Yazarın önerdiği karşı önlemler

- Yapılandırma yönetimini açık kurallara bağla; kurulumu yapan BT ve telefon personelini eğit ve düzenli olarak değerlendir.
- Yeni sistem ve cihazları üretime almadan önce güvenlik testinden geçir; çalışanlara farkındalık eğitimi ver (yazar burada *Aldatma Sanatı* kitabına atıf yapıyor).
- Yalnızca sabit parolaya güvenme; zaman tabanlı token, güvenilir biyometri veya fiziksel şifreleme aygıtı gibi ek doğrulama katmanları kullan.
- Parolaları düzenli değiştir; en az bir rakam, bir simge ya da büyük-küçük harf karışımı isteyen güçlü parola kuralı uygula.
- Kullanıcıların parolayı not alıp monitöre, klavyenin altına veya çekmeceye bırakmasını engelle; farklı makinelerde aynı ya da benzer parolayı kullanma.
- Yazılım üreticileri güvenli ayarları varsayılan yapmalı ve kullanıcıyı varsayılanları değiştirmesi için uyarmalı; yazar örnek olarak Windows XP SP2'de güvenlik duvarının varsayılan açık gelmesini gösteriyor.
- Varsayılan hesapları ve parolaları hemen değiştir; ilk günkü doğru ayarların kendiliğinden korunacağını varsayma. (güncel yorum: bugün çok faktörlü kimlik doğrulama ve otomatik yapılandırma denetimi olağan kabul ediliyor.)

## Okuma kapsamı

Kaynak 4.17 özetine kadar baştan sona okundu; ancak Türkçe OCR çıkarımındaki harf boşlukları ve bozulmuş adlar (örneğin "Don" yer yer "Dot/Dom") nedeniyle birkaç ayrıntı belirsiz kaldı.
