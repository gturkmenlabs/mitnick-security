# Sızma 11: Kıssalar

## Temel fikir
Kısa vakalar, sıradan varsayılanlar ve günlük davranışların güvenlik sonuçları doğurabileceğini gösterir.

## Uygulama
Varsayılan kimlik bilgilerini kaldır; kimlik bilgilerini paylaşmadan destek süreci tasarla; örneklerden ölçülebilir kontrol çıkar.

## Kaçınılacak hata
Bir teknik destek işi için başkasının parolasının rutin olarak istenmesi.

## Çalışılmış örnek
Destek görevlisi kullanıcı parolasını öğrenmeden yetkili destek yolunu kullanır.

## Kaynak sınırı
Bu dosya kaynakların ilgili ana kısmından çıkarılmış uygulama notudur. Örnek, anlatıdan çıkarılan savunma senaryosudur; doğrudan alıntı değildir. Tarihsel teknik önerileri güncel standartlarla doğrula.

## Kaynak örneği ve karar gerekçesi
Kısa öykülerden biri iki kişinin aynı yanlış kaydı girmesiyle hatalı kaydın onaydan geçebileceğini; bir diğeri varsayılan ve kolay tahmin edilebilir parolaların yarattığı tehlikeyi gösterir.

## Kontrol adımları
Çift girişin bağımsızlığını ve yetki ayrımını değerlendir; kayıt değişikliklerini denetle; kullanıcı parolasını istemeden destek verebilen iş akışları kur.

## Kaynak
*The Art of Intrusion*, Çince çeviri PDF, dosya sayfaları 275–289; Türkçe çevirinin 11. bölümü aynı esere aittir. Öyküler görüşmelere dayanır; ayrıntılar değiştirilmiş ve bazı iddialar bağımsız doğrulanmamış olabilir.

<!-- kaynak-okumasi -->
## Kaynaktaki vakalar

- **Kaybolan maaş çeki** — Anlatıya göre Jim (Fort Lewis) ve arkadaşları, kendilerine kötü davranan üstçavuşu cezalandırmak için maaş kaydına onu "ölü" olarak girdi. Çift giriş kuralı vardı, ama iki girişi de aynı ekip yaptığı için bağımsız doğrulama sağlamadı; kâğıt dosya da bulunamayınca ödeme durdu.

- **Hollywood'da bir genç** — Kitaba göre 16 yaşındaki Yuki, Jurassic Park sitesinin zayıf web korumasından tam erişim elde etti, ardından iş ortağının ağı üzerinden iç ağdaki yapı çizimlerine ulaştı. Arkadaşıyla sitenin logosunu değiştirdiler; şirket açığı bildirilince iş teklif etti, yaşı nedeniyle ücret anlaşmazlığı çıktı.

- **İçecek otomatı** — David'in anlatımına göre Coca-Cola'nın Unix'e bağlı deneme otomatlarında açık bir oturum bulundu ve parola birkaç denemede tahmin edildi. Yazılımın kaynak kodu makinenin üzerinde olduğu için çıktıya kendi mesajları eklenebildi; zayıf parola ile üretimde kaynak kod bulundurma birleşti.

- **Çöl Fırtınası** — Mike'ın anlatımına göre ABD istihbaratı Irak telsizlerini dinledi; Farsça bilen bir dinleyici çağrı işaretlerini taklit ederek komuta düzenini karıştırdı. Frekans değişiklikleri taramayla, yer altı telefonlarına geçiş hat dinlemeyle karşılandı, kuryeyle emir taşıma da hedef alındı. Telsizde ve kabloda karşı tarafın kimliğini doğrulayan bir mekanizma yoktu.

- **Milyar dolarlık kupon** — Bir sızma testinde ekip, şifrelemeyi değil kupon kullanım uygulamasındaki komut çalıştırma açığını hedef aldı. Aynı alt ağdaki kupon basma makinesine güven ilişkisi üzerinden geçilip geçerli ve çok yüksek değerli bir kupon üretildi; ağ bölümlendirmesi ve uygulama girdisi denetimi yoktu.

- **Poker botu** — Kitaba göre Ron, çevrimiçi Texas Hold'em'de insan gibi görünen güçlü bir bot yazdı ve turnuvalarda derece aldı. Botu satmaya başlayınca siteler tespit kodu ekledi ve yakalananları yasakladı; Ron gizli kart paylaşan "takım" kipine geçti. İnsan doğrulaması ve çoklu hesap korelasyonu zayıftı.

- **Genç ve avcı** — 15 yaşındaki anlatıcı, bir sohbet odasında çocuk istismarı görselleri arayan biriyle temas kurdu. Antivirüs ilk denemeleri engelledi; anlatıcı güvenlik sorularından hesap erişimi ve güvenilen bir kaynaktan geliyormuş gibi görünen bir dosyayla sonuç aldı. Kitap öykünün kısmen veya tamamen uydurma olabileceğini belirtir; mekanizma teknik değil, ikna ve güvendir.

- **Hacker olmaya gerek yok** — John, elektrik şirketindeki stajında Lotus Notes yükseltmesi bahanesiyle çalışanlardan parolalarını istedi ve çoğu çekinmeden verdi. Varsayılan parolalar, yapıştırılmış notlar ve kişisel eşyalardan çıkan ipuçları sayesinde çoğunu kısa sürede tahmin etti; zayıf seçim ile kolay bulunabilirlik birleşti.

## Yazarın önerdiği karşı önlemler

- Kitabın kapanış mesajı parola hijyenine dayanır: kullanıcı parolasını değiştirmeli ve yeni parolayı kolayca bulunacak bir yerde bırakmamalı.
- Kitaba göre ilk savunma hattı aynı zamanda en zayıf halkadır: kullanıcılar ve onların parola seçimleri.
- Açılış epigrafı savunmanın yönünü işaret eder: saldırganlar kırılmamış şifreleme yerine uygulamalarda tekrar tekrar yapılan hataları arar.
- Kitaba göre poker sitelerinin verdiği yanıt, bot tespit kodu ve kalıcı yasak oldu.
- Yuki vakasında Universal'in açığı bildiren kişiyi dinlemesi ve işe almayı düşünmesi, kitapta olumlu karşılanan bir tepki olarak aktarılır.

## Okuma kapsamı

Kaynağın tamamı okundu; Türkçe çıkarımdaki harf aralığı bozuklukları ve yinelenen bölüm numaralandırması (iki ayrı 11.7) dışında belirsiz yer yok, ancak çocuk istismarcısı öyküsünün doğruluğu kitabın kendisi tarafından kuşkulu bırakılıyor.
