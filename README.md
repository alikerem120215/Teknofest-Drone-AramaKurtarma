# 🛰️ Teknofest — DJI Mini Drone Enkaz Altı Arama-Kurtarma Taşıyıcı Kartı

Bu proje; deprem ve afet durumlarında enkaz altı arama-kurtarma çalışmalarına destek vermek üzere **DJI Mini Drone** platformuna entegre edilebilir **ESP32, LoRa ve GPS** tabanlı donanım taşıyıcı kart tasarımını içerir.

---

## 📐 Tasarım & Donanım Özellikleri
- **Mikrodenetleyici:** ESP32 (Düşük güç tüketimi, dahili Wi-Fi & Bluetooth).
- **Uzun Menzilli İletişim:** LoRa 433/868 MHz modülü ile baz istasyonu olmadan kilometrelerce menzilden telemetri ve canlı sinyal iletimi.
- **Konumlandırma:** GPS modülü ile hassas enlem/boylam koordinat tespiti.
- **Güç Yönetimi:** Drone bataryasından veya harici 1S/2S LiPo pilden regüle besleme.

---

## 📁 Dosya Yapısı
- `circuit.kicad_sch` — KiCad 8 şematik çizim dosyası.
- `easyeda_pcb.json` — EasyEDA web tabanlı PCB tasarım ve yerleşim şablonu.
- `gerber_pack/` — Endüstriyel PCB üreticilerine (JLCPCB, PCBWay vb.) doğrudan gönderilmeye hazır Gerber paketi:
  - Bakır katmanları (`.gtl`, `.gbl`)
  - Lehim maskesi (`.gts`, `.gbs`)
  - Serigrafi baskı (`.gto`)
  - Delik delme koordinatları (`drill_file.drl`)
  - Malzeme Listesi (`BOM.csv`) ve Bağlantı Raporu (`Netlist_Report.txt`)
