# 04. Test Mükemmelliği: Sıfır Hata Stratejileri

Test, profesyonel bir dağıtım (deployment) ile üretim (production) felaketi arasındaki tampondur.

## 📖 Kapsanan Konular

### 1. API'lar için Test Piramidi
*   **Birim (Unit) Testleri**: Controller veya servis içindeki mantık.
*   **Entegrasyon Testleri**: Veritabanlarını ve harici bağımlılıkları doğrulamak.
*   **Kontrat Testi**: Değişikliklerin sistemi bozmamasını sağlamak için Pact/Spring Cloud Contract.

### 2. Otomasyon Araçları
*   **Postman/Newman**: Koleksiyon yönetimi ve CI entegrasyonu.
*   **RestAssured (Java)**: JVM tabanlı API testleri için altın standart.
*   **Supertest (Node.js)**: JS ekosistemi için hızlı ve etkileyici test setleri.

### 3. Performans ve Kaos
*   **K6**: JavaScript ile geliştirici odaklı yük testi.
*   **JMeter**: Endüstriyel düzeyde stres testi.
*   **Resilience (Dayanıklılık) Testleri**: Yeniden deneme mantığını test etmek için gecikme (latency) ve hata enjekte etmek.

---
[Ana Yol Haritasına Dön](../README.md)
