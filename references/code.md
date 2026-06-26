# Kod & Proje Promptları (Claude Code, VS Code, uygulama geliştirme)

Bu dosyayı, kullanıcının amacı çalışan kod, bir özellik veya bir yazılım projesi ürettirmek olduğunda kullan.

## Mutlaka düşünülmesi gereken katmanlar

İyi bir kod promptu, AI'ın tahmin yapmasını en aza indirir:

- **Hedef:** Ne yapılacak, tek net cümleyle. ("X yapan bir Y oluştur.")
- **Teknoloji yığını:** Dil, framework, kütüphaneler. Belirtilmediyse makul bir varsayım yap ve belirt.
- **Girdi/çıktı:** Fonksiyon/uygulama ne alacak, ne döndürecek.
- **Dosya yapısı:** Hangi dosyalar oluşacak, nasıl organize edilecek. Çok dosyalı projelerde bu kritik.
- **Görev sırası:** Adım adım ne yapılacağı. AI'a "önce şunu, sonra şunu" demek dağınık tek-blok istekten çok daha iyi sonuç verir.
- **Kısıtlar:** Performans, basitlik, harici bağımlılık olmaması gibi sınırlar.
- **Hata kontrolü / edge case:** Boş girdi, hatalı veri, sınır durumları nasıl ele alınacak.
- **Kabul kriteri:** "Bittiğini" nasıl anlayacağız — ne çalışmalı, hangi test geçmeli.

## Claude Code'a özel

Claude Code dosya sistemiyle çalışır, o yüzden promptta net dosya yolları ve adımlar vermek işe yarar. Büyük bir işi tek seferde istemek yerine, görevi sıralı parçalara bölmek ve "her adımdan sonra dur ve göster" demek daha kontrollü ilerletir. Mevcut bir kod tabanında çalışılıyorsa, AI'a önce ilgili dosyaları okumasını söyle.

## Ultra-detaylı katmanda ekle

Tam teknik şartname: stack + dosya ağacı + adım adım görev listesi + her dosyanın sorumluluğu + hata senaryoları + test/kabul kriterleri + (varsa) örnek girdi-çıktı.

## Teslim notu için

Promptu Claude Code'a mı yoksa normal sohbete mi vermenin daha iyi olacağını belirt. Çok dosyalı/projeyse Claude Code, tek fonksiyon/açıklamaysa sohbet yeterli olur.

## Üretim/çalıştırma araçları (örnek)

Gerekiyorsa kısa bir not ekle:

> Çalıştırma/test (örnek): kod yazımı → Claude Code veya sohbet; düzenleme → VS Code/Cursor; hızlı deneme → Replit veya yerel terminal. (Örnektir.)
