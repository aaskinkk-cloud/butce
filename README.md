# Bütçe & Hedef

## Android uygulaması (APK) — 23.10.2026
**İndir:** https://github.com/aaskinkk-cloud/butce/releases/download/android/butce.apk

- 1.3 (29.10.2026): Okur uygulamasındaki alıntıları alır.
- 1.2 (29.10.2026): Kaydettikten sonra "Dosyayı aç / Klasörü aç" sorusu.
- 1.1 (28.10.2026): Okur uygulamasıyla aynı güncel kabuk — GitHub açılmazsa kendiliğinden Cloudflare yedeğinden (ahmet-uygulamalar.pages.dev/butce) açılır; simge: mavi zemin, sütun grafiği ve altın sikke.
- Kalıcı tam ekran (Android'in kendi yöntemi): alttaki tuşlar kaydırılınca sayfanın **üstüne biner**, sayfa kaymaz; Chrome'un tam ekran uyarısı ve "Dokunarak ara" paneli yoktur. Ön kamera bölgesi sayfanın renginde, içerik kameranın altından başlar. Ekran açık kalır.
- Sayfa GitHub'daki Bütçe'dir; buraya gönderilen her güncelleme uygulamaya kendiliğinden gelir.
- Dosya indirmeleri **İndirilenler** klasörüne kaydedilir; dosya seçimi telefonun dosya seçicisiyle yapılır.
- Verisi Chrome'dakinden **ayrıdır**: ilk açılışta Chrome'daki sürümden **Yedek indir**, uygulamada **Yedekten geri yükle**.
- Kaynak `android/`; APK'yı GitHub Actions derler. İmza anahtarı (`android/okur.jks`) sabittir: yeni sürüm eskisinin üzerine kurulur, veriler silinmez.

## 4.0 (30.10.2026) — Hedefler: her hedef ayrı bölüm, alındı tarihi
- Satır düzeni: **Ürün | Adet | Birim fiyatı | Tutar**; tutar = adet × birim fiyatı (otomatik), tutar elle yazılırsa birim fiyatı geri hesaplanır. Eski kayıtlar adet 1, birim = tutar.
- Görünüm seçimi (Alıntılar'daki seçiciyle aynı): **Liste** ya da **Her hedef ayrı bölüm**. Bölüm görünümünde her hedef kendi renkli kartında: başlıkta ad, bağlantı, ⋯; ortada Adet × Birim fiyatı = Tutar kutuları; altta Alınacak/Alındı onayı.
- Onay işaretlenince **günün tarihi** kaydedilir ve gösterilir (listede satırın altında yeşil "Alındı" etiketi, bölümde onayın yanında); tarih dokunularak değiştirilebilir. Onay kaldırılınca tarih silinir.
- Kopyala/Yazdır: Adet, Birim fiyatı, Alındı tarihi sütunları.
- 3.9'daki kişi bölümleri kaldırıldı.

## 3.8 (29.10.2026) — Okur alıntıları Android'de yeniden geliyor
- Okur ve Bütçe ayrı Android uygulamaları olduğu için Bütçe, Okur'daki vurguları göremiyordu. Bütçe uygulaması (1.3) artık alıntıları doğrudan **Okur uygulamasından** ister; Alıntılar sekmesine "Okur" kategorisiyle gelir. Yalnız Bütçe okuyabilir (imza denetimi).
- Gerekenler: yeni **Okur** ve **Bütçe** APK'ları; güncellemeden sonra Okur'u bir kez açmak.
- Chrome'da (aynı adreste) eski yol, Okur'un tarayıcı verisinden okuma, aynen sürüyor.

## 3.7 (29.10.2026) — Şifreler: toplu yapıştır, otomatik dağıt
- Kasanın üstünde **Toplu yapıştır — gruplara otomatik dağıt** düğmesi: listenin tamamı yapıştırılır, her satır site adına ve mail adresine göre bölüme yerleşir (Gmail/Yandex/Hotmail → mail; Trendyol, Hepsiburada… → alışveriş; bankalar, Papara → banka; e-Devlet, MHRS, SGK… → resmi; MEBİS, TAKPAS, BelgeNet, .gov.tr adresleri → iş/kurum; Instagram, Facebook… → sosyal; tanınmayanlar → Diğer).
- Eklemeden önce önizleme: bölüm başına sayı ve her satırın yanında bölüm seçici; yanlış düşeni değiştir. Aynı site + kullanıcı + şifre zaten varsa tekrar eklenmez; "Geri al" çalışır.
- Bölüm adını değiştirsen de eşleşme ada göre yapılır (ör. adında "mail", "alış", "banka", "devlet", "kurum", "sosyal" geçmesi yeter).

## 3.6 (29.10.2026) — Şifre sayfası hep güncel gelir
- `sifre.html` önce internetten yükleniyor (Bütçe sayfası gibi); telefonda kalan eski sürüm yüzünden kasa boş görünmez. İnternet yoksa son kaydedilen sürüm açılır.

## 3.5 (29.10.2026) — Şifre Kasası boş sayfa düzeltmesi
- Kasa açıldıktan sonra kilit ekranının yeri boş bir sayfa olarak kalıyor, kayıtlar aşağıya kayıyordu; kilit ekranı artık tamamen kalkıyor.

## 3.4 (29.10.2026) — Şifre sekmesi düzeltmesi
- Şifre Kasası çerçevesi ekranın küçük bir kısmında kesik görünüyordu; artık üst başlıkla alt çubuk arasını tam dolduruyor (döndürmede de).
- Alt çubuk adları kısaldı: Bütçe · Fındık · Hedef · Düğün · Zikir · Alıntı · Şifre.

## 3.3 (29.10.2026) — Şifreler sekmesi (Şifre Kasası)
- Alt çubuğa **Şifreler** sekmesi eklendi. Ana şifreyle açılır; Gmail, Alışveriş, Banka & ödeme, e-Devlet & resmi, İş / kurum, Sosyal medya, Diğer bölümleri her biri ayrı renk ve simgeyle gelir. Bölüm ekle / adlandır / renk / sırala / sil; kayıt ekle, düzenle, başka bölüme taşı, toplu yapıştır; şifre göster, kopyala, güçlü şifre üret; arama.
- **Güvenlik:** kayıtlar ana şifreden türetilen anahtarla (PBKDF2-SHA256 310.000 tur, AES-GCM 256) şifrelenir ve yalnız bu cihazda durur. Bütçe verisine girmez, Milli Emlak köprüsüne gönderilmez. Sekmeden çıkınca, 5 dk işlem olmayınca ya da 1 dk başka uygulamaya geçince kilitlenir. Ana şifre unutulursa kayıtlar açılamaz.
- **Yedek:** Kasa menüsünden şifreli metin olarak kopyala ya da dosya olarak kaydet. Bütçe'nin **Yedek indir** dosyası da kasayı şifreli hâliyle içerir; geri yüklerken kasanın yerine konup konmayacağı sorulur.
- Kasa ayrı sayfadır: `sifre.html`. Tek başına da açılır.
- Düzeltme: 3.2 güncellemesinde `sw.js` (çevrimdışı çalışma dosyası) yanlışlıkla boş yüklenmişti; geri getirildi. İnternetsiz açılış yeniden çalışır.

## 3.2 (29.10.2026) — Silme onayı, kaydettikten sonra aç
- **× ve çöp kutusu** ile tek kayıt silerken önce "Silmek istediğinizden emin misiniz?" sorulur (bütçe kalemi, fındık kalemi/geliri, düğün, hedef, zikir, alıntı). Onaydan sonra "Geri al" yine çalışır.
- **Yedek indir** sonrası soru: *Dosyayı aç / Klasörü aç / Hayır*. Android uygulamasında dosya telefondaki uygun uygulamayla, klasör İndirilenler'de açılır. Chrome'da yalnız *Dosyayı aç* vardır (tarayıcı klasör açamaz).
- Android 1.2: kayıttan sonra kısa bildirim yerine bu soru çıkar. Yeni APK'yı aynı bağlantıdan indirip üzerine kur; veriler silinmez.

## 3.1 (29.10.2026) — Düğün defteri eşitlendi
- Verilen takı listesindeki **62 kayıt** (2019–2026) Düğünler sekmesine eklendi; liste tarihe göre sıralanır. Tarihsiz kayıt ("İbrahim Güney oğlu") en sonda.
- Mevcut kayıtlar silinmez; aynı kişi + tarih + tutar + tür zaten varsa yeniden eklenmez. Ekleme bir kez yapılır, sildiğin kayıt geri gelmez.
- **Yeniden kurulumda varsayılan:** Uygulama sıfırdan kurulduğunda (veri yokken) tüm zikir/dua kayıtları (74) ve düğün kayıtları (63) kendiliğinden gelir.
- Yorumlanan satırlar: "30 Temmuz" → 2023; Kemal Bilgin 22.06.**2022** → 2024 (dolar 32 TL o yıla ait); "100+300" → nişan 100 + düğün 300 iki kayıt; "Dolar" → Nakit USD; "çeyrek" → 1 Çeyrek Altın.

## 3.0 (29.10.2026) — Zikir listesine eklemeler
- **31 yeni kayıt** (dua, niyet, olumlama, ayet, şifa, korunma) ve **1 alıntı** (Mecelle md. 4 — Hikmet) eklendi: haşere duası, nazar duası, kapı aç duası, iftar duası, Târık Sûresi, Fâtiha meali, Bakara 222, Zuhruf 79, Hıdırellez / anne bağı / değer (Yâ Habîb) niyetleri vb.
- Eksik kalmış 9 kaydın metni tamamlandı (Bolluk niyeti, Sağlık olumlaması, Felak meali, Ahkâf 15, Evlat için…). **Senin değiştirdiğin kayıtlara dokunulmaz**; yalnız hiç düzenlenmemiş olanlar tamamlanır.
- Eklemeler **telefondaki mevcut verine** de gelir: güncellemeden sonraki ilk açılışta bir kez eklenir, listenin sonuna düşer. Aynı metin zaten varsa eklenmez; sildiğin kayıt bir daha geri gelmez.

## 2.9 (23.10.2026) — Tam ekran düğmesi geri
- Kurulu uygulamada gizlenen tam ekran düğmesi yeniden görünür ve çalışır. Düğmeye basınca Chrome kendi "Tam ekrandan çıkmak için…" uyarısını bir kez gösterir (tarayıcı kuralı). Dokununca kendiliğinden tam ekran isteği gönderilmez.

## 2.8 (22.10.2026) — Kurulu uygulamada tam ekran düğmesi
- Ana ekrandan yüklenen uygulama baştan tam ekran açıldığı için tam ekran düğmesi gizlendi ve basılsa da tam ekran isteği gönderilmez. Önceden düğmeye basınca uyarı çıkıyor, sayfa yeniden diziliyor, yazılar kayboluyor / sayfa değişiyordu.

## 2.7 (22.10.2026) — Tam ekran uyarısı kesin çözüm
- Sayfanın kendiliğinden tam ekrana geçme istekleri (ilk dokunuşta, açılışta, dosya seçiciden dönünce) **tamamen kaldırıldı**; Chrome'un "Tam ekrandan çıkmak için…" uyarısı ekrana dokununca artık çıkmaz. Tam ekran isteği yalnız tam ekran düğmesine basınca gönderilir. Ana ekrandan yüklenen uygulama zaten tam ekran açılır.

## (22.10.2026) — Açılışta tam ekran
- Ana ekrandan açılınca uygulama **doğrudan tam ekran** gelir (`manifest.webmanifest`: `"display": "fullscreen"`). Tarayıcı içinden tam ekran isteği gönderilmediği için Chrome'un "Tam ekrandan çıkmak için…" uyarısı da çıkmaz.
- Daha önce yüklenmiş simge eski ayarla açılabilir: simgeyi kaldırıp Chrome › ⋮ › **Uygulamayı yükle** ile yeniden yükle.

## 2.6 (22.10.2026) — Sessiz ekran
- **Tam ekran uyarısı:** Ana ekrandan açılan (kurulu, tam ekran) uygulamada içeriden tam ekran isteği gönderilmez → Chrome'un "Tam ekrandan çıkmak için yukarıdan sürükleyip…" uyarısı çıkmaz. Chrome sekmesinde tam ekrana her girişte bu uyarıyı tarayıcı kendisi gösterir; sayfa kapatamaz.
- **Kelimeye dokununca Google paneli:** Chrome'un "Dokunarak ara" paneli açılmasın diye sayfa (ve içindeki çerçeveler) dokunuşu kendisi karşılar. Uzun basıp seçme çalışır.
- Blok `/* SESSİZ EKRAN */` adıyla `index.html`'in başındadır; tüm uygulamalarda aynıdır.

Aylık bütçe, fındık sarfı, hedefler, düğün takıları, zikir ve alıntıları tek yerde tutan, telefonda çalışan kişisel bir web uygulaması (PWA).

**Uygulamayı aç:** https://aaskinkk-cloud.github.io/butce/

## Bölümler

| Sekme | Ne işe yarar |
|---|---|
| **Bütçe** | Aylık gelir, bölüm bölüm kalemler, ödendi işareti, plan bölümleri (Σ toplama dahil/dışı), üstte sabit özet (toplam · ödenen · kalan) |
| **Fındık** | Fındık sezonu masrafları ve gelirleri |
| **Hedefler** | Biriktirme ve alım hedefleri |
| **Düğünler** | Takılan/alınan takılar; yıl, kişi, yön ve türe göre bölümler |
| **Zikir** | Zikir ve dualar, günlük sayaç, favoriler |
| **Şifreler** | Ana şifreyle açılan şifreli kasa; renkli bölümler, kopyala/göster, toplu yapıştır |
| **Alıntılar** | Alıntılar; kategori, yazar ve kitaba göre listeleme, toplu yapıştırmada yazar tanıma |

Bütçe ekranında her açılışta rastgele bir zikir ve alıntı gelir (★ favorilerden ya da tümünden).

## Kullanım ipuçları

- **Kalem taşıma:** ⋮⋮ tutamağına **dokun** → taşıma menüsü; **basılı tut ve sürükle** → sırayı değiştir.
- **Süzgeç:** Bölümde *Tümü / Ödenmemiş* seçimi hatırlanır.
- **Yeni dönem:** Önceki ayın kalemleri kopyalanır.

## Kurulum

Chrome'da adresi aç → menü → **Ana ekrana ekle**. İnternetsiz de çalışır; yeni sürüm çıkınca ekranda "Yenile" görünür.

## Veriler

Tüm veriler **yalnız bu cihazın tarayıcısında** saklanır; hiçbir sunucuya gönderilmez. Tarayıcı verilerini silmek kayıtları da siler; düzenli olarak menüden **Yedek indir** ile yedek al.

## Dosyalar

| Dosya | Açıklama |
|---|---|
| `index.html` | Uygulamanın tamamı (tek dosya) |
| `sw.js` | Çevrimdışı önbellek ve sürüm güncelleme |
| `manifest.webmanifest`, `icon-*.png` | Ana ekran simgesi ve uygulama bilgileri |

## Sürüm

**2.5** — Zikir/alıntı bandındaki **Tümü** düğmesi düzeldi: yazı düğmenin içinde ortalı, taşmıyor, üstte kalmıyor.  
2.4 — Arama motorları için sayfa bilgileri (başlık, açıklama, paylaşım önizlemesi); uygulama işleyişi aynı.  
2.3 — Zikir ve alıntı bantlarında renkli şerit sağa alındı.  
2.2 — Zikir/alıntı kartında ★ sağ üstte, kategori başlıkla aynı satırda, alt düğmeler tek satırda.  
2.1 — Kalem taşıma yalnız basılı tutunca; rastgele zikir/alıntı favorilerden ya da tümünden; kesik çizgiler kaldırıldı.  
2.0 — Sabit küçülen özet, bölümde Σ dahil/dışı, kalem sürükle/taşı/çoğalt.
