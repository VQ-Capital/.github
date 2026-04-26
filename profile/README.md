<div align="center">
  <h1>🦅 VQ-Capital (Vector Quantitative Capital)</h1>
  <p><b>Institutional Grade Event-Driven Algorithmic Trading Infrastructure</b></p>
</div>

VQ-Capital, mikro saniye hassasiyetinde veri işleyen, sıfır gecikmeli (zero-latency) mesajlaşma omurgasına sahip ve yapay zeka (LLM/SLM) ile istatistiksel benzerlik (Vector Search) algoritmalarını uçta (Edge) birleştiren yeni nesil bir HFT altyapısıdır.

## 🧠 Felsefemiz (The VQ Way)
1. **Zero Python in Hot Path:** Veri akışı, normalizasyon ve emir iletimi katmanlarında sadece **Rust** ve **C++** kullanılır.
2. **Zero JSON in IPC:** Servisler arası iletişimde JSON yasaktır. Tüm veri paketleri **Protobuf** formatında serileştirilir.
3. **Zero HTTP (Internal):** Mikroservisler birbirleriyle HTTP REST üzerinden konuşmaz. Tüm iletişim **NATS JetStream** üzerinden olay güdümlü (Event-Driven) yapılır.
4. **Vector Memory over Time-Series:** Gelecek tahmin edilmez, mevcut durumun geçmişe benzerliği aranır (**Qdrant**).

## 🖥️ Sentinel Terminal (Live Observability)
Sistemimiz, `sentinel-*` önekiyle adlandırılmış, kesin sınırlarla ayrılmış mikroservislerden oluşur. Tüm sistemin tek doğruluk kaynağı (Source of Truth) `sentinel-spec` reposudur. 

Aşağıda, otonom yapay zeka ajanlarımızın aldığı aksiyonları, Z-Score sapmalarını ve borsa gecikmelerini (SLA) anlık izlediğimiz, sıfır-bağımlılık (Zero-Dependency) ile geliştirilen **Read-Only Quant Dashboard** yer almaktadır.

<div align="center">
  <!-- Masaüstü Ekranı (Geniş) -->
  <img src="desktop.png" alt="HFT Data Visualization & Monitoring - Desktop" width="100%" style="border-radius: 8px; border: 1px solid #333;">
  <br><br>
  <!-- Mobil Ekran (Dar) -->
  <img src="mobile.png" alt="HFT Data Visualization & Monitoring - Mobile" width="40%" style="border-radius: 8px; border: 1px solid #333;">
</div>

<br>

---
<div align="center">
  <i>"Speed is not just for profit; it is for survival."</i>
</div>