# EVE GİDİNCE: KULLANICI ADIMLARI (sade, numaralı)

Bu rehber, gerçek verinle ilk denemeyi yapman içindir. Hedef: ürünün en büyük açığını (içe aktarıcılar gerçek dosyalarla hiç denenmedi) kapatmak ve "Claude beni tanıyor mu?" testini gerçek veriyle yapmak.

**Dürüst uyarı:** Üçüncü taraf menü adları (Google, Reddit, ChatGPT, Claude, DeepSeek, Gemini) bu ortamdan doğrulanamadı; aşağıda menü adı UYDURMUYORUM. Ekranda farklı gördüğünde ya da bir şey bulamadığında, ekrandaki yazıları bana yaz. Sorun çıkarsa her zaman önce "Hata raporunu kopyala" düğmesi.

## A. Kurulum (Windows)
1. GitHub'da depoya gir, sağda **Releases** bölümünden **en son ön sürümü** (v0.1.1 ya da daha yenisi) aç.
2. `KimlikMerkezi-Kurulum-...exe` dosyasını indir.
3. (İstersen) bütünlüğü kontrol et: indirme klasöründe PowerShell aç, `Get-FileHash .\KimlikMerkezi-Kurulum-....exe` yaz; çıkan SHA256 değeri, sürümdeki `SHA256SUMS.txt` ile aynı olmalı.
4. Dosyaya çift tıkla. "Windows bilgisayarınızı korudu" çıkarsa (imzasız olduğu için):
   - **"Ek bilgi"** (More info) bağlantısına tıkla, sonra **"Yine de çalıştır"** (Run anyway).
   - Düğmeyi göremezsen dur ve bana yaz (Windows 11 Akıllı Uygulama Denetimi açıksa çıkmayabilir).
5. Kurulum yönetici izni istemez. Bitince uygulamayı aç; **ilk açılış sihirbazı** veri klasörünü sorar.
6. **Şifreleme varsayılan olarak AÇIK** gelir (Windows hesabına bağlı, parolasız). Parola eklemek istersen uygulamadaki **Güvenlik** sayfasından eklenir. Parola eklerken önce bir **kurtarma ifadesi** kurman istenir. Hem parolayı hem kurtarma ifadesini unutursan verin KURTARILAMAZ. İfadeyi bir kâğıda yaz ve güvenli bir yerde sakla. (Parola eklemek zorunlu değil.)
7. Hata çıkarsa uygulamada **"Hata raporunu kopyala"** düğmesine bas, metni bana yapıştır.

## B. Veri arşivlerini iste (hazır olması saatler-günler sürer, önce bunu başlat)
Menü adlarını ben bilmiyorum; aşağıdakiler yön gösterir. Bulamazsan ekran yazısını bana ilet.
1. **Google Takeout** (takeout.google.com): önce tüm seçimleri kaldır; YouTube ve YouTube Music, Chrome, "Etkinliklerim" (My Activity), konum geçmişi (varsa), Gmail (isteğe bağlı) seç. Geçmiş verilerinde **JSON** biçimini seç (HTML değil). Hazır olunca e-postayla gelen bağlantıdan zip'i indir. Gemini etkinliği için "Etkinliklerim" kapsamında bak.
2. **Reddit:** tarayıcıda `reddit.com/settings/data-request` adresine git, hesap geçmişi için istek gönder. Zip gelince indir.
3. **ChatGPT, Claude, DeepSeek:** her birinin ayarlar bölümünde veri dışa aktarma / indirme seçeneği aranır; adı değişebilir. Bulduğunda e-postayla gelen bağlantıdan zip'i indir. Bulamazsan bana o uygulamanın ayarlar ekranındaki başlıkları yaz.
4. **Instagram/Facebook (Meta), GitHub, Spotify:** her birinin "verilerimi indir" bölümünden iste; JSON biçimi tercih et. Bekleme süresi uzun olabilir.
5. Hepsi aynı anda gelmek zorunda değil. Gelen zip'i **açma**, olduğu gibi kullan.

## C. İçe aktarma (her zip için)
1. Uygulamada **İçe aktar** ekranını aç, zip'i seç.
2. Ekranda **biçim raporu** görünür (dosya adları ve alan adları, kişisel içerik yok). Başarılıysa kaç kayıt eklendiği yazar.
3. **Bir şey ters giderse** (dosya tanınmadı, hata, 0 kayıt, ya da "bozuk"): biçim raporunu ve hata metnini kopyalayıp bana yapıştır. Bu, içe aktarıcıyı gerçeğe göre düzeltmem için en değerli veri. İçerik değil yalnız yapı içerir.
4. Gerçek dosyada ilk kez deneme olduğu için ilk içe aktarmalarda hata çıkması NORMAL. Bu testin amacı bu.
5. Kaynaklar sayfasında ve Harita'da kayıtların göründüğünü kontrol et.

## D. Claude ile "beni tanıyor mu?" testi (MCP)
1. **Erişim** ekranından **"Claude'a ekle"** düğmesine bas. Sonuç kutusu başarılı ya da başarısız olduğunu açıkça söyler; başarısızsa aranan dosya yollarını gösterir.
2. **Dikkat:** "Claude'a ekle", **hassas olmayan 10 kategoriyi süresiz AÇIK** verir. E-posta, mesaj, konum ve sohbet kapalı kalır; onları açmak için ayrı onay istenir. Daha dar bir yetki istersen "Yeni anahtar" ile hiçbir izin vermeden başlayıp Erişim ekranından tek tek açabilirsin.
3. Claude Desktop'u tamamen kapatıp yeniden aç.
4. Yeni sohbette önce: "kategorilerimi listele". Sonuç gelmezse bana yaz.
5. Sonra kendi sorularını sor. Önerilen kısa test (hafızasız ve hafızalı karşılaştır):
   - Önce **hafızasız** bir sohbette (MCP kapalıyken ya da başka bir yapay zekâda) 5–6 şey sor: "Ben hangi şehirde yaşıyorum?", "Kod yazarken hangi dili ve editörü kullanıyorum?", "Son zamanlarda hangi konulara ilgi duyuyorum?", "Hangi müzikleri dinlerim?", "Günün hangi saatlerinde çalışırım?"
   - Aynı soruları **MCP açıkken** sor. Cevapları yan yana koy.
   - Yanlış, uydurma ya da hiç bilmediği şeyler olursa bana yaz: hangi soru, ne dedi, gerçek ne. Bu, kimlik kartı ve aramanın gerçek veriyle ne kadar iyi olduğunu gösteren en önemli kanıt.
6. Ayrıca bir hassas kategori kapalıyken (örn. e-posta) o kategoriye ait bir şey sor: **cevap vermemeli**, "izin yok" demeli. Verirse ciddi bir hata, hemen bana yaz.
7. **Persona önerileri:** Claude sana `persona_oner` ile çıkarım önerebilir; bunlar **Persona > Öneriler** sekmesinde bekler. Kendin onayla, düzelt ya da reddet. Onaylamadıkça hiçbir şey kalıcı olmaz.

## E. Telefon ve diğer cihazlar
Android toplayıcı henüz yok (sonraki sürüm). Şimdilik telefondaki verileri yukarıdaki arşivlerle (Google, Meta, Spotify...) getiriyoruz.

## F. Bana ne getireceksin (özet)
1. Her içe aktarma için: başarılı mı, kaç kayıt, hata/biçim raporu.
2. Kurulum ya da açılışta yaşadığın her takılma (ekran yazısıyla).
3. "Beni tanıyor mu?" testinin yan yana cevapları.
4. Hassas kategori kapalıyken sızıntı olup olmadığı.

## G. Bekleyen sorular
1. DeepSeek masaüstü uygulamasının tam adı nedir?
2. Redmi Note 10 Pro ve Galaxy Tab A9 Plus Android sürümü (sonraki sürüm için).
3. İzin varsayılanı: "Claude'a ekle" 10 hassas olmayan kategoriyi açık versin mi (şu an böyle) yoksa hiçbirini açmasın mı?
4. Varsayılan tema koyu kalsın mı?
