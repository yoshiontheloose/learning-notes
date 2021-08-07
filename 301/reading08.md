# APIs, RegExr

## API Design Best Practices

Source (https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

---

**What does REST stand for?**

Representational State Transfer

**REST APIs are designed around a ____.**

Resource. Resources can be objects, data, or a service accessed by the client.

**What is an identifer of a resource? Give an example.**

URI - uniform resource identifier

- identifies a resource

Example:  
website/api path/identifier

```
"https://adventure-works.com/orders/1"
```

**What are the most common HTTP verbs?**

- GET

- POST

- PUT

- PATCH

- DELETE

**What should the URIs be based on?**

"Resource URIs should be based on nouns" which are the resource

Verbs are the operations in the resource so they should not be verbs.

**Give an example of a good URI.**

```
"https://adventure-works.com/orders // Good"

"https://adventure-works.com/create-order // Avoid"
```

Resources should show up to the client in a singular fashion rather than be exposed to the internal process.

It's good to give URIs consistent naming systems so they may be reffered to as collections. Also keep them simple. - Plural nouns is a good example.

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

Chatty APIs are not good because they bring more requests to the server if they have a large amount of resources exposed.

**What status code does a successful GET request return?**

Status code 200

**What status code does an unsuccessful GET request return?**

404 not found

**What status code does a successful POST request return?**

HTTP status code 201

**What status code does a successful DELETE request return?**

HTTP status code 204

---

POST - creates a resource

PUT - creates a resource or updates a resource that already exists

PATCH - makes a partial update to an existing resource

<br>

---

### Additional Sources Provided by Reading Topic

[RegExr](https://regexr.com/)

[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)

[Regex 101](https://regex101.com/)

<br>

[<<<Back](README.md)