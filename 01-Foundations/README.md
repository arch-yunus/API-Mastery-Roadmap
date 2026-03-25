# 01. Temeller: Çekirdek Mekanikler

Bu modül, modern web iletişiminin %99'una güç veren temel protokolleri ve standartları kapsar. Bu temelleri anlamak, bir API Ustası olmayı hedefleyen herkes için tartışmaya kapalıdır.

## 📖 Kapsanan Konular

### 1. HTTP Protokolü (Kalp Atışı)
*   **Statelessness (Durumsuzluk)**: Ölçeklenebilirlik için neden önemlidir?
*   **HTTP Metotları**: GET/POST'un ötesi (PUT vs PATCH, HEAD, OPTIONS).
*   **Header'lar (Başlıklar)**: Content-Type, Accept, Cache-Control, ETag.

### 2. Durum Kodları (API'ların Dili)
| Aralık | Kategori | Amaç |
| :--- | :--- | :--- |
| **1xx** | Bilgilendirme | Protokol değişimi, işleme. |
| **2xx** | Başarı | Her şey yolunda gitti. (POST için 201 şart!) |
| **3xx** | Yönlendirme | Kaynaklar taşındı. |
| **4xx** | İstemci Hatası | İsteği yapan kontratı bozdu. |
| **5xx** | Sunucu Hatası | Sistem dahili olarak başarısız oldu. |

### 3. REST vs SOAP
*   **REST**: Mimari stil, durumsuz (stateless), kaynak tabanlı.
*   **SOAP**: Protokol tabanlı, katı XML, yerleşik ACID uyumluluğu.

## 🚀 Laboratuvar Egzersizleri
*   [Laboratuvar 01: curl ile HTTP Uzmanlığı](labs/01-curl-commands.md)
