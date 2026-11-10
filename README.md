# Murat Can Cihanyandı

Full-stack geliştirici · Python & TypeScript · Kendi kendine barındırılan üretim sistemleri

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](#)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](#)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](#)
[![Next.js](https://img.shields.io/badge/Next.js-000000?logo=next.js&logoColor=white)](#)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](#)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](#)

---

Yazılımı **çalışan sistemler** olarak görüyorum. Buradaki üç proje Raspberry Pi 5
üzerinde 7/24 çalışıyor; ikisi canlıda gerçek kullanıcıya hizmet ediyor.

Odaklandığım üç konu:

- **Uçtan uca ürün** — sepet/sipariş/ödeme akışı, yönetim ve satıcı panelleri, kargo
  takibi; iş kuralları istemci ve sunucuda tek kaynaktan yönetilir.
- **Kısıtlı donanımda üretim** — ARM64 multi-arch imajlar, düşük RAM'de çalışan
  servisler, tek konteyner dağıtımı.
- **Veri güvenliği** — kaotik sistem tabanlı anahtar üretimi ve ChaCha20-Poly1305 ile
  şifrelenmiş tıbbi görüntü aktarımı, kimlik doğrulama sertleştirme, girdi doğrulama.

---

## Projeler

### [Fakeyol](https://github.com/muratcihanyandi/fakeyol) · [fakeyol.com](https://fakeyol.com)

Tam yığın e-ticaret platformu — Next.js 15 + Express + PostgreSQL.
**58 API ucu**, 15 sayfa, 11 Prisma modeli. Kargo ve kupon kuralları istemci ile
sunucuda tek kaynaktan yönetilir, böylece gösterilen tutar ile hesaplanan tutar
ayrışamaz. Sipariş yaşam döngüsü 7 aşamalı bir durum makinesiyle yürür; kurye rotası
ve sipariş akışı simülasyon motoruyla canlı üretilir. Kimlik doğrulama zayıf
anahtarlarla başlamayı reddeder, giriş ve yazma uçlarında hız sınırlama vardır.
AMD64 + ARM64 multi-arch imaj ile Raspberry Pi 5 üzerinde üretimde.

`TypeScript` `Next.js` `Express` `Prisma` `PostgreSQL` `Docker`

### [AutoShorts Studio v2](https://github.com/muratcihanyandi/autoshorts-studio-v2) · [ass.fakeyol.com](https://ass.fakeyol.com)

Yayın platformlarından otomatik dikey klip (Shorts / Reels / TikTok) üreten ve
yayınlayan otonom stüdyo. FastAPI backend, React web arayüzü ve React Native mobil
istemci tek üründe birleşir; Whisper ile transkripsiyon, LLM ile klip seçimi, kuyruk
yönetimi ve 7 adımlı kurulum sihirbazı içerir. Yaklaşık 160 commit'lik aktif bir
kod tabanı.

`Python` `FastAPI` `React` `React Native` `FFmpeg` `Whisper`

### [DICOM Secure Transfer](https://github.com/muratcihanyandi/dicom-secure-transfer)

İki cihaz arasında MR görüntülerini uçtan uca şifreleyerek aktaran PyQt5
istemci–sunucu sistemi. Anahtarlar Lorenz kaotik sistemi çıktısının donanım
entropisiyle karıştırılıp HKDF ile türetilir; piksel verisi ChaCha20-Poly1305 AEAD ile
şifrelenir, aktarım TLS 1.2+ üzerinden yürür ve hasta kimlik etiketleri anonimleştirilir.
Sunucu tarafında PyTorch CNN ile tümör tespiti yapılır; 21/21 test geçmektedir.

`Python` `PyQt5` `Cryptography` `PyTorch` `DICOM` `TLS`

---

## Teknoloji

**Diller** Python · TypeScript · JavaScript · C++ · SQL
**Backend** FastAPI · Express · Next.js Route Handlers · Prisma · SQLAlchemy · PostgreSQL
**Frontend** React · Next.js · Tailwind CSS
**Mobil** React Native / Expo · Capacitor
**Altyapı** Docker (multi-arch ARM64) · GitHub Actions · GHCR · n8n · Cloudflare Tunnel
**Güvenlik** ChaCha20-Poly1305 AEAD · TLS · JWT sertleştirme · girdi doğrulama

---

📫 [mcihanyandi@gmail.com](mailto:mcihanyandi@gmail.com)
