# 06. Altyapı ve CI/CD: Ekosistemi Orkestre Etmek

Bir API, ancak onu barındıran ve izleyen altyapı kadar iyidir.

## 📖 Kapsanan Konular

### 1. API Gateway'ler ve Service Mesh
*   **Gateway'ler**: Kenar yönlendirme, kimlik doğrulama yükünü hafifletme ve yük dengeleme (Kong, Tyk).
*   **Service Mesh**: Servisler arası iletişim ve karşılıklı TLS (Istio, Linkerd).

### 2. Gözlemlenebilirlik ve İzleme
*   **Tracing (İzleme)**: Jaeger veya Zipkin ile dağıtık izleme.
*   **Logging (Günlükleme)**: Merkezi toplama (ELK Stack, Datadog).
*   **Metrikler**: Prometheus ile altın sinyaller (Gecikme, Trafik, Hatalar, Doygunluk).

### 3. CI/CD ve Otomasyon
*   **SDK Üretimi**: OpenAPI spesifikasyonlarından istemci kütüphaneleri üretmek.
*   **Bozucu Değişiklik Tespiti**: Geriye dönük uyumluluk için sürekli entegrasyon testleri.
*   **Dağıtım Stratejileri**: API'lar için Mavi/Yeşil ve Kanarya dağıtımları.

---
[Ana Yol Haritasına Dön](../README.md)
