# Bütçe & Hedef

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
