# XY_Plotter_ToolHeadSwap
# XY Plotter Projesi - README

Bu proje, X ve Y eksenlerinde hareket edebilen; kalem, lazer ve motor gibi farklı uç modülleri kullanılabilen çok amaçlı bir XY Plotter sistemini içerir. Ender 3 V2 kartı (4.2.2 / 4.2.7) baz alınarak geliştirilmiştir.

---

## 🚀 Proje Özeti

Bu XY Plotter tamamen **Ender 3 V2'nin orijinal mekanik parçaları ve elektronik donanımı** kullanılarak tasarlanmıştır. Gövde, kızaklar, kayış sistemi, motorlar ve kontrol kartı Ender 3 V2 altyapısından uyarlanmıştır.

Bu XY Plotter:

* **Kalem modu** (çizim, yazı, robotik kol)
* **Lazer modu** (ahşap yakma, kazıma)
* **Motor modu** (küçük CNC uygulamaları)

olmak üzere 3 farklı çalışma modunu destekler.

Z ekseni, kalem ve motor modlarında **step motor ile kaldırma/indirme mekanizması** olarak kullanılır. Lazer modunda Z ekseni kullanılmaz.

---

## 🧰 Donanım Gereksinimleri

### Ana Kart

* Ender 3 V2 kartı (4.2.2 veya 4.2.7)
* Color LCD (CR Touch olmayan sürüm)

### Motorlar

* X Ekseni: NEMA17
* Y Ekseni: NEMA17
* Z Ekseni: NEMA17 (Kalem/kaldırma mekanizması için)

### Sürücüler

* TMC2208 / TMC2209 / A4988 (kart üzerinde hazır geliyor)

### Ek Parçalar

* Z Endstop (eklenecek)
* GT2 kayışlar
* 5mm lazer modülü (Lazer modu için)
* Kalem tutucu mekanizması
* Motor tutucu (CNC modu için)

### Çıkışlar

* **FAN0 → Lazer modülü çıkışı** olarak kullanılacak
* **Z Endstop → Z ekseninin referans pozisyonu**

---

## 🔧 Yazılım Ayarları

Bu proje Marlin yazılımı kullanılarak yapılandırılır. (**Proje şu anda yapım aşamasındadır.**) Mod sistemi, donanım uyarlamaları ve mekanik bileşenlerin tamamı geliştirilmeye devam etmektedir.

Kod ve firmware yapılandırmaları proje tamamlandığında eklenmek üzere kaldırılmıştır.

---

## 📝 Kullanım

Bu bölüm proje tamamlandığında detaylandırılacaktır. Kalem, lazer ve motor modlarının çalışma prensipleri geliştirme sürecindedir.

**Not:** XY Plotter hâlâ *yapım aşamasındadır* ve tüm fonksiyonlar tamamlanmamıştır.

---

## 📁 Dosya Yapısı

Proje hâlen geliştirildiğinden klasör yapısı tamamlanmamıştır. Donanım çizimleri, hareketli parçaların STL dosyaları ve kullanım dokümanları ilerleyen aşamalarda eklenecektir.

```

---

## ⚙️ Kalibrasyon Adımları
1. X ve Y ekseni limitlerini ayarlayın.
2. Z endstop ekleyin ve test edin.
3. FAN0 çıkışını test edin.
4. Kalem tutucunun Z yüksekliğini ayarlayın.
5. LCD üzerinden mod seçimini kontrol edin.

---

## 🛡️ Güvenlik Notları
- Lazer kullanımında mutlaka koruyucu gözlük kullanılmalıdır! 🔥
- FAN0 çıkışı yüksek güçler için kullanılmamalıdır.
- Hareketli bölgelerde elinizi unutmayın.

---

## 📌 Gelecek Geliştirmeler
- Kablosuz G-code gönderme (ESP32 Klipper Bridge)
- Otomatik kalem kalibrasyonu
- Çoklu uç değiştirme aparatı

---
