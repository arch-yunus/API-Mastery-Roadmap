# 🧪 Laboratuvar 01: `curl` ile HTTP Uzmanlığı

Bu laboratuvarda, mock bir API ile etkileşim kurmak için `curl` kullanacak ve header'ların (başlıklar) ve metotların sunucu yanıtını tam olarak nasıl etkilediğini anlayacaksınız.

## 🛠 Ön Koşullar
`curl`'ün kurulu olduğundan emin olun. Kontrol etmek için `curl --version` komutunu çalıştırın.

## 📝 Egzersizler

### 1. Ayrıntılı GET (Verbose GET)
Bir kaynağı çekin ve tam başlık değişimini inceleyin.
```bash
curl -v https://jsonplaceholder.typicode.com/posts/1
```
> **Gözlem**: `> GET` (İstek) ve `< HTTP/1.1 200 OK` (Yanıt) satırlarını arayın.

### 2. Özel Başlıklar ve İçerik Pazarlığı (Content Negotiation)
Sunucuya JSON yerine XML tercih ettiğinizi söyleyin (eğer destekleniyorsa).
```bash
curl -H "Accept: application/xml" https://jsonplaceholder.typicode.com/posts/1
```

### 3. Idempotent PUT
Bir kaynağı güncelleyin. Bu komutu birden çok kez çalıştırmanın aynı durumla sonuçlandığına dikkat edin.
```bash
curl -X PUT -H "Content-Type: application/json" \
     -d '{"title": "Güncellenmiş Başlık", "body": "bar", "userId": 1}' \
     https://jsonplaceholder.typicode.com/posts/1
```

### 4. `ETag` İncelemesi (Önbellek Kontrolü)
Gövdeyi çekmeden kaynağın değişip değişmediğini görmek için bir HEAD isteği çalıştırın.
```bash
curl -I https://jsonplaceholder.typicode.com/posts/1
```

---
[Temeller Modülüne Dön](../README.md)
