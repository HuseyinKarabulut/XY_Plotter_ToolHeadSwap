# XY_Plotter_ToolHeadSwap
# XY Plotter Project - README (English)

This project is a multi-purpose XY Plotter system capable of moving along the X and Y axes, designed to operate with different tool modules such as a pen, laser, and small CNC motor. The system is built entirely using **Ender 3 V2’s original mechanical parts and electronics**.

**Note:** The project is currently **under development**, and the mechanical, electronic, and firmware components are still being improved.

---

## 🚀 Project Overview

This XY Plotter utilizes:

* Original Ender 3 V2 frame and mechanical parts
* X/Y belt system and linear motion components
* Ender 3 V2 mainboard (4.2.2 or 4.2.7)
* Stock NEMA17 stepper motors

The machine supports three primary operating modes:

* **Pen Mode** – drawing, writing, simple robotics
* **Laser Mode** – engraving and light cutting
* **Motor Mode** – light CNC applications

The Z-axis is used only for pen and CNC motor lifting mechanisms. It is **not used** in laser mode.

---

## 🧰 Hardware Requirements

### Mainboard

* Ender 3 V2 Mainboard (4.2.2 or 4.2.7)
* Ender 3 V2 Color LCD (non-CR Touch version)

### Motors

* X Axis: NEMA17
* Y Axis: NEMA17
* Z Axis: NEMA17 (pen/motor lifting mechanism)

### Drivers

* Pre-installed TMC2208 / TMC2209 / A4988 depending on board model

### Additional Components

* Z Endstop (to be added)
* GT2 belts
* 5mm laser module (for laser mode)
* Pen holder mechanism
* CNC motor holder

### Output Ports

* **FAN0 → Used for laser module output**
* **Z Endstop → Used as Z-axis home reference**

---

## 🔧 Firmware Information

This project is based on **Marlin firmware**, but detailed configuration files and code sections have been intentionally removed because the project is still being developed.

Once the hardware and mechanical structure are finalized, firmware configuration details will be added.

---

## 📝 Usage (In Development)

The functional usage system for pen, laser, and CNC modes is still in progress.

The following sections will be added after development:

* Pen Mode operation
* Laser Mode safety and PWM control
* CNC Motor Mode lifting and toolpath logic

**Note:** The XY Plotter is currently *under construction*, and not all functions have been implemented yet.

---

## 📁 Project Structure

The full file structure will be published once development is complete. It will include:

* Mechanical STL files
* Firmware configuration files
* Example G-code files
* Assembly diagrams

---

## ⚙️ Calibration Steps (Planned)

1. Configure X and Y axis limits
2. Install and test the Z endstop
3. Test FAN0 output for laser control
4. Adjust pen Z-height
5. Add tool mode selection menu to LCD

---

## 🛡️ Safety Notes

* Always use protective goggles when operating the laser module 🔥
* Do not connect high-power devices to FAN0 output
* Keep hands away from moving mechanical parts

---

## 📌 Future Improvements

* Wireless G-code sending (ESP32 + Klipper Bridge)
* Automatic pen height calibration
* Multi-tool quick-change system

---
# XY Plotter Projesi - README (Türkçe)

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



