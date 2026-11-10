# KULLANICI ADIMLARI (sade, numaralı)

Menü adları resmî Microsoft/Google/Reddit sayfalarından doğrulanamadı (bu ortamdan açılmadı); aşağıdakiler üçüncü taraf kaynaklara dayanır. Ekranda farklı görürsen bana ekran yazısını yapıştır.

## A. v0.1.0 kurulumu (Windows)
1. GitHub'da depoya gir, sağda "Releases" bölümünden `v0.1.0` (ön sürüm) sürümünü aç.
2. `KimlikMerkezi-Kurulum-v0.1.0.exe` dosyasını indir.
3. Dosyaya çift tıkla. "Windows bilgisayarınızı korudu" yazan mavi bir pencere çıkabilir (dosya imzasız olduğu için):
   - Pencerede **"Ek bilgi"** (İngilizce: "More info") bağlantısına tıkla.
   - Çıkan **"Yine de çalıştır"** (İngilizce: "Run anyway") düğmesine tıkla.
   - Bu düğmeyi göremezsen dur ve bana yaz. Windows 11'deki "Akıllı Uygulama Denetimi" açıksa düğme hiç çıkmayabilir.
4. Kurulum yönetici izni istemez. Bitince uygulamayı aç; ilk açılış sihirbazı veri klasörünü sorar.
5. Hata çıkarsa uygulamada **"Hata raporunu kopyala"** düğmesine bas ve metni bana yapıştır.
6. İstersen indirdiğin dosyanın bütünlüğünü kontrol et: `SHA256SUMS.txt` içindeki değerle eşleşmeli (İstersen adımlarını yazarım).

## B. Veri arşivlerini iste (hazır olması saatler-günler sürer)
1. **Google Takeout** (takeout.google.com): önce "Hepsinin seçimini kaldır" de; YouTube ve YouTube Music, Chrome ve "Etkinliklerim" (My Activity) seç. Geçmiş verisi için **biçimi HTML yerine JSON** yap ("Birden çok biçim"/"Multiple formats" altında). Dışa aktarmayı oluştur, e-postayla gelen bağlantıdan zip'i indir. Menü adları doğrulanmadı.
2. **Reddit:** tarayıcıda reddit.com/settings/data-request adresini aç, tüm hesap geçmişi için istek gönder. Hazır olunca mesajla bağlantı gelir; zip'i indir. Aynı anda 30 günde bir istek yapılabilir (üçüncü taraf kaynak).
3. Arşivler gelince uygulamada **İçe aktar** ekranından zip'i seç (açma). Çıkan **biçim raporunu** kopyalayıp bana yapıştır (içerik yok, yalnız dosya ve alan adları).

## C. MCP bağlantısı
1. Uygulamada **Erişim** ekranından "Claude'a ekle" düğmesine bas.
2. Claude Desktop'u kapatıp yeniden aç.
3. Bir sohbette "kategorilerimi listele" de; sonuç gelmezse bana yaz.
4. Başta hiçbir kategori açık değildir; Erişim ekranından hangisini istersen açarsın. E-posta, mesaj ve konum için ek onay çıkar.
5. DeepSeek uygulaması için önce uygulamanın tam adını yaz (henüz sorulmadı: bkz. aşağıda).

## D. Bekleyen sorular
1. DeepSeek masaüstü uygulamasının tam adı nedir?
2. Redmi Note 10 Pro ve Galaxy Tab A9 Plus Android sürümü (v0.2.0 için).
3. Karar B/C seçimi: geçici olarak web+tepsi ve resmî `mcp` varsayıldı; başka istersen yaz.
