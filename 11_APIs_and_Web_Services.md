# 11. APIs & Web Services

---

## What is an API?

An API (Application Programming Interface) is a set of rules, protocols, and tools that allows different software components to communicate with each other. APIs expose specific functionalities or data, enabling integration and interoperability between systems.

---

## What is a Web Service?

A web service is a type of API that is accessible over a network (usually HTTP/HTTPS). It enables communication between systems, regardless of platform or language, using standard protocols.

---

## Types of Web Services

- **REST (Representational State Transfer):**
  - Uses standard HTTP methods: GET, POST, PUT, DELETE.
  - Resource-oriented, stateless, supports JSON/XML.
  - Widely used for modern APIs.

- **SOAP (Simple Object Access Protocol):**
  - Uses XML for messaging.
  - Strict standards, built-in error handling, and security.
  - Common in enterprise and legacy systems.

- **GraphQL:**
  - Query language for APIs.
  - Clients specify exactly what data they need.
  - Single endpoint, flexible and efficient.

---

## RESTful API Principles

- **Stateless:** No client context is stored on the server between requests.
- **Resource-Based:** Everything is a resource (users, products, orders).
- **Use of HTTP Verbs:** GET (read), POST (create), PUT/PATCH (update), DELETE (remove).
- **Standard Status Codes:** 200 OK, 201 Created, 400 Bad Request, 401 Unauthorized, 404 Not Found, 500 Server Error.

---

## Example: REST API Endpoints

```
GET /api/users/123         # Get user with ID 123
POST /api/users            # Create a new user
PUT /api/users/123         # Update user 123
DELETE /api/users/123      # Delete user 123
```

---

## API Authentication & Security

- **API Keys:** Simple, but should be kept secret.
- **OAuth 2.0:** Industry standard for delegated authorization.
- **JWT (JSON Web Tokens):** Secure, compact, self-contained tokens.
- **Basic Auth:** Username and password in HTTP headers (not recommended for sensitive data).
- **TLS/SSL:** Always use HTTPS to encrypt data in transit.

---

## Best Practices

- Use versioning (`/api/v1/`).
- Validate and sanitize all input.
- Implement rate limiting and throttling.
- Provide clear, consistent error messages.
- Write and maintain comprehensive API documentation.
- Use standard HTTP status codes.
- Log and monitor API usage.

---

## API Documentation Tools

- **Swagger/OpenAPI:** Interactive documentation and contract-first API development.
- **Postman Collections:** Document and test APIs.
- **RAML, Apiary:** Alternative documentation/specification tools.

---

## Testing APIs

- Use tools like Postman, curl, and automated test suites.
- Test for correct functionality, edge cases, and error handling.

---

## Design Considerations

- **Idempotence:** Repeating an operation produces the same result.
- **Pagination:** Chunk large data sets for efficiency.
- **Filtering and Sorting:** Allow clients to specify data needs.
- **Caching:** Use HTTP cache headers for performance.

---

## GraphQL vs REST

| Feature          | REST                   | GraphQL                |
|------------------|------------------------|------------------------|
| Endpoints        | Multiple               | Single                 |
| Data retrieval   | Fixed structure        | Client-defined         |
| Over-fetching    | Common                 | Avoided                |
| Under-fetching   | Possible               | Avoided                |
| Tooling          | Mature                 | Rapidly growing        |

---

## API Gateways

- Central point for managing, authenticating, and routing API requests.
- Add security, analytics, rate limiting, and caching.
- Examples: Kong, AWS API Gateway, Apigee.

---

## API Rate Limiting

- Protects APIs from misuse and abuse.
- Common strategies: IP-based, user-based, token bucket, leaky bucket.

---

## Webhooks

- Allow external systems to receive real-time notifications (push) when events happen.
- Example: GitHub sending a POST request to your server when a repo is pushed.

---

## Interview Questions

1. What is the difference between REST and SOAP?
2. How do you secure an API?
3. When would you use GraphQL over REST?
4. What status codes would you use for a failed authentication?
5. How do you handle backward compatibility for APIs?

---

## References

- [RESTful API Tutorial](https://restfulapi.net/)
- [Swagger/OpenAPI](https://swagger.io/)
- [GraphQL Official Site](https://graphql.org/)
- [Postman](https://www.postman.com/)

---

## Exercises

1. Design a simple RESTful API for a todo application.
2. Implement rate limiting for an endpoint.
3. Write a Postman collection to test a user registration API.
4. Document an existing API using Swagger/OpenAPI.
5. Compare REST and GraphQL for a given use case.

---

## Summary

APIs and web services are the backbone of modern software systems, enabling integration, automation, and flexibility. Understanding their principles, security, and best practices is essential for every software engineer.

---
