# Aldatma Sanatı — 10: İçeriye girmek

**Kaynak:** Türkçe PDF, dosya sayfaları 248–292. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Fiziksel erişim, ağ bağlantısı ve içeriden görünme birbirini destekleyen risklerdir.

## Ne zaman ve nasıl kullanılır?
Ziyaretçileri doğrula ve refakat et; kapı ve ağ erişimini ayrı kontrol et; ziyaretçi ağını kurumsal kaynaklardan ayır.

## Çalışılmış örnek
Toplantı odasındaki ziyaretçinin kimliği teyit edilir; cihazı kurumsal ağa otomatik erişmez. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Rozet görüntüsünü veya başkasının kapıyı açmasını erişim yetkisi saymak.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar
- **Havacılık fabrikasına gece sızması** — Bir genç, telefonla edindiği şirket içi unvan ve dahili numaraları kullanarak güvenlik kulübesine mesai dışı ziyaret notu bıraktırmış ve sahte plakalı araçla tesise girmiştir. Üretim alanında yakalandıklarında, yöneticisiyle telefonda görüşüyormuş gibi davranarak ve görevlinin üst yöneticiyi gece rahatsız etme çekincesinden yararlanarak tesisten serbestçe ayrılmışlardır. Resimli kimlik doğrulaması yapılmaması ve tesisten çıkana kadar şahıslara refakat edilmemesi kontrolün başarısız olmasına yol açmıştır.
- **Çöp dalışı ve fiziksel atık istismarı** — Anlatıya göre yazar telefon şirketlerinin çöplerinden dahili rehberler ve yırtılmış kağıtları birleştirerek sistem şifreleri elde etmiş; basına yansıyan bir başka olayda da bir araştırma şirketi rakip firmanın çöplerini ele geçirmek için temizlik görevlilerine rüşvet teklif etmiştir. Belgelerin ve depolama ortamlarının imha edilmeden doğrudan çöpe atılması ile temizlik personeli üzerindeki denetim eksikliği bilgi sızıntısına zemin hazırlamıştır.
- **Görev yeri değiştirilen çalışanın intikamı** — Başka bir birime aktarılan öfkeli bir çalışan, kurum dışından genç bir korsanın yardımıyla ofisteki bir bilgisayara gizlice modem ve uzaktan erişim yazılımı bağlatmış, yöneticisinin bilinen parolasını kullanarak bütçe sunumuna uygunsuz fotoğraflar yerleştirmiştir. Kurumdan ayrılma aşamasındaki personelin mesai saatlerinde denetimsiz dolaşabilmesi, izinsiz donanım bağlantılarının engellenmemesi ve parola paylaşımı alışkanlığı kontrollerin çökmesine neden olmuştur.
- **Oto yedek parça toptancısına ağ üzerinden sızma** — Bir saldırgan, danışma görevlisinin kariyer arzusunu istismar edip güven sağlayarak ve şirket içi gerçek isimleri kullanarak toplantı bekleme bahanesiyle konferans salonuna geçmiştir. Odadaki Ethernet hattından şirket ağına bağlanmış, hedef muhasebe yazılımındaki varsayılan zayıf parolaları aşarak fiyatlandırma kayıtlarını kendi lehine değiştirmiştir. Ziyaretçi kimliğinin teyit edilmemesi, ziyaretçiye eşlik edilmemesi ve toplantı odalarındaki ağ portlarının sınırlandırılmaması güvenlik zaafı yaratmıştır.
- **Bilgi işlem personelinin bordro merakı** — Anlatıya göre yazarın çalıştığı şirketteki bilgi işlem personeli, sahip oldukları geniş sistem yetkilerini kötüye kullanarak mesai arkadaşlarının ve yöneticilerin gizli maaş ile bordro bilgilerini incelemiştir. Ayrıcalıklı sistem erişimine sahip kullanıcıların faaliyetlerinin denetlenmemesi ve hassas dosyalara erişim günlüklerinin takip edilmemesi bu yetki aşımına imkan tanımıştır.

## Yazarın önerdiği karşı önlemler
- **Ziyaretçi ve mesai dışı giriş kontrolü:** Kartı olmayan çalışanlar ve tüm harici ziyaretçiler lobide resimli kimlik kontrolünden geçirilmeli, ziyaretçilere bina içinde daima refakat edilmeli ve mesai dışı ziyaretler ilgili yöneticiden doğrudan teyit edilmelidir.
- **Kapsamlı atık yönetimi ve imha:** Hassas veriler sınıflandırılmalı, kağıtlar birleştirilemeyecek biçimde çapraz kesim öğütücülerden geçirilmeli; disk ve manyetik bant gibi veri taşıyıcıları kalıcı olarak imha edilmeli ve çöp konteynerleri kilitli tutulmalıdır.
- **İşten ayrılma süreçlerinin yönetimi:** Ayrılan personelin erişim yetkileri bina henüz terk edilmeden derhal kapatılmalı, giriş kartları ile anahtarları teslim alınmalı ve gerektiğinde ilgili çalışma grubunun sistem parolaları yenilenmelidir.
- **Ortak alanlarda ağ izolasyonu:** Konferans ve eğitim salonlarındaki ağ bağlantı noktaları kilitlenmeli, güvenlik duvarı veya yönlendiricilerle iç ağdan yalıtılmalı ya da ağa bağlanan her cihaz için kimlik doğrulama zorunlu kılınmalıdır (güncel yorum: 802.1X / NAC).
- **Hassas verilere erişim ve denetim kayıtları:** Bordro ve insan kaynakları gibi kritik dosyalara erişim yetkileri sınırlandırılmalı, başarılı veya başarısız tüm erişim girişimleri denetim günlüklerine (audit log) kaydedilerek düzenli izlenmelidir.
- **Sosyal mühendislik farkındalığı:** Güvenlik ve danışma görevlileri, kişilerin profesyonel görünümüne, giyimine veya unvan iddialarına aldanmamaları, üst kademelerden çekinmeden kuralları eksiksiz uygulamaları konusunda eğitilmelidir.

## Okuma kapsamı
Bölüm metninin tamamı Türkçe çevirideki sözcük ve harf arası boşluk bozulmalarına rağmen eksiksiz olarak okunmuş olup, içeriğin anlaşılmasını engelleyen bir belirsizlik bulunmamaktadır.
