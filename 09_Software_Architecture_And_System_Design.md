# 09. Software Architecture & System Design

---

## What is Software Architecture?

Software architecture is the high-level organization of a system, describing its major components, their responsibilities, and how they interact. Good architecture supports scalability, maintainability, and robustness.

---

## Why is Architecture Important?

- **Sets the foundation for development.**
- **Guides decision-making throughout the project.**
- **Enables scalability and performance.**
- **Facilitates maintainability and extensibility.**
- **Helps manage complexity.**

---

## Architecture Patterns

- **Monolithic:** All-in-one application.
- **Layered (n-tier):** Presentation, business, data layers.
- **Client-Server:** Separate client and backend.
- **Microservices:** Small, independent services.
- **Event-Driven:** React to events, decoupled components.
- **Service-Oriented Architecture (SOA):** Communicating services.

---

## System Design Process

1. **Requirement Analysis**
    - Functional and non-functional requirements.
2. **Component Identification**
    - Define modules and their responsibilities.
3. **Choose Architecture**
    - Pick a pattern based on needs.
4. **Define Interfaces**
    - APIs, contracts, and integration points.
5. **Data Management**
    - Storage, consistency, caching, and backup.
6. **Scalability & Performance**
    - Load balancing, replication, sharding.
7. **Security**
    - Authentication, authorization, encryption.
8. **Monitoring & Logging**
    - Observability, health checks, alerts.
9. **Deployment**
    - Cloud, containers, CI/CD.

---

## Designing for Scalability

- **Vertical Scaling:** Add resources to a single machine.
- **Horizontal Scaling:** Add more machines.
- **Caching:** Use Redis, Memcached.
- **Load Balancing:** Distribute traffic (Nginx, HAProxy).
- **CDN:** Serve static content globally.

---

## Designing for Reliability

- **Redundancy:** Duplicate critical components.
- **Failover:** Automatic switch to backup systems.
- **Replication:** Multiple copies of data.
- **Graceful Degradation:** Partial functionality during failures.

---

## Example: 3-Tier Web Application

- **Presentation Layer:** UI/Frontend.
- **Business Logic Layer:** API/services.
- **Data Layer:** Database/storage.

---

## Diagrams

- **UML:** Class, sequence, deployment, component diagrams.
- **ERD:** Entity-relationship for databases.
- **Architecture Diagrams:** High-level overview.

---

## System Design Interviews

- Clarify requirements and constraints.
- Estimate scale: users, requests per second, data size.
- Draw high-level architecture first.
- Discuss bottlenecks and trade-offs.
- Address consistency, availability, and partition tolerance (CAP theorem).

---

## Common System Design Questions

1. Design Twitter/Instagram backend.
2. How would you build a scalable URL shortener?
3. Design a file storage service (like Dropbox).
4. How to architect a real-time chat application?
5. How would you handle millions of users uploading photos?

---

## Best Practices

- Keep it simple—avoid overengineering.
- Document architectural decisions.
- Use industry standards and proven patterns.
- Review and iterate on architecture regularly.

---

## References

- [System Design Primer](https://github.com/donnemartin/system-design-primer)
- [Martin Fowler: Architecture](https://martinfowler.com/architecture/)
- [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected/)

---

## Exercises

1. Draw a high-level architecture diagram for an e-commerce website.
2. List trade-offs between monolithic and microservices architectures.
3. Simulate scaling a web app from 1,000 to 1 million users.
4. Design the backend for a ride-sharing application.
5. Write a document justifying your architectural choices for a sample project.

---

## Summary

Software architecture and system design define how software is built and how it will grow. Mastering this area is crucial for advanced engineering roles and technical interviews.

---
