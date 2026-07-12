# Discord Bot Doğrulama ve URL Ayarları

## 1. Bu sayfaları nasıl kullanırsın
Bu dizinde iki HTML sayfası oluşturuldu:

- `terms-of-service.html`
- `privacy-policy.html`

Discord doğrulamasında bu dosyaları barındırabileceğin bir HTTPS URL'ye ihtiyacın var.

## 2. En kolay yöntem: GitHub Pages
Eğer bir GitHub hesabın varsa, bu dosyaları bir repo'ya yükleyip GitHub Pages ile yayınlayabilirsin.

1. Yeni bir GitHub deposu oluştur.
2. `terms-of-service.html` ve `privacy-policy.html` dosyalarını repoya ekle ve push et.
3. Repo ayarlarından GitHub Pages'i etkinleştir.
   - Branch: `main` veya kullandığın ana branch
   - Folder: `/root`
4. Yayınlanan URL şu şekilde olur:
   - `https://<kullanici-adi>.github.io/<repo-adi>/terms-of-service.html`
   - `https://<kullanici-adi>.github.io/<repo-adi>/privacy-policy.html`

> GitHub Pages kullanıyorsan URL kesinlikle `https://` ile başlamalıdır.

## 3. Discord geliştirici portalında URL'leri nasıl ayarlarsın
1. Discord Developer Portal'a gir: https://discord.com/developers/applications
2. Bot uygulamanı seç.
3. Sol menüden **General Information** veya **App Information** bölümüne git.
4. `Terms of Service URL` ve `Privacy Policy URL` alanlarına GitHub Pages veya kendi sitesi URL'lerini yapıştır.
5. Kaydet.

## 4. Örnek URL formatları
- `https://<kullanici-adi>.github.io/<repo-adi>/terms-of-service.html`
- `https://<kullanici-adi>.github.io/<repo-adi>/privacy-policy.html`

Eğer kendi alan adın varsa:
- `https://ornek.com/terms-of-service.html`
- `https://ornek.com/privacy-policy.html`

## 5. Bot özellikleri ve neden gerekli oldukları
Bu bot aşağıdaki özellikleri kullanıyor ve bu yüzden gizlilik/kullanım şartları gereklidir:

- Moderasyon komutları: `--ban`, `--kick`, `--clear`, `--warn`, `--unwarn`
- Müzik komutları: `--play`, `--stop`, `--pause`, `--resume`
- Çekiliş komutları: `--çekiliş`, `--çekilişbitir`
- Davet takibi ve komutları: `!davet`, `!davetsayısı`
- Öneri komutu: `--öneri`
- Duyuru komutu: `--duyuru`

Bu bot, kullanıcı kimliklerini, davet bilgilerini ve çekiliş katılımını geçici olarak işler. Bu nedenle `Gizlilik Politikası` gerekli olur.

## 6. Önemli not
`config.mjs` içinde bot token'ı var. Bu dosyayı kesinlikle kimseyle paylaşma ve GitHub'a açık şekilde yükleme.

---

Bu adımları tamamladıktan sonra, Discord Developer Portal'daki `Terms of Service` ve `Privacy Policy` alanlarına yukarıdaki HTTPS URL'leri yapıştırabilirsin.