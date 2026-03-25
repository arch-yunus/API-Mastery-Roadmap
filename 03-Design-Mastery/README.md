# 03. Tasarım Uzmanlığı: Zarif Kontratlar İnşa Etmek

Bir API tasarlamak kolaydır. On yıl sürecek *zarif* bir API tasarlamak ise bir sanattır.

## 📖 Kapsanan Konular

### 1. Kaynak Odaklı Tasarım
*   **Adlandırma Protokolleri**: Çoğul isimler, kebab-case vs snake_case.
*   **Alt Kaynaklar**: URI içindeki ilişkiler (örn: `/users/{id}/orders`).

### 2. Evrim ve Versiyonlama
*   **URI Versiyonlama**: `/v1/resource` (Klasik).
*   **Header Versiyonlama**: `X-API-Version` (Daha temiz).
*   **Media Type Versiyonlama**: `Accept: application/vnd.myapi.v1+json` (Gerçek REST).

### 3. Dayanıklılık ve Kontrol
*   **Idempotency (Aynı Etkililik)**: Yeniden denemelerin işlemleri çoğaltmamasını sağlamak (örn: `Idempotency-Key`).
*   **Sayfalama (Pagination)**: Cursor-tabanlı vs Offset-tabanlı.
*   **Rate Limiting**: Sınırlama stratejileri (Leaky Bucket vs Token Bucket).

---
[Ana Yol Haritasına Dön](../README.md)
