# Murat Can Cihanyandı

Full-stack geliştirici · Python & TypeScript · Raspberry Pi üzerinde kendi kendine barındırılan üretim sistemleri

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](#)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](#)
[![Next.js](https://img.shields.io/badge/Next.js-000000?logo=next.js&logoColor=white)](#)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](#)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](#)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](#)

---

## Ne yapıyorum

Yazılımı **çalışan sistemler** olarak görüyorum. Buradaki projelerin çoğu
Raspberry Pi 5 üzerinde CasaOS/Docker ile 7/24 çalışıyor; bir kısmı gerçek
kullanıcıya hizmet ediyor.

Üç konu etrafında birleşiyorlar:

- **Uçtan uca ürün** — sepet/sipariş/ödeme akışı, admin ve satıcı panelleri, kargo
  takibi; iş kuralları istemci ve sunucuda tek kaynaktan yönetilir.
- **Kısıtlı donanımda üretim** — ARM64 multi-arch imajlar, düşük RAM'de çalışan
  servisler, tek konteyner dağıtımı, kendi kendine güncellenen Android kabukları.
- **Güvenlik ve veri bütünlüğü** — kaotik sistem tabanlı anahtar üretimi +
  ChaCha20-Poly1305 ile şifreli tıbbi görüntü aktarımı, JWT sertleştirme, HTML
  temizleme, denetim kaydı.

---

## Öne çıkan projeler

### 🛒 [Fakeyol](https://github.com/muratcihanyandi/fakeyol) · [fakeyol.com](https://fakeyol.com)
Tam yığın e-ticaret platformu — Next.js 15 + Express + PostgreSQL.
**58 API ucu**, 15 sayfa, 11 Prisma modeli; JWT sertleştirme, hız sınırlama,
tek kaynaklı kargo/kupon kuralları ve sipariş durum makinesi (7 statü + kurye
rota simülasyonu). ARM64 native Docker imajı, Pi 5 üzerinde üretimde.
`TypeScript` `Next.js` `Express` `Prisma` `PostgreSQL` `Docker`

### 🎬 [AutoShorts Studio v2](https://github.com/muratcihanyandi/autoshorts-studio-v2) · [ass.fakeyol.com](https://ass.fakeyol.com)
YouTube / Twitch / Kick yayınlarından otomatik dikey klip (Shorts/Reels/TikTok)
üreten ve yayınlayan otonom stüdyo. Backend (FastAPI) + frontend (React) +
mobil (React Native/Expo) tek üründe; Whisper transkripsiyon, LLM tabanlı klip
seçimi, kuyruk yönetimi, kurulum sihirbazı.
`Python` `FastAPI` `React` `React Native` `FFmpeg` `Whisper`

### 📡 [AutoShorts Hub](https://github.com/muratcihanyandi/autoshorts-hub)
Çok kanallı YouTube operasyon motoru: kanalları 7/24 izler, zaman serisi
istatistik toplar, **kural motoruyla** yayın planlar (*aynı içerik iki kanala
aynı gün gitmez*, kanallar arası ≥7 gün, kanal başına günlük limit, yayın
penceresi) ve OAuth ile doğrudan YouTube'a yükler. Kural motoru birim testli.
`Python` `FastAPI` `SQLAlchemy` `APScheduler` `PostgreSQL`

### 🔐 [DICOM Secure Transfer](https://github.com/muratcihanyandi/dicom-secure-transfer)
İki cihaz arasında MR görüntülerini **Lorenz kaotik sistemi** ile üretilen
anahtarlar ve **ChaCha20-Poly1305** AEAD ile şifreleyip TLS üzerinden aktaran
PyQt5 istemci-sunucu sistemi. Sunucuda PyTorch CNN ile tümör tespiti; hasta
kimlik etiketleri anonimleştirilir. 21/21 test geçiyor.
`Python` `PyQt5` `Cryptography` `PyTorch` `DICOM`

### 📰 [NodeHaber](https://github.com/muratcihanyandi/nodehabercom) · [nodehaber.com](https://nodehaber.com)
Haber yayın platformu — Next.js + Prisma + PostgreSQL. Tiptap editör, sunucu
tarafı HTML temizleme (XSS), 9 migration'lık şema evrimi, denetim kaydı, n8n
webhook ile otomatik içerik aktarımı, GHCR üzerinden Docker dağıtımı.
`TypeScript` `Next.js` `Prisma` `NextAuth` `Tiptap`

### 🍓 [Ahududu](https://github.com/muratcihanyandi/ahududu)
Kendi kendine barındırılan çift uygulaması — FastAPI + WebSocket + Capacitor
Android + Wear OS. S-Pen basınç hassasiyetli el yazısı, dairesel saat arayüzü,
uzaktan titreşim desenleri, canlı konum/mesafe/pil senkronizasyonu, APK'yı
yeniden kurmadan sunucudan güncellenen arayüz.
`Python` `FastAPI` `React` `Capacitor` `WebSocket`

### 💍 [Wedding Memories](https://github.com/muratcihanyandi/wedding-memories)
Düğün QR fotoğraf/video paylaşım sistemi — FastAPI + React + SQLite/WAL.
1 GB+ videoları RAM'e almadan 1 MB'lık parçalarla diske akıtır, yarıda kesilen
yüklemede geçici dosya bırakmaz, klasörlü streaming ZIP indirme sunar.
Pi 5 + USB disk üzerinde internet olmadan çalışır.
`Python` `FastAPI` `React` `SQLite` `Docker`

### 🌐 [Obsidian Local Web](https://github.com/muratcihanyandi/obsidian-local-web)
Obsidian vault'ını ağdaki herhangi bir tarayıcıdan düzenlemeyi sağlayan tek
dosyalık sunucu. **Sıfır bağımlılık** (Python stdlib), atomik yazma, `.trash`'e
güvenli silme, wikilink/callout/görev listesi desteği, canlı senkron.
`Python` `JavaScript`

---

## Diğer çalışmalar

- **[Windows Dual Audio](https://github.com/muratcihanyandi/windows-dual-audio)** — WASAPI Loopback ile aynı sesi iki çıkışa veren köprü; jitter buffer + gerçek zamanlı resampling ile ana cihazda sıfır kesinti.
- **[Trendyol_Scraper](https://github.com/muratcihanyandi/Trendyol_Scraper)** — Cloudflare arkasındaki DOM'u headless Edge ile okuyup Fakeyol şemasına doğrudan aktarılabilir JSON üreten kazıyıcı; kesintiden devam edebilir.
- **[BalKurye](https://github.com/muratcihanyandi/jetgiller-kurye)** — çok platformlu kurye operasyon paneli; webhook ile sipariş toplama, vardiya, kredi ve Web Push bildirim.
- **[Mira](https://github.com/muratcihanyandi/mira)** — hamile pilatesi/eğitim platformu; danışan, danışman ve admin panelleri + OTA güncellenen Android istemci.
- **[Düğün Davetiyesi](https://github.com/muratcihanyandi/dugun-davetiyesi)** / **[Geri Sayım](https://github.com/muratcihanyandi/dugunekalanzaman)** — WebAudio ile üretilen müzik, 3D zarf animasyonu, canvas yaprak yağmuru; internet gerektirmeyen tek sayfa.

---

## Teknoloji

**Diller** Python · TypeScript · JavaScript · C++ · SQL
**Backend** FastAPI · Express · Next.js Route Handlers · Prisma · SQLAlchemy · PostgreSQL · SQLite
**Frontend** React · Next.js · Tailwind CSS · Vite
**Mobil** React Native / Expo · Capacitor · Wear OS
**Altyapı** Docker (multi-arch ARM64) · CasaOS · GitHub Actions · GHCR · n8n · Cloudflare Tunnel
**Alan** AES/ChaCha20-Poly1305 · JWT · OWASP odaklı girdi doğrulama · Whisper · PyTorch

---

📫 [mcihanyandi@gmail.com](mailto:mcihanyandi@gmail.com)
