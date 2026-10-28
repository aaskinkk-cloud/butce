# Bütçe & Hedef

## Android uygulaması (APK) — 23.10.2026
**İndir:** https://github.com/aaskinkk-cloud/butce/releases/download/android/butce.apk

- 1.1 (28.10.2026): Okur uygulamasıyla aynı güncel kabuk — GitHub açılmazsa kendiliğinden Cloudflare yedeğinden (ahmet-uygulamalar.pages.dev/butce) açılır; simge: mavi zemin, sütun grafiği ve altın sikke.
- Kalıcı tam ekran (Android'in kendi yöntemi): alttaki tuşlar kaydırılınca sayfanın **üstüne biner**, sayfa kaymaz; Chrome'un tam ekran uyarısı ve "Dokunarak ara" paneli yoktur. Ön kamera bölgesi sayfanın renginde, içerik kameranın altından başlar. Ekran açık kalır.
- Sayfa GitHub'daki Bütçe'dir; buraya gönderilen her güncelleme uygulamaya kendiliğinden gelir.
- Dosya indirmeleri **İndirilenler** klasörüne kaydedilir; dosya seçimi telefonun dosya seçicisiyle yapılır.
- Verisi Chrome'dakinden **ayrıdır**: ilk açılışta Chrome'daki sürümden **Yedek indir**, uygulamada **Yedekten geri yükle**.
- Kaynak `android/`; APK'yı GitHub Actions derler. İmza anahtarı (`android/okur.jks`) sabittir: yeni sürüm eskisinin üzerine kurulur, veriler silinmez.

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
