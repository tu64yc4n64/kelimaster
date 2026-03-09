# App Store Connect – Review Öncesi Kontrol Listesi

Bu liste, "Unable to Add for Review" uyarısındaki maddeleri tek tek nasıl tamamlayacağınızı özetler.

---

## 1. Privacy Policy URL (Gizlilik Politikası)

- **Nerede:** App Store Connect → Uygulamanız → **App Privacy** (veya App Information içinde Privacy Policy URL alanı).
- **Ne yapın:** Gizlilik politikası sayfasının adresini girin.
- **URL:** Repoyu push edip GitHub Pages’i açtıktan sonra:
  - `https://cantugay.github.io/kelimaster/privacy-policy`
  - veya repo farklı bir kullanıcıda (örn. tu64yc4n64) ise: `https://tu64yc4n64.github.io/kelimaster/privacy-policy`

**GitHub Pages’i açmak için:**
1. Bu projedeki `docs` klasörünü push edin.
2. GitHub’da repo → **Settings** → **Pages**.
3. **Source:** Deploy from a branch.
4. **Branch:** main (veya default branch), **Folder:** /docs → Save.
5. Birkaç dakika sonra yukarıdaki URL’den sayfa açılır.

---

## 2. Primary Category (Birincil Kategori)

- **Nerede:** App Store Connect → Uygulamanız → **App Information** (veya Genel Bilgiler).
- **Ne yapın:** **Primary Category** alanından bir kategori seçin (örn. **Games** veya **Word**).

---

## 3. Content Rights (İçerik Hakları)

- **Nerede:** App Store Connect → Uygulamanız → **App Information** → **Content Rights**.
- **Ne yapın:** Uygulama içeriğinin (metin, görsel, ses vb.) size ait veya kullanım izniniz olduğunu belirleyin. Gerekirse “I have all necessary rights to this content” benzeri onay kutusunu işaretleyin veya açıklama girin.

---

## 4. App Privacy & Tracking (NSUserTrackingUsageDescription)

Uygulama **NSUserTrackingUsageDescription** kullandığı için Apple, “tracking” ile toplanan verileri App Privacy’de bildirmenizi istiyor.

**İki seçenek:**

**A) ATT ile reklam/tracking kullanıyorsanız (önerilen):**
- **Nerede:** App Store Connect → Uygulamanız → **App Privacy**.
- **Ne yapın:** “Data Used to Track You” bölümüne gidin; reklam kimliği, kullanım verisi vb. için “Used for Tracking Purposes” işaretleyin. AdMob için genelde **Identifiers** (Advertising Data) ve gerekirse **Usage Data** işaretlenir.

**B) Tracking yapmayacaksanız:**
- Info.plist’ten **NSUserTrackingUsageDescription** anahtarını kaldırın (veya ATT izni istemeyen bir build yükleyin).
- Yeni build yükleyip tekrar deneyin.

---

## 5. Price Tier (Fiyat)

- **Nerede:** App Store Connect → Uygulamanız → **Pricing and Availability** (veya **App Pricing**).
- **Ne yapın:** **Price** alanından bir fiyat seçin. Ücretsiz ise **Free** (0,00) seçin.

---

## Özet

| Madde | Nerede | Eylem |
|-------|--------|--------|
| Privacy Policy URL | App Privacy / App Information | `https://...github.io/kelimaster/privacy-policy` gir |
| Primary Category | App Information | Games / Word vb. seç |
| Content Rights | App Information → Content Rights | Hakları onayla / formu doldur |
| Tracking / App Privacy | App Privacy | Tracking verilerini işaretle veya ATT’yi kaldır |
| Price | Pricing and Availability | Free veya ücretli tier seç |

Hepsini tamamladıktan sonra **Add for Review** / **Submit for Review** tekrar aktif olur.
