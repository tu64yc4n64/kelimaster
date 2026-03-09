# Privacy Policy URL – Ne Yapmalı?

Gizlilik metni zaten hazır (`docs/privacy-policy/index.html`). Şimdi bunu internette açıp App Store Connect’e URL’i vermeniz yeterli.

---

## Adım 1: Kodu GitHub’a gönderin

Terminalde proje klasöründeyken:

```bash
cd /Users/cantugay/kelimaster
git add docs/
git commit -m "Gizlilik politikası sayfası eklendi"
git push origin main
```

(Eğer branch adınız `main` değilse `git branch` ile kontrol edin; `master` ise `git push origin master` yazın.)

---

## Adım 2: GitHub’da Pages’i açın

1. Tarayıcıda **https://github.com** → giriş yapın.
2. **kelimaster** reponuza gidin (URL: `https://github.com/KULLANICI_ADINIZ/kelimaster`).
3. Üst menüden **Settings** (Ayarlar) tıklayın.
4. Sol menüden **Pages** seçin.
5. **Build and deployment** altında:
   - **Source:** "Deploy from a branch" seçin.
   - **Branch:** "main" (veya varsayılan branch), **Folder:** "**/docs**" seçin.
   - **Save** deyin.

---

## Adım 3: Birkaç dakika bekleyin

GitHub sayfayı yayınlar (genelde 1–2 dakika). Hazır olunca şu adres çalışır:

- **https://KULLANICI_ADINIZ.github.io/kelimaster/privacy-policy**

(Örneğin kullanıcı adınız `cantugay` ise: **https://cantugay.github.io/kelimaster/privacy-policy**)

Tarayıcıda bu adresi açıp “Gizlilik Politikası” sayfasını gördüğünüzden emin olun.

---

## Adım 4: Bu URL’i App Store Connect’e girin

1. **App Store Connect** → https://appstoreconnect.apple.com
2. Uygulamanızı seçin (**Kelimaster**).
3. **App Privacy** veya **App Information** bölümüne gidin.
4. **Privacy Policy URL** (Gizlilik Politikası URL’i) alanına yapıştırın:
   - `https://KULLANICI_ADINIZ.github.io/kelimaster/privacy-policy`

Kaydedin. Bu madde tamamlanmış olur.

---

## Özet

| # | Ne yaptınız |
|---|-------------|
| 1 | `docs` klasörünü GitHub’a push ettiniz |
| 2 | Repo → Settings → Pages → Source: branch, Folder: **/docs** → Save |
| 3 | Birkaç dakika sonra sayfayı tarayıcıda kontrol ettiniz |
| 4 | Aynı URL’i App Store Connect → Privacy Policy URL alanına yazdınız |

Takıldığınız adımı yazarsanız, o adımı birlikte netleştirebiliriz.
