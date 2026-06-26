# Görsel Promptları (Midjourney, Gemini, DALL·E, Stable Diffusion)

Bu dosyayı, kullanıcının amacı bir görsel/illüstrasyon/tasarım üretmek olduğunda kullan.

## Önemli not: dil

Görsel araçları (özellikle Midjourney ve Stable Diffusion) İngilizce promptlarda belirgin şekilde daha iyi çalışır. Bu yüzden bu alanda profesyonel ve ultra-detaylı katmanları **İngilizce** ver, ama yanında Türkçe kısa bir açıklama bırak ki kullanıcı ne yazdığını anlasın. Kısa promptu Türkçe verebilirsin.

## Mutlaka düşünülmesi gereken katmanlar

- **Konu (subject):** Ne çiziliyor — net ve spesifik.
- **Stil:** Fotoğraf mı, dijital sanat mı, 3D render mı, yağlı boya mı, anime mi? Varsa sanatçı yerine *tarz* tarif et (telif açısından daha güvenli).
- **Kompozisyon:** Yakın çekim mi, geniş açı mı; özne nerede; arka plan ne?
- **Işık:** Altın saat, stüdyo ışığı, neon, sinematik karanlık vb.
- **Renk paleti:** Sıcak/soğuk, pastel, yüksek kontrast.
- **Kamera/lens (foto-gerçekçi için):** 35mm, 85mm portre, geniş açı, alan derinliği.
- **Ruh hali (mood):** Huzurlu, gizemli, epik, melankolik.
- **Teknik:** En-boy oranı (aspect ratio), çözünürlük/detay seviyesi.
- **Negatif prompt:** İstenmeyen şeyler (bozuk eller, fazla parmak, bulanıklık, metin, logo).

## Araç-özel ipuçları

- **Midjourney:** Promptun başına `/imagine prompt:`, sonuna parametreler: `--ar 16:9`, `--style raw`, `--v 6` gibi. Virgülle ayrılmış öbekler iyi çalışır.
- **Stable Diffusion:** Pozitif ve negatif prompt ayrı alanlarda. Ağırlıklandırma (token:1.3) kullanılabilir.
- **Gemini / DALL·E:** Daha doğal, cümle bazlı tarif sever; parametre yerine açık dille anlat.

İlgili araç belliyse o aracın formatına göre yaz; belli değilse Midjourney + doğal dil olmak üzere iki sürüm vermeyi düşün.

## Ultra-detaylı katmanda ekle

Tam İngilizce prompt + ayrı negatif prompt + en-boy oranı + stil parametreleri + 2-3 varyasyon önerisi (örneğin aynı sahnenin farklı ışık/açı versiyonları).

## Teslim notu için

Hangi araca yapıştırılacağını ve parametrelerin nereye geleceğini belirt.

## Üretim araçları (örnek)

Ultra katmanın sonuna kısa bir araç notu ekle, "örnek/değişebilir" diyerek:

> Üretim araçları (örnek): üretim → Midjourney, Flux, Leonardo veya Gemini/DALL·E; ücretsiz/açık kaynak → Stable Diffusion; büyütme (upscale) ve rötuş → Magnific veya Photoshop. (Örnektir, kendi tercihini kullanabilirsin.)
