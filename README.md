# 🎮 GridMind

**ARC-Style Pattern Puzzle Game**

GridMind, ARC (Abstraction and Reasoning Corpus) tarzı bir bulmaca oyunudur. Blokları hareket ettirerek hedef deseni oluşturun!

![GridMind Screenshot](screenshot.png)

## 🎯 Oyun Hakkında

GridMind'da amacınız, farklı davranışlara sahip blokları hareket ettirerek ekranda gösterilen hedef deseni (pattern) oluşturmaktır. Her blok tipi farklı şekilde hareket eder veya renk değiştirir.

## 🕹️ Nasıl Oynanır?

1. Ekranın üstündeki **Target Pattern** hedef deseninizi gösterir
2. Grid üzerindeki blokları **yön tuşları** veya **D-pad** ile hareket ettirin
3. Blokları hedef alana getirip doğru renklerde hizalayın
4. Süre bitmeden deseni tamamlayın!

## 🧱 Blok Tipleri

| Blok | Sembol | Davranış |
|------|--------|----------|
| **Classic** | → | Normal yönde hareket eder |
| **Reverse** | ← | Ters yönde hareket eder |
| **Static** | ◆ | Hareket etmez, sadece renk değiştirir |
| **Hybrid** | ⟳ | Hareket eder + renk değiştirir |
| **Rev.Hybrid** | ⟲ | Ters hareket + renk değiştirir |

## 🎲 Oyun Modları

### Random Mode
- Prosedürel üretilen sonsuz seviyeler
- Kademeli artan zorluk
- Ne kadar ileri gidebilirsin?

### Campaign Mode
- Önceden tasarlanmış seviyeler
- JSON formatında level pack yükleme
- LocalStorage'a kaydedilir (bir kere yükle, hep oyna)

## 🎮 Kontroller

| Platform | Kontrol |
|----------|---------|
| **Klavye** | Arrow Keys veya WASD |
| **Mobil** | Ekrandaki D-pad butonları |
| **Pause** | ESC tuşu veya ⏸ butonu |

## 📁 Dosyalar

```
GridMind/
├── index.html          # Ana oyun dosyası
├── gridmind_designer.html  # Level tasarlama aracı
├── README.md           # Bu dosya
└── levels/             # (Opsiyonel) Level pack dosyaları
    └── campaign.json
```

## 🛠️ Level Designer

Kendi bölümlerinizi tasarlamak için `gridmind_designer.html` dosyasını kullanın:

1. **Araç seçin**: Wall, Classic, Reverse, Static, Hybrid, Rev.Hybrid
2. **Renk seçin**: 9 farklı renk
3. **Grid'e tıklayın**: Blok ve duvarları yerleştirin
4. **Target Area**: Boyut seçip grid üzerine yerleştirin
5. **Pattern düzenleyin**: Preview'da hedef renkleri ayarlayın
6. **Kaydet**: Level adı, süre ve zorluk girin
7. **İndir**: Tüm levelleri JSON olarak indirin

## 🚀 Kurulum

### Yerel Çalıştırma
Herhangi bir sunucuya ihtiyaç duymadan doğrudan tarayıcıda açabilirsiniz:

```bash
# Dosyayı tarayıcıda açın
open index.html
# veya
start index.html  # Windows
```

### Web Sunucusu ile
```bash
# Python ile basit sunucu
python -m http.server 8000

# Node.js ile
npx serve
```

## 📱 Özellikler

- ✅ Tamamen responsive tasarım
- ✅ Mobil uyumlu (touch controls)
- ✅ Offline çalışır (tek HTML dosyası)
- ✅ Replay sistemi (oyunları kaydet ve izle)
- ✅ LocalStorage ile level pack kaydetme
- ✅ 25+ kademeli zorluk seviyesi
- ✅ Pause/Resume desteği
- ✅ Cyberpunk neon tema

## 🔄 Replay Sistemi

- Oyunlarınız otomatik kaydedilir
- Game Over ekranından **Watch Replay** ile izleyin
- **Download Replay** ile JSON olarak indirin
- Ana menüden **Load Replay File** ile tekrar izleyin
- Hız kontrolü: 0.5x, 1x, 2x, 4x

## 📊 Puanlama

```
Puan = (Pattern Genişliği × Yüksekliği × 20) + (Kalan Süre × 2)
```

Daha büyük patternler ve hızlı çözümler = daha yüksek puan!

## 🎨 Teknolojiler

- Vanilla JavaScript (framework yok)
- CSS Grid & Flexbox
- LocalStorage API
- Tek HTML dosyası (~2000 satır)

## 📄 Lisans

MIT License - Dilediğiniz gibi kullanabilirsiniz.

## 🤝 Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request açın

## 📞 İletişim

Sorularınız için issue açabilirsiniz.

---

**Enjoy the game! 🎮**
