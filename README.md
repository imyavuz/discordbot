# imyavuzBot GitHub Pages

Bu proje için oluşturulan HTML dosyaları:

- `terms-of-service.html`
- `privacy-policy.html`

GitHub Pages ile bu dosyaları yayınlamak istiyorsan aşağıdaki adımları kullan:

1. GitHub'da yeni bir repository oluştur.
2. Bu projeyi GitHub'a it:
   ```bash
   git remote add origin https://github.com/<kullanici-adi>/<repo-adi>.git
   git branch -M main
   git push -u origin main
   ```
3. GitHub repository ayarlarından `Pages` bölümünü aç.
4. `Branch` olarak `main`, `Folder` olarak `/root` seç.
5. Sayfa yayınlandığında şu URL'leri kullanabilirsin:
   - `https://<kullanici-adi>.github.io/<repo-adi>/terms-of-service.html`
   - `https://<kullanici-adi>.github.io/<repo-adi>/privacy-policy.html`

> `config.mjs` dosyasındaki token, güvenlik nedeniyle `.gitignore` içine alındı ve GitHub'a gönderilmemelidir.
