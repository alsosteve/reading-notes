# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 301

# Read: 08 - APIs

## Reading

### [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)
1. REST stands for Representational State Transfer.
2. REST APIs are designed around a  resources, which are any kind of object, data, or service that can be accessed by the client.
3. A URI can uniquely identify a resource.
4. The most common HTTP verbs are Get, Post, Put, Delete.
5. URI’s should be based on nouns and not verbs.
6. Examples:

``` javascript
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid
```

7. Chatty web API is one that exposes a large amount of small resources.
8. A successful Get request returns 200.
9. An unsuccessful Get request returns 404.
10. A successful Post request returns 201.
11. A successful Delete request returns 204.
