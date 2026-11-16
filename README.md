# Extraiş tanıtım sitesi

Tek sayfalık, statik tanıtım sitesi. Önizleme: https://emreguven35.github.io/extrais-tanitim/

## İçerik

- `index.html`: sayfanın tamamı (HTML, CSS ve JavaScript tek dosyada)
- `assets/`: logo, ikon ve uygulama ekran görüntüleri

Derleme adımı, sunucu tarafı kod ve paket bağımlılığı yok. Dışarıdan yalnızca Google Fonts üzerinden Plus Jakarta Sans yükleniyor.

## Yayına alma

1. `index.html` dosyasını ve `assets/` klasörünü, aynı klasör yapısıyla alan adının kök dizinine koyun. Dosya yolları görelidir; alt klasörde de çalışır.
2. Site HTTPS üzerinden sunulmalı.

## Yayından önce yapılacaklar

1. **Google Play bağlantısı:** `index.html` içinde `GOOGLE_PLAY_URL` satırını bulun ve tırnakların arasına mağaza adresini yazın. Boş kaldığı sürece Google Play butonu "bağlantı henüz eklenmedi" uyarısı gösterir.
2. **Arama motorları:** Bu depodaki sürüm geçici önizleme olduğu için `<head>` içinde `<meta name="robots" content="noindex">` satırı var. Canlı sitede bu satır silinmeli. (Ayrıca gönderilen zip dosyasında bu satır zaten yok.)

App Store bağlantısı hazır (`APP_STORE_URL`).

## Notlar

- Karanlık mod yok; sayfa bilerek tek temalı.
- Kum saati animasyonu `<canvas>` ile kodla çiziliyor, video ya da hazır görsel değil. "Hareketi azalt" ayarı açık olan cihazlarda tek karelik sabit hali gösterilir.
- Masaüstü Chrome'da ve telefon boyutunda test edildi. Yayından sonra gerçek iPhone (Safari) ve Android cihazda bir kez kontrol edilmesi iyi olur.
