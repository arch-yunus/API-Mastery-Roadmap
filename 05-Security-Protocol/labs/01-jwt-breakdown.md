# 🧪 Laboratuvar 02: JWT'yi (JSON Web Token) Parçalara Ayırma

API'lardaki dijital kimlik büyük ölçüde JWT'lere dayanır. Bu laboratuvarda, bir token'ın katmanlarını soymayı öğreneceksiniz.

## 🛠 Ön Koşullar
*   Web Tarayıcısı veya `node.js`.
*   [jwt.io](https://jwt.io) (Referans Araç).

## 📝 Egzersizler

### 1. Bir Token'ın Anatomisi
Bir JWT, noktalarla ayrılmış üç bölümden oluşur: `Header.Payload.Signature`.
*   **Header (Başlık)**: Algoritmayı belirtir (HS256, RS256).
*   **Payload (Yük)**: "Talepler" (Kullanıcı Kimliği, Sona Erme Süresi, Roller).
*   **Signature (İmza)**: Token'ın kurcalanmadığını kanıtlar.

### 2. Base64 vs Şifreleme
**KRİTİK**: JWT'ler şifrelenmiş DEĞİL, kodlanmıştır (genellikle). Token'a sahip olan herkes yükünüzü (payload) çözebilir.
*   Bir mock sağlayıcıdan token'ınızı kopyalayın.
*   Tarayıcı konsolunuzda `atob()` içine yapıştırın:
```javascript
let payload = "eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ";
console.log(JSON.parse(atob(payload)));
```

### 3. Sır (Secret) ile İmzalama
Bir HS256 token oluşturmak için bir araç kullanın ve bir gizli anahtar (secret key) ile doğrulayın.
> **Gözlem**: Yükteki 1 karakteri bile değiştirmek imzayı geçersiz kılar. Bu, API güvenliğinin temelidir.

---
[Güvenlik Modülüne Dön](../README.md)
