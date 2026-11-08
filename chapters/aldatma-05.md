# Aldatma Sanatı — 05: Size yardımcı olabilirim

**Kaynak:** Türkçe PDF, dosya sayfaları 87–126. Metin çıkarımında sözcük ayrımı bozulmaları vardır.

## Temel fikir
Beklenmedik yardım ve sorun çözme iddiası karşılıklılık duygusu yaratabilir ve güvenlik kararını etkileyebilir.

## Ne zaman ve nasıl kullanılır?
Destek talebinin gerçekten açılıp açılmadığını doğrula; destek görevlisini bilinen kanal üzerinden teyit et; parola paylaşmadan destek sağla.

## Çalışılmış örnek
Ağda sorun yaşayan çalışan, beklenmeyen destek aramasını kapatıp yardım masasının kayıtlı numarasını arar. Bu, kaynağın ilkesinden türetilmiş kısa bir savunma senaryosudur; kitaptan birebir olay aktarımı değildir.

## Kaçınılacak hata
Sorunu çözen kişinin kimlik bilgisi istemeye yetkili olduğunu varsaymak.

## Bağlantılar
Kimlik ve yetki ayrımı için ana beceriyi; saldırı zincirleri için *Sızma Sanatı* bölüm notlarını oku. Kaynaktaki hikâyelerin çoğu yazarın belirttiği üzere kurgudur. Tarihsel teknik önerileri güncel kaynaklarla doğrula.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

* **Starboard Tersanesi ve ters toplum mühendisliği** — Anlatıya göre saldırgan, kendisini yardım masası görevlisi olarak tanıtıp kurbanın ağ port bilgisini almış, ardından kurumun ağ yönetim birimini arayarak ilgili portu devre dışı bıraktırmıştır. Bağlantısı kopan çalışan, sorunu çözeceğine inandırıldığı için saldırganın bıraktığı numarayı kendi isteğiyle aramış; sorun giderildikten sonra oluşan minnet ve suçluluk duygusuyla sistemine güvenlik yaması kisvesi altında bir Truva atı yüklemiştir. Ağ yönetiminin arayan kişinin kimliğini doğrulamadan portu kapatması ve kurbanın teyit edilmemiş bir kaynaktan dosya çalıştırması kontrolleri boşa çıkarmıştır.
* **İnsan Kaynakları üzerinden yeni çalışan listesinin sızdırılması** — Anlatıya göre saldırgan, şirket güvenliği biriminden aradığını ve yeni başlayanlara dönük eğitim planladığını iddia ederek İnsan Kaynakları çalışanından son bir ayda işe girenlerin isim ve dahililerini talep etmiştir. İlgili personel, arayanın kurumsal kimliğini ve yetkisini doğrulamaksızın listeyi hazırlayıp telefonda saldırgana okumuştur. Dahili bilgilerin yetkisiz kişilerle paylaşılmasını engelleyecek resmi teyit veya onay prosedürlerinin işletilmemesi bilginin sızmasına yol açmıştır.
* **Yeni personele yönelik parola avcılığı (Rosemary Morgan)** — Anlatıya göre bilgi güvenliği biriminden aradığını öne süren saldırgan, kurumsal güvenlik kurallarını anlatan destekleyici bir uzman rolüyle yeni çalışana yaklaşmıştır. Parola karmaşıklığı tavsiyesi verme bahanesiyle kurbanın mevcut parolasını ve yeni belirleyeceği şifreleme modelini adım adım konuşturarak doğrudan elde etmiştir. Kuruma yeni katılan personelin yardımseverlik ve uyum gösterme eğilimi istismar edilmiş; parola gizliliği ilkesinin henüz sistem erişimleri verilmeden personele benimsetilmemiş olması güvenlik açığı yaratmıştır.
* **GeminiMed sanayi casusluğu ve teslim baskısı (Craig Cogburne ve Steve Cramer)** — Anlatıya göre bir sanayi casusu; posta odası, tatildeki ekip lideri ve danışma görevlisi üzerinden adım adım ilerleyerek kritik bir tıbbi cihaz projesinin ekibini ve sistem bilgilerini faks yoluyla ele geçirmiştir. Ardından teknik destek kimliğine bürünerek hafta sonu proje teslimi yetiştirmeye çalışan başmühendisi aramış, sunucu arızası gerekçesiyle acil erişim sağlamak için kurbanın kullanıcı adı ve parolasını istemiştir. Danışma biriminin veri hassasiyetini gözetmemesi, varsayılan sistem hesaplarının açık unutulması ve teslimat stresi altındaki uzmanın kimlik sorgulamasını yarıda kesmesi nedeniyle tüm güvenlik bariyerleri aşılmıştır.

## Yazarın önerdiği karşı önlemler

* **Ters toplum mühendisliğine ve karşılıklılık tuzağına dikkat edilmesi:** Tanınmayan birinden gelen beklenmedik bir yardım ya da problem çözme vaadinin ardından istenen ayrıcalık ve bilgiler şüpheyle değerlendirilmeli; minnet duygusunun güvenlik sınırlarını aşmasına izin verilmemelidir.
* **Parola paylaşımının koşulsuz yasaklanması:** Sistem yöneticileri veya teknik destek dahil hiç kimseyle parolaların paylaşılmayacağına dair kesin kurallar konulmalı; istisnalara izin veren esnek yaklaşımlardan kaçınılmalıdır.
* **Yeni başlayanlara erişim öncesi güvenlik eğitimi:** Çalışanların kurumsal sistemlere erişimine izin verilmeden önce, başta kimlik ve parola gizliliği olmak üzere temel sosyal mühendislik tehditlerine karşı zorunlu eğitime tabi tutulmaları gerekir.
* **Rol ve risk odaklı eğitim modelleri:** Eğitimler tek tip olmamalı; danışma, sekreterlik ve insan kaynakları gibi saldırganların ilk temas kurduğu çevre birimlerin yanı sıra kritik verilere erişen uzmanlara iş profillerine uygun özel farkındalık kazandırılmalıdır.
* **Veri çıkış noktalarının denetlenmesi:** Şirket rehberi, çalışan listeleri ve teknik yapılandırmaların dışarıya (e-posta, faks vb.) aktarılması sıkı prosedürlere bağlanmalı; birimlerde bu tür talepleri değerlendirecek yetkili kontrol personeli belirlenmelidir.
* **Merkezi olay ve tehdit bildirim noktası:** Şüpheli bir arama veya yönlendirme ile karşılaşan çalışanların durumu gecikmeden aktarabileceği tek bir güvenlik iletişim merkezi kurulmalı; böylece planlı saldırılar erken aşamada tespit edilebilmelidir.
* **Geri arama ve rehber doğrulamasının yetersizliği:** Kurum içi rehberden isim kontrolü yapmak veya numarayı geri aramak her zaman güvenli sayılmamalıdır; arama yönlendirme ve sahte kayıt ihtimallerine karşı çok adımlı doğrulama uygulanmalıdır (güncel yorum: harici kanaldan bant dışı doğrulama zorunlu tutulmalıdır).

## Okuma kapsamı

Metin çıkarımındaki yaygın sözcük içi harf boşluklarına rağmen kaynağın tamamı okunmuş olup, içeriğin anlaşılmasını veya vakaların çözümlenmesini engelleyen herhangi bir belirsizlik bulunmamaktadır.
