# 🧪 Lab 03: GraphQL vs REST (Over-fetching Analysis)

In this lab, you compare the payload size and number of requests between REST and GraphQL.

## 📝 Exercises

### 1. The REST Waterfall
To get a user and their post titles in REST:
1.  `GET /users/1`
2.  `GET /users/1/posts`
> **Issue**: You might get 50 fields when you only needed 2. This is **Over-fetching**.

### 2. The GraphQL Surgical Strike
Perform the same operation in a single query:
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
> **Benefit**: Zero over-fetching. One round-trip.

---
[Return to Module Architectural Patterns](../README.md)
