# Yöntemler

## Bağımsız kimlik ve yetki kontrolü
**Ne zaman:** Beklenmedik bilgi, erişim veya işlem talebinde.  
**Nasıl:** Talebi beklet; önceden güvenilir olduğu belirlenmiş rehber veya kanaldan kişiye ulaş; istenen işlem için yetkiyi ve iş gereğini ayrıca kontrol et. Doğrulama başarısızsa güvenli destek kanalına yönlendir ve gerektiğinde bildir.  
**Bedel:** İşlemi yavaşlatır; erişilebilir bir istisna süreci ve sorumlu gerekir. [Aldatma 2](chapters/aldatma-02.md), [13](chapters/aldatma-13.md)

## Bilgi parçalarının birleşimini değerlendir
**Ne zaman:** Zararsız görünen kurum içi ayrıntılar veya birden çok küçük talep söz konusuysa.  
**Nasıl:** Bilgiyi sınıflandır; kimlerin hangi amaçla alabileceğini belirle; parçaların sonraki talepleri inandırıcı hale getirip getirmediğini değerlendir; erişimi gerekçeye göre sınırla.  
**Bedel:** Aşırı sınırlama iş akışını aksatabilir; sınıfları iş sahipleriyle belirle. [Aldatma 2](chapters/aldatma-02.md)

## Yardım isteğini güvenli kanala taşı
**Ne zaman:** Acil bir sorun, destek çağrısı veya yardım talebi olağan kontrollerin atlanmasını gerektiriyorsa.  
**Nasıl:** Sorunu ve yardım iddiasını ayır; kayıtlı yardım masasını bağımsız ara; destek görevlisinin kimliğini ve işlemi doğrula; kullanıcı parolası istemeyen iş akışı kullan.  
**Bedel:** Gerçek sorunlar da bekleyebilir; hızlı ve tanımlı eskalasyon yolu sağla. [Aldatma 5](chapters/aldatma-05.md), [9](chapters/aldatma-09.md)

## Fiziksel ve dijital sınırları birlikte değerlendir
**Ne zaman:** Ziyaretçi, yüklenici veya çalışan bir alana ya da ağ bağlantısına erişiyorsa.  
**Nasıl:** Ziyaret kaydı ve kimliği doğrula; refakat ve alan yetkisini belirle; ağ erişimini ayrıca kontrol et; iş bitince erişimi geri al.  
**Bedel:** İşletim ve ziyaretçi deneyimi maliyeti vardır. [Aldatma 10](chapters/aldatma-10.md)

## Katmanlı savunma ve etki sınırlama
**Ne zaman:** Tek bir sistemin ele geçirilmesi değerli varlıklara ulaşmayı sağlayabiliyorsa.  
**Nasıl:** Varlık ve veri akışlarını belirle; kamuya açık, iç ve hassas sistemler arasında erişim sınırları koy; en az yetki, uç nokta güvenliği, güvenilir kayıt ve müdahaleyi birlikte değerlendir.  
**Bedel:** Yönetim ve izleme yükü artar; kontroller düzenli sınanmalıdır. [Sızma 2](chapters/ch06-szma-2-terristler-ibanda.md), [9](chapters/ch13-szma-9-uzak-eriim.md)

## Yetkili güvenlik testi
**Ne zaman:** Güvenlik kontrolünün etkinliğini sınarken.  
**Nasıl:** Yetki, kapsam, zaman, veri işleme, yasaklı işlemler, irtibat ve durdurma kurallarını yazılı belirle; bulguyu kanıt ve etkiyle raporla; düzeltmeyi yeniden doğrula.  
**Bedel:** Hazırlık ve koordinasyon gerektirir; kapsam dışındaki sistemlerin güvenli olduğu sonucunu vermez. [Sızma 6](chapters/ch10-szma-6-szma-testi.md)

## Eğitimi iş akışına bağla
**Ne zaman:** Çalışanlardan hassas talepleri değerlendirmeleri bekleniyorsa.  
**Nasıl:** Rolün gerçek taleplerinden örnek seç; doğrulama, güvenli ret ve bildirim pratiği yaptır; ortaya çıkan süreç eksikliğini düzelt. Çalışanların hatayı saklamadan bildirebilmesini sağla.  
**Bedel:** Eğitimin sürdürülmesi ve uygun destek kanalı gerekir. [Aldatma 15](chapters/aldatma-15.md)

<!-- sentez-2026-11-08 -->
## Varsayılan ve paylaşılan kimlik bilgilerini kaldır
**Ne zaman:** Yeni bir sistem, ağ cihazı, santral veya yazılım devreye alınırken ya da bakım sonrasında.  
**Nasıl:** Donanım ve yazılımlarla gelen üretici varsayılan parolalarını, fabrika PIN kodlarını ve standart hesapları derhal değiştir; bakım personeli veya servisler için ortak hesap kullanımını sonlandır; her cihaza ve yetkiliye tekil, güçlü kimlik bilgisi ata. (güncel yorum: merkezi kimlik yönetimi ve parola kasası çözümleri kullan).  
**Bedel:** Kurulum süresini uzatır; cihaz ve hesap envanterinin düzenli takibini gerektirir. [Aldatma 9](chapters/aldatma-09.md), [Sızma 4](chapters/ch08-szma-4-hrszlar-ve-polisler.md), [Sızma 7](chapters/ch11-szma-7-banka-gvenlii.md), [Sızma 9](chapters/ch13-szma-9-uzak-eriim.md), [Ghost 14](chapters/ghost-14.md), [Ghost 20](chapters/ghost-20.md)

## Kurumsal jargon ve makam iddiasını yetki sayma
**Ne zaman:** Tanınmayan bir kişi kurum içi terimler, sistem adları, yönetici isimleri veya hiyerarşik unvanlar kullanarak bilgi ya da işlem talep ettiğinde.  
**Nasıl:** Kurum içi jargona, dahili kısaltmalara veya üst düzey yönetici adına güvenerek yetki varsayma; talebi nezaketle beklemeye al; arayanın kimliğini ve talep gerekçesini bağımsız kurumsal kanallardan doğrulamadan veri paylaşma.  
**Bedel:** İletişimi yavaşlatır; personelin yöneticilerden çekinmeden sorgulama yapabilmesi için kurumsal güvence ve kültür gerekir. [Aldatma 3](chapters/aldatma-03.md), [Aldatma 4](chapters/aldatma-04.md), [Aldatma 6](chapters/aldatma-06.md), [Aldatma 8](chapters/aldatma-08.md), [Ghost 18](chapters/ghost-18.md), [Ghost 20](chapters/ghost-20.md)

## Geri aramada hat ve yönlendirme bütünlüğünü doğrula
**Ne zaman:** Dışarıdan veya şüpheli dahili hattan gelen işlem ve veri taleplerinde geri arama ile doğrulama yapılırken.  
**Nasıl:** Karşı tarafın sunduğu numarayı değil, resmi rehberdeki doğrulanmış numarayı geri ara; aranan dahili hatta aktif bir harici çağrı yönlendirmesi (call forwarding) bulunup bulunmadığını teknik olarak kontrol et; şüpheli sesli mesaj aktarmalarını veya doğrulanmamış santral hatlarını teyit sayma. (güncel yorum: bant dışı çok faktörlü doğrulama zorunlu tutulmalı).  
**Bedel:** Doğrulama sürecini uzatır; telekomünikasyon altyapısında çağrı yönlendirme kısıtlamaları ve teknik denetim yapılandırması gerektirir. [Aldatma 5](chapters/aldatma-05.md), [Ghost 2](chapters/ghost-02.md), [Ghost 12](chapters/ghost-12.md), [Ghost 14](chapters/ghost-14.md), [Ghost 18](chapters/ghost-18.md)

## Geçici yapılandırmaları ve atıl varlıkları tasfiye et
**Ne zaman:** Bakım, test, arıza giderme veya altyapı değişikliği çalışmaları tamamlandığında.  
**Nasıl:** Acil müdahale amacıyla açılan geçici konsol bağlantılarını, test hesaplarını, uzaktan erişim tünellerini ve web alanındaki kurulum betiklerini iş bitiminde sil; ortak alanlardaki kullanılmayan ağ prizlerini kapat; hizmet dışı kalan eski sunucuları ve test sistemlerini ağdan fiziksel olarak ayır.  
**Bedel:** Kapsamlı varlık envanteri, düzenli port taraması ve katı değişiklik yönetimi prosedürleri gerektirir. [Sızma 3](chapters/ch07-szma-3-teksas-hapishanesi.md), [Sızma 5](chapters/ch09-szma-5-bilgisayar-korsan-robin-hood.md), [Sızma 6](chapters/ch10-szma-6-szma-testi.md), [Sızma 8](chapters/ch12-szma-8-fikri-mlkiyet.md), [Sızma 9](chapters/ch13-szma-9-uzak-eriim.md)

## Dışa açık bilgi yüzeyini ve üstveriyi sınırla
**Ne zaman:** Kurum alan adları, DNS altyapısı, web servisleri veya e-posta sunucuları dış dünyaya açılırken.  
**Nasıl:** Whois ve alan adı kayıtlarında çalışan veya departman bilgisi yerine genel kurumsal iletişim verisi kullan; bölünmüş (split) DNS uygulayarak iç ağ yapısını ve sunucu adlandırmalarını dışarıya gizle; giden e-posta başlıklarındaki iç IP ve ana makine üstverilerini filtrele; web dizinlerinde konfigürasyon ve yedek dosyaları barındırma.  
**Bedel:** DNS yönetimini ve e-posta sunucu konfigürasyonunu karmaşıklaştırır; dış teknik desteğin teşhis süreçlerini kısıtlayabilir. [Sızma 5](chapters/ch09-szma-5-bilgisayar-korsan-robin-hood.md), [Sızma 7](chapters/ch11-szma-7-banka-gvenlii.md), [Sızma 8](chapters/ch12-szma-8-fikri-mlkiyet.md), [Ghost 18](chapters/ghost-18.md), [Ghost 22](chapters/ghost-22.md)

## Aciliyet ve kriz baskısında süreci esnetmeme
**Ne zaman:** Karşı taraf veri kaybı, sistem çökmesi, teslimat krizi veya yönetici öfkesi bahanesiyle acil kural dışı işlem talep ettiğinde.  
**Nasıl:** Korku, panik ve suçluluk duygusu uyandıran baskıları bilinçli bir aldatma işareti olarak değerlendir; aciliyet öne sürülerek parola paylaşımı, uzaktan erişim veya güvenlik kontrolü atlama taleplerini kesinlikle reddet; standart onay ve eskalasyon yollarını tavizsiz işlet.  
**Bedel:** Gerçek kriz durumlarında anlık esneklik kaybına yol açabilir; kuralı uygulayan çalışanın üst yönetici tarafından kurumsal olarak korunmasını gerektirir. [Aldatma 5](chapters/aldatma-05.md), [Aldatma 8](chapters/aldatma-08.md), [Aldatma 12](chapters/aldatma-12.md), [Ghost 3](chapters/ghost-03.md), [Ghost 21](chapters/ghost-21.md)

## Hassas atıkları ve basılı evrakı güvenli imha et
**Ne zaman:** Çalışma alanlarında, santrallerde veya arşivlerde basılı dokümanlar, kâğıt notlar, test çıktıları ya da manyetik ortamlar kullanım dışı kaldığında.  
**Nasıl:** Şirket içi rehber, parola notu veya operasyonel belge niteliğindeki tüm kâğıtları birleştirilemeyecek biçimde çapraz kesim öğütücülerden geçir; eski kaset, disket ve sabit diskleri fiziksel olarak imha et; atık kutularını ve konteynerleri kilitli tut; temizlik ve taşeron personelin atık alanlarına erişimini denetle.  
**Bedel:** Güvenli kâğıt imha ekipmanı, kilitli atık kutuları ve düzenli fiziksel atık denetim süreci gerektirir. [Aldatma 3](chapters/aldatma-03.md), [Aldatma 10](chapters/aldatma-10.md), [Aldatma 16](chapters/aldatma-16.md), [Sızma 4](chapters/ch08-szma-4-hrszlar-ve-polisler.md), [Sızma 6](chapters/ch10-szma-6-szma-testi.md)

## Çalışma alanında oturum ve konsol kilit disiplini
**Ne zaman:** Çalışanlar veya yöneticiler bilgisayarlarından, konsollarından ya da çalışma masalarından kısa süreliğine dahi ayrıldığında.  
**Nasıl:** Masadan ayrılırken işletim sistemi oturumunu veya parola korumalı ekran koruyucuyu derhal kilitle; belirli bir süre işlem yapılmadığında otomatik kilitlemeyi merkezi politika ile zorunlu tut; kritik sunucu konsollarını ve ağ izleme ekranlarını gözetimsiz açık bırakma; parolaları ekran veya masa çevresinde yazılı tutma.  
**Bedel:** Her oturum başına dönüldüğünde parola girilmesini gerektirir; kullanıcı konforunu ve iş akış hızını bir miktar düşürebilir. [Aldatma 11](chapters/aldatma-11.md), [Aldatma 12](chapters/aldatma-12.md), [Sızma 3](chapters/ch07-szma-3-teksas-hapishanesi.md), [Ghost 8](chapters/ghost-08.md), [Ghost 15](chapters/ghost-15.md)
