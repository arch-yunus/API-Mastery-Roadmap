# 🧪 Laboratuvar 03: GraphQL vs REST (Over-fetching Analizi)

Bu laboratuvarda, REST ve GraphQL arasındaki yanıt boyutu ve istek sayısını karşılaştıracaksınız.

## 📝 Egzersizler

### 1. REST Şelalesi (Waterfall)
REST'te bir kullanıcıyı ve gönderi başlıklarını almak için:
1.  `GET /users/1`
2.  `GET /users/1/posts`
> **Sorun**: Sadece 2 alana ihtiyacınız varken 50 alan alabilirsiniz. Buna **Over-fetching (Aşırı Veri Çekme)** denir.

### 2. GraphQL Cerrahi Müdahalesi
Aynı işlemi tek bir sorguda gerçekleştirin:
```graphql
query GetUserPosts {
  user(id: "1") {
    name
    posts {
      title
    }
  }
}
```
> **Avantaj**: Sıfır over-fetching. Tek bir gidiş-dönüş (round-trip).

---
[Mimari Desenler Modülüne Dön](../README.md)
