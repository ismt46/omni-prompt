# Otomasyon & AI Agent Promptları (n8n, iş akışları, agent tasarımı)

Bu dosyayı, kullanıcının amacı bir otomasyon akışı, bir iş akışı tasarımı veya bir AI agent kurmak olduğunda kullan.

## İki farklı durumu ayır

1. **Akış tasarımı promptu:** Kullanıcı "şunu otomatikleştirmek istiyorum" diyor. Burada AI'a akışı tasarlatıyorsun — hangi tetikleyici, hangi adımlar, hangi araçlar.
2. **Agent sistem promptu:** Kullanıcı bir AI agent'a kişilik/görev tanımı yazmak istiyor. Burada agent'ın rolünü, sınırlarını ve davranışını yazıyorsun.

Konudan hangisi olduğunu sez; emin değilsen ikisini de kısaca ele al.

## Akış tasarımı için katmanlar

- **Tetikleyici (trigger):** Akışı ne başlatır — yeni e-posta, form, zamanlayıcı, webhook?
- **Adımlar:** Sırayla ne olacak. Her adımda hangi servis/araç devreye girer.
- **Veri akışı:** Bir adımdan diğerine ne taşınıyor.
- **Koşullar / dallanma:** "Eğer şu olursa şunu yap" mantığı.
- **Hata yönetimi:** Bir adım başarısız olursa ne olacak.
- **Kullanılan servisler:** Gmail, Sheets, Slack, OpenAI node vb.

## Agent sistem promptu için katmanlar

- **Rol ve amaç:** Agent kim, ne için var.
- **Yetenekler ve araçlar:** Neye erişebilir, ne yapabilir.
- **Sınırlar:** Ne yapmamalı, ne zaman insana devretmeli.
- **Ton ve çıktı formatı:** Nasıl konuşmalı, nasıl yanıt vermeli.
- **Adım adım mantık:** Bir görevi nasıl ele almalı.

## Ultra-detaylı katmanda ekle

Akış için: node-by-node tam akış (tetikleyici → her adım → koşullar → hata dalı) + her node'da hangi servisin ne yaptığı + örnek veri.
Agent için: tam sistem promptu (rol + araçlar + sınırlar + ton + örnek diyaloglar).

## Teslim notu için

n8n akışıysa, bunu doğrudan n8n'e koyamayacağını ama node node kurması için rehber olduğunu belirt. Agent promptuysa, hangi platformun sistem promptu alanına yapıştırılacağını söyle.

## Üretim araçları (örnek)

> Kurulum (örnek): görsel iş akışı → n8n veya Make; agent kurulumu → kullandığın LLM platformunun sistem promptu alanı. (Örnektir.)

## Hazır agent iskeleti

Kullanıcı bir AI agent sistem promptu istediğinde, ultra katmanda bu iskeleti onun konusuna göre doldurarak ver. Bu, kullanıcıya hazır bir başlangıç noktası sunar; her alanı konuya göre özelleştir, boş bırakma:

```
# Rol
Sen [agent'ın kim olduğu, tek cümle]. Amacın [ne için var].

# Yetenekler ve araçlar
- [erişebildiği araç/veri 1]
- [erişebildiği araç/veri 2]

# Çalışma mantığı
Bir görev geldiğinde sırayla:
1. [ilk adım]
2. [ikinci adım]
3. [sonuç/çıktı]

# Sınırlar
- [yapmaması gereken şey]
- Emin olmadığında [insana devret / soru sor].

# Ton ve format
[nasıl konuşmalı] + [çıktıyı hangi formatta vermeli].
```

İskeleti olduğu gibi köşeli parantezlerle bırakma — kullanıcının konusuna göre her kısmı gerçek içerikle doldur, sonra "istersen şu kısımları kendine göre değiştir" diye kısa bir not düş.
