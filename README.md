# J.A.R.V.I.S — Android

Koyu teal / cyan Iron Man tarzı arayüz + Gemini Live sesli sohbet.

---

## Bilgisayar olmadan APK alma (GitHub Actions)

### 1. GitHub hesabı aç
Telefondan: https://github.com → Sign up

### 2. Yeni repo oluştur
1. Sağ üstte **+** → **New repository**
2. Repository name: `JarvisAndroid` (istediğin isim)
3. **Public** seç
4. **Create repository**

### 3. Dosyaları yükle
1. Bu `JarvisAndroid` klasörünün **içindeki tüm dosyaları** GitHub’a yükle.
2. Telefondan:
   - Repoya gir → **uploading an existing file** (veya Add file)
   - Tüm dosya ve klasörleri seç (özellikle **.github** klasörü de gelsin)
   - **Commit changes**

### 4. Otomatik derleme
- **Actions** sekmesine gir
- **Build APK** işinin yeşil tik almasını bekle (3–8 dk)
- İş bitince:
  - İşin üzerine tıkla
  - En altta **Artifacts** → **Jarvis-APK** indir
  - Zip içinden `app-debug.apk` çıkar

### 5. Telefona yükle
- `app-debug.apk` dosyasını aç → Yükle
- İlk açılışta Gemini API anahtarını gir (bir kere)
- Sonraki açılışlarda sormaz

---

## Gemini API anahtarı (ücretsiz)

https://aistudio.google.com/apikey  
→ Create API key → kopyala → uygulamaya yapıştır

---

## Elle tekrar derlemek

GitHub → **Actions** → **Build APK** → **Run workflow**

---

## Notlar

- Model adı değişirse: `GeminiLiveClient.kt` içindeki `MODEL` satırını güncelle
- Artifact 14 gün saklanır
