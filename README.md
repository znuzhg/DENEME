# 🎥 OBS İLE KICK’TE YAYIN AÇMA (ADIM ADIM)

## 1️⃣ OBS’Yİ İNDİR VE KUR
1. Tarayıcıdan aç: https://obsproject.com
2. İşletim sistemini seç (Windows / macOS / Linux)
3. İndir → Kur → Next → Next → Finish
4. İlk açılışta Auto-Configuration Wizard çıkarsa:
   - Optimize for streaming → Next → Next → Finish

## 2️⃣ KICK’TEN STREAM KEY AL
1. https://kick.com adresine gir
2. Hesabına giriş yap
3. Sağ üst → Profil Fotoğrafı
4. Creator Dashboard
5. Settings → Stream
6. Stream URL ve Stream Key’i al (Stream Key gizlidir)

## 3️⃣ OBS → STREAM AYARLARI (EN ÖNEMLİ ADIM)
1. OBS aç
2. Settings → Stream
3. Ayarları aynen gir:
   - Service: Custom
   - Server: rtmp://fa.kick.com/app
   - Stream Key: Kick’ten aldığın key
4. OK bas

## 4️⃣ OBS → OUTPUT (YAYIN KALİTESİ)
1. Settings → Output
2. Output Mode: Advanced
3. Streaming sekmesi:
   - Encoder: NVENC (varsa) / x264
   - Bitrate: 5000 kbps
   - Keyframe Interval: 2
   - Preset: Quality
   - Profile: High

### Düşük Sistem İçin
- Bitrate: 3500 kbps
- Preset: Performance

## 5️⃣ OBS → VIDEO AYARLARI
1. Settings → Video
2. Ayarları gir:
   - Base (Canvas) Resolution: 1920x1080
   - Output (Scaled) Resolution: 1280x720
   - Downscale Filter: Lanczos
   - FPS: 60

### Zayıf PC İçin
- FPS: 30

## 6️⃣ SAHNE VE KAYNAK EKLE
1. Scenes → + → Sahne oluştur (Örn: Yayın)
2. Sources → +
   - Display Capture → Ekran yayını
   - Game Capture → Oyun yayını (Capture specific window)
   - Video Capture Device → Kamera (opsiyonel)

## 7️⃣ MİKROFON AYARI
1. Settings → Audio
2. Mic/Auxiliary Audio: Mikrofonunu seç
3. Desktop Audio: Kulaklık / hoparlör
4. Mikrofon → Filters:
   - Noise Suppression
   - Compressor

## 8️⃣ YAYINI BAŞLAT
1. OBS ana ekranda Start Streaming
2. Kick’te yayın 3–10 saniye içinde başlar

## 9️⃣ KICK’TE BAŞLIK VE KATEGORİ
1. Creator Dashboard
2. Title (Yayın başlığı)
3. Category (Just Chatting / Oyun)
4. Save

## ❗ YAYIN AÇILMIYORSA KONTROL ET
- Stream Key doğru mu
- OBS açık mı
- VPN kapalı mı
- Bitrate çok yüksek mi
- Kick hesabın yayın yetkili mi

## ✅ TAMAM
Bu adımları eksiksiz yaptıysan OBS üzerinden Kick’te yayın sorunsuz şekilde başlar.
