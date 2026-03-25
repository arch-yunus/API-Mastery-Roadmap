# 05. Güvenlik Protokolü: Geçidi Sertleştirmek

Güvenlik bir özellik değil; yüksek yetkili API'ların temel bir özelliğidir.

## 📖 Kapsanan Konular

### 1. Kimlik Doğrulama ve Yetkilendirme
*   **OAuth 2.1**: Kapsamlar (Scopes), İzin Türleri (Grant Types) ve Yetkilendirme Kodları.
*   **OIDC (OpenID Connect)**: OAuth üzerindeki kimlik katmanı.
*   **JWT (JSON Web Tokens)**: Talepler (Claims), İmza doğrulama ve JWS/JWE.

### 2. OWASP API Security Top 10
*   **BOLA (Broken Object Level Authorization)**: 1 numaralı API zafiyeti.
*   **BFLA (Broken Function Level Authorization)**: Yönetici işlevlerine yetkisiz erişim.
*   **Mass Assignment**: Hassas alanların kontrolsüz güncellenmesi.

### 3. Savunma Yapılandırması
*   **CORS**: Güvenli çapraz köken kaynak paylaşımı.
*   **CSP (Content Security Policy)**: Yanıtlarda XSS'i önlemek.
*   **IP Beyaz Listeye Alma ve VPN**: Kurumsal düzeyde API izolasyonu.

## 🚀 Laboratuvar Egzersizleri
*   [Laboratuvar 02: JWT'yi Detaylı İnceleme](labs/01-jwt-breakdown.md)

---
[Ana Yol Haritasına Dön](../README.md)
