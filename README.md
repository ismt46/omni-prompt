# Omni-Prompt 🎯

> A Claude Skill that turns a one-line idea into professional, platform-aware AI prompts.
> (Kullanıcının verdiği basit bir fikri, profesyonel ve üretime hazır AI promptlarına dönüştüren bir Claude Skill'i.)

Bir konu yaz, Omni-Prompt onu **üç katmanlı** profesyonel bir prompta çevirsin: kısa, profesyonel ve ultra-detaylı. Hangi araca (video, görsel, kod, otomasyon) gideceğini sezer, o alanın kurallarını uygular ve promptun nasıl kullanılacağını söyler.

---

## Ne yapar?

Tek satırlık dağınık bir fikir verirsin (ör. *"kara deliğe düşersen ne olur konulu uzay shorts'u"*), Omni-Prompt sana şunu döner:

- **Analiz** — konunun amacı + sezilen platform
- **Kısa prompt** — hızlı denemek için öz hali
- **Profesyonel prompt** — önerilen, dengeli sürüm
- **Ultra-detaylı üretim promptu** — tüm teknik parametrelerle tam sürüm
- **Nasıl kullanılır** — promptu hangi araca nasıl vereceğin

### Desteklenen alanlar

| Alan | Örnek araçlar |
|------|---------------|
| 🎬 Video (YouTube, Shorts, Reels, TikTok) | senaryo + hook + retention yapısı |
| 🎨 Görsel (Midjourney, Gemini, DALL·E, SD) | kamera, ışık, kompozisyon, negatif prompt |
| 💻 Kod / Proje (Claude Code, VS Code) | hedef, dosya yapısı, görev sırası, hata kontrolü |
| ⚙️ Otomasyon / AI Agent (n8n, Make) | akış tasarımı + hazır agent iskeleti |

---

## Kurulum

### Claude.ai / Claude uygulaması (web & masaüstü)

1. **Ayarlar > Capabilities**'e gidip **Code Execution and File Creation**'ı aç.
2. **Customize > Skills**'e git.
3. Sağ üstteki **"+"** > **"Create skill"**'e tıkla.
4. Bu repo'daki `omni-prompt` klasörünün **ZIP'ini** yükle (`omni-prompt.zip`).
5. Skill listende görünür; anahtarı açık tut.

> Skill ücretsiz, Pro, Max, Team ve Enterprise planlarında çalışır. Yüklediğin skill'ler hesabına özeldir.

### Claude Code (terminal)

```bash
# Repo'yu klonla
git clone https://github.com/<kullanıcı-adın>/omni-prompt-skill.git

# omni-prompt klasörünü kişisel skill dizinine kopyala
cp -r omni-prompt-skill/omni-prompt ~/.claude/skills/

# Claude Code'da doğrula
/skills
```

---

## Kullanım

Yeni bir sohbette ya konuyu doğrudan yaz (otomatik tetiklenir) ya da başına `/omni-prompt` ekle.

**Örnek 1 — Video**
```
meditasyon uygulaması tanıtım videosu
```

**Örnek 2 — Görsel**
```
kütüphanede ders çalışan insanlar, sıcak ışık
```

**Örnek 3 — Kod**
```
bir klasördeki dosyaları uzantılarına göre ayıran python scripti
```

Her durumda üç katmanlı, üretime hazır bir prompt paketi alırsın.

---

## Güvenlik

Bu skill yalnızca **metin talimatı** içerir — çalıştırılabilir kod veya script yoktur. Yine de genel kural olarak: yalnızca güvendiğin kaynaklardan skill kur ve yüklemeden önce dosyaları incele.

---

## Lisans

MIT License — © 2026 [ismt46](https://github.com/ismt46)

Bu proje MIT lisansı ile lisanslanmıştır. Kaynak göstererek serbestçe kullanabilir, kopyalayabilir, değiştirebilir ve dağıtabilirsin.
