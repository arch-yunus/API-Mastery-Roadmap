# 02. Mimari Desenler: Çeşitli İletişim Stratejileri

REST endüstri standardı olsa da, modern sistemler genellikle esneklik için GraphQL veya performans için gRPC gibi alternatifler gerektirir.

## 📖 Kapsanan Konular

### 1. GraphQL
*   **Şema Odaklı Yaklaşım**: Tipleri, sorguları (queries) ve mutasyonları tasarlamak.
*   **Resolver Deseni**: Sorguların veri kaynaklarıyla nasıl eşleştiği.
*   **Performans**: Data Loader'lar ile N+1 problemini çözmek.

### 2. gRPC
*   **Protocol Buffers (Protobuf)**: Dilden bağımsız ikili (binary) serileştirme.
*   **Tek Yönlü vs Çift Yönlü Akış**: Yüksek verimli servisler arası iletişime güç vermek.
*   **Kod Üretimi**: `protoc` kullanımı.

### 3. Gerçek Zamanlı ve Olay Odaklı (Event-Driven)
*   **Webhook'lar**: Otomatik bildirimler için tersine API'lar.
*   **WebSocket'ler**: Çift yönlü tam-dupleks iletişim.
*   **SSE (Server-Sent Events)**: Paneller (dashboards) için tekten çoğa olay akışı.

## 🚀 Laboratuvar Egzersizleri
*   [Laboratuvar 03: GraphQL vs REST (Analiz)](labs/01-graphql-vs-rest.md)

---
[Ana Yol Haritasına Dön](../README.md)
