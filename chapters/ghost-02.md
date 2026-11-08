# Ghost in the Wires — 02: Just Visiting

## Bölüm odağı
Okul bilgisayarı ve telefon altyapısıyla erken deneyimler. Bu bölüm birinci kişinin anı anlatısıdır; olaylar ve görüşler yazara atfedilmelidir.

## Uygulama ilkesi
Eğitim ağları için hesap yaşam döngüsü ve erişim sınırları tanımla.

## Kaynaktan örnek
Okul bilgisayarı ve RSTS/E işletim sistemiyle ilgilenirken telefon altyapısını da öğrenir.

## Karar ve uygulama
Öğrenci hesabının kullanabileceği sistemleri ve destek kanallarını açık tanımla. Kimlik doğrulama ile işlem yetkisini ayrı ele al; doğrulanamayan talepleri bilinen destek kanalına yönlendir.

## Sınır
Bu kısa not bölümün ayrıntılı okumasının yerine geçmez. Tarihsel uygulamaları güncel standartlara karşı değerlendir. Kaynak: İngilizce PDF, dosya sayfaları 15–24.

## Bölümün ayrıntılı okuması

- Anlatıcı okul ve üniversite bilgisayarlarında öğrendiğini; bir üniversite görevlisinin, kendisine şahsi hesabını kullanma izni verdiğini anlatır. Meşru öğrenme izniyle başkalarının kimlik bilgilerini toplamak arasındaki sınır daha sonra aşılır; erişim sonlandırılır.
- Telefon şirketi örneğinde bir geri arama kuralı bulunmasına rağmen telefon yönlendirmesi ve başka bir yetkili çalışanın taklit edilmesiyle bu kuralın etkisizleştirildiğini iddia eder. Savunma dersi, doğrulama kanalının da yönetilmesi gerektiğidir.
- Öğretmenin parolasını fiziksel ortamda saklama biçimiyle ilgili örnek, dijital sırrın korunmasının fiziksel çevreyi de kapsadığını gösterir.

## Karar modeli

Bir kontrolü değerlendirirken yalnızca son adıma bakma: (1) doğrulanan kişi kim, (2) doğrulama hangi kanala dayanıyor, (3) o kanal kim tarafından değiştirilebilir, (4) istenen işlem için yetki ayrıca kontrol ediliyor mu? Bunlar bölümden çıkarılmış değerlendirme sorularıdır; yazarın adlandırdığı bir model değildir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Yayımlanmamış numaraların geri arama atlatılarak elde edilmesi** — Kitaba göre anlatıcı, telefon şirketinin yetkili birimlerini arayıp kurum içi rol ve terminolojiyi taklit ederek gizli abone numaralarını talep etmiştir. Şirketin "yetkili dahili numaraya geri arama" kontrolü; ilgili hatta sosyal mühendislikle çağrı yönlendirme yaptırılması ve teyit aramasının harici bir devrede karşılanması nedeniyle atlatılmıştır. Hat üzerinde yetkisiz yönlendirme olup olmadığı denetlenmediği için güvenlik kontrolü işlevsiz kalmıştır.
- **Delikli kağıt banttaki sistem parolasının görsel olarak okunması** — Anlatıya göre öğretmen, minibilgisayar parolasının klavyeden gözetlenmesini engellemek amacıyla parolayı delikli kağıt banda basmış, ancak bandı gömlek cebinde taşımıştır. Dijital gizlilik önemsenirken fiziksel çevre güvenliği göz ardı edilmiş; delik desenlerinin ince kumaş arkasından görsel olarak çözümlenebileceği hesaba katılmadığı için parola ifşa olmuştur.
- **Kısıtlı okul telefonundaki mekanik kadran kilidinin aşılması** — Laboratuvar telefonunun harici sistemleri aramasını engellemek amacıyla döner kadrana fiziksel kilit takılmıştır. Ancak şebekenin darbe sinyalleşmesini (pulse dialing) ahize çatalındaki basışlarla da kabul etmesi sebebiyle, fiziksel kısıtlama mantıksal sinyal düzeyindeki açığı kapatamamış ve arama engeli işlememiştir.
- **CSUN laboratuvarında sahte oturum açma yazılımıyla kimlik avı** — Anlatıya göre Mitnick, üniversite terminallerinde işletim sisteminin giriş ekranını taklit eden bir program çalıştırarak öğrencilerin hesap ve parolalarını gizlice kaydetmiştir. Sistem ile kullanıcı arasında güvenilir bir oturum açma yolu (trusted path) bulunmadığı ve kullanıcılar oturum ekranının gerçekliğini sorgulamadığı için kimlik doğrulama mekanizması istismar edilmiştir.
- **Sunset-Gower santral binasına fiziksel sızma ve sahte teyit** — Kitaba göre anlatıcı ve arkadaşı, sosyal mühendislikle elde ettikleri giriş koduyla telefon santraline gece izinsiz girmiş ve güvenlik görevlisine yakalanmıştır. Görevlinin teyit amacıyla aradığı amirle görüşmeyi Mitnick devralıp tek taraflı bir diyalog sahnelemiş; görevlinin amiri bizzat dinlemeyip çekince göstermesi ve süreci sonuna kadar takip etmemesi nedeniyle fiziksel erişim denetimi başarısız olmuştur.

## Yazarın önerdiği karşı önlemler

- **Geri arama mekanizmalarında hat bütünlüğünün doğrulanması (çıkarım)**: Kritik bilgi paylaşımı öncesinde yapılan geri aramalarda yalnızca kayıtlı dahili numara aranmamalı; hat üzerinde etkin bir çağrı yönlendirme (call forwarding) bulunup bulunmadığı ve çağrının harici bir hatta iletilmediği doğrulanmalıdır.
- **Fiziksel erişim denetimlerinde teyit sürecinin tavizsiz yürütülmesi (çıkarım)**: Güvenlik personeli, kurum kimliği olmayan kişilerin sözlü beyanlarına veya şüphelinin yürüttüğü telefon görüşmelerine güvenmemeli; yetkili amirle görüşmeyi bizzat tamamlayıp doğrudan onay almalı ve resmi kimlik doğrulanana dek geçişe izin vermemelidir.
- **Fiziksel ortamdaki kimlik bilgilerinin gözetlemeye karşı korunması (çıkarım)**: Parola veya erişim kodları kağıt ve delikli bant gibi fiziksel materyallerde saklanıyorsa, bunların başkaları tarafından görülebilecek veya okunabilecek açık alanlarda taşınması engellenmelidir.
- **Terminallerde güvenilir oturum açma yolu (trusted path) oluşturulması (çıkarım)**: Çok kullanıcılı sistemlerde yetkisiz kullanıcıların sahte giriş ekranları oluşturmasını engellemek için doğrudan işletim sistemi çekirdeğine bağlı güvenli oturum açma mekanizmaları devreye alınmalıdır.
- **Mekanik engellerin mantıksal ve sinyal düzeyinde desteklenmesi (çıkarım)**: İletişim cihazlarındaki erişim sınırlandırmaları yalnızca mekanik kilitlerle bırakılmamalı; hattın altyapı düzeyinde de kısıtlanması sağlanarak alternatif sinyalleşme yöntemleriyle kontrollerin aşılması önlenmelidir.
- **Yönetici ve imtiyazlı hesaplarda temel parola disiplini (çıkarım)**: Sistem yöneticisi ve yetkili kullanıcı hesaplarında tahmin edilebilir basit şifreler (örneğin kullanıcı adı) kullanılmamalı, güçlü parola politikaları zorunlu tutulmalı ve hesaplar üçüncü taraflarla paylaşılmamalıdır.

## Okuma kapsamı
Bölüm başındaki kısa şifreli bulmaca hariç kaynağın tamamı okunmuştur; metin bozukluğu nedeniyle belirsiz kalan bir yer bulunmamaktadır.
