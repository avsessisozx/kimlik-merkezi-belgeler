# DURUM

## Devam noktası
YOL-HARITASI.md sırası geçerli. main'de: çekirdek (sohbet kategorisi, şema v3), 12 içe aktarıcı (sohbet dahil, hepsi doğrulanmadı), Harita veri katmanı + drill-down API + persona öneri kuyruğu (İ2 bitti). Kırmızı (main): entegrasyon test_icealdan_kimlik_kartina ve windows test_mcp_stdio...(7 araç) → İ5'e verildi. Çalışan: İ5 (1) 2 test düzeltme + Öneri inceleme ekranı, (2) Harita görsel tasarım yenilemesi (HUD, ECharts, zengin demo veri, drill-down/çapraz filtre). Sıradaki: İ2/İ3 boşta → ses/görüntü içe aktarıcıları (yerel whisper+OCR), izlenen klasörler (sürekli güncel), Claude gerçek bağlantı adımları KULLANICI_ADIMLARI'na, sohbet dışa aktarma adımları (ChatGPT/Claude/DeepSeek/Gemini), v0.1.1 ön sürüm, Karar A + Android.

## Yapıldı
- Özel depo avsessisozx/kimlik-merkezi bağlandı; main'e kök dosyalar ve INTERFACES.md v1 itildi.

## Kaldı
Aşama 1-8 (v0.1.0), sonra Karar A + v0.2.0.

## Bilinen hatalar / notlar
- LICENSE: kişisel kullanım için "tüm hakları saklıdır" metni konuldu (kullanıcı değiştirebilir).
- `gh auth status` GH_TOKEN'ı geçersiz gösteriyor, ama REST (gh api) çalışıyor. Repo oluşturma otomatik izin denetiminde reddedildi; kullanıcı depoyu elle açtı.

## Doğrulandı / doğrulanmadı
Doğrulandı (CI, 2026-11-10): ci (ubuntu, py3.12/3.13), tam (windows-latest + 2 GiB büyük test), paket (PyInstaller+Inno sessiz kurulum, açılış, sağlık, MCP stdio, kaldırma, Claude'a ekle sahte ayarla). Yerel: core 60, server 41, importers 35, entegrasyon 3, windows 23.
Doğrulanmadı: gerçek Takeout/Reddit dosyaları; Türkçe Takeout adları; Reddit sütunları; Claude Desktop gerçek ayar yolu; DeepSeek MCP; Windows 10 (runner Server 2025); SmartScreen; tepsi simgesinin ekranda görünmesi; gerçek tarayıcıda görsel kontrol; modelin enjeksiyona kanmaması.

## Müdüre istekler
(yok)

## Kullanıcıdan bekleyen cevaplar
DeepSeek uygulama adı; Redmi Note 10 Pro ve Galaxy Tab A9 Plus Android sürümü; Claude Code otomatik onay adımları.
