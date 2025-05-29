# 14. Security in Software Engineering

---

## Why is Security Important?

Security ensures the confidentiality, integrity, and availability of software systems and user data. With increasing threats and attacks, security must be a core concern throughout the software development lifecycle.

---

## Security Principles

- **Least Privilege:** Only grant the minimum access required.
- **Defense in Depth:** Multiple layers of security controls.
- **Fail Securely:** Systems should default to a secure state on failure.
- **Secure by Design:** Security is built in from the start, not added later.

---

## Common Vulnerabilities

- **SQL Injection:** Unsanitized input in SQL queries.
- **Cross-Site Scripting (XSS):** Malicious scripts in user inputs.
- **Cross-Site Request Forgery (CSRF):** Unintended actions via authenticated sessions.
- **Sensitive Data Exposure:** Unencrypted sensitive information.
- **Broken Authentication:** Weak session management or password handling.

---

## Secure Coding Practices

- Validate and sanitize all inputs.
- Use parameterized queries for SQL.
- Store passwords securely (hash + salt).
- Avoid hard-coded secrets.
- Use HTTPS everywhere.
- Implement strong authentication and session management.

---

## Authentication & Authorization

- **Authentication:** Verifies user identity (passwords, OAuth, SSO, biometrics).
- **Authorization:** Determines user permissions (role-based access control).

---

## Security Testing

- **Static Application Security Testing (SAST):** Analyze source code for vulnerabilities.
- **Dynamic Application Security Testing (DAST):** Test running applications.
- **Penetration Testing:** Simulate real-world attacks.

---

## Threat Modeling

- Identify assets, threats, and vulnerabilities.
- Use models like STRIDE (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege).

---

## OWASP Top 10

Familiarize yourself with the [OWASP Top 10](https://owasp.org/www-project-top-ten/), the most critical security risks for web applications:
- Injection
- Broken Authentication
- Sensitive Data Exposure
- XML External Entities (XXE)
- Broken Access Control
- Security Misconfiguration
- Cross-Site Scripting (XSS)
- Insecure Deserialization
- Using Components with Known Vulnerabilities
- Insufficient Logging & Monitoring

---

## Security in DevOps (DevSecOps)

- Integrate security into CI/CD pipelines.
- Automate security scans and compliance checks.
- Use secrets management tools (Vault, AWS Secrets Manager).

---

## Regulations & Compliance

- **GDPR:** Data privacy in Europe.
- **HIPAA:** Healthcare data in the US.
- **PCI-DSS:** Payment card industry standards.

---

## Incident Response

- Preparation, detection, containment, eradication, recovery, lessons learned.
- Maintain logs, monitor systems, and have a response plan.

---

## Interview Questions

1. How do you prevent SQL injection?
2. What is the difference between authentication and authorization?
3. Explain a time you secured an application.
4. What tools do you use for security testing?
5. How do you manage secrets in applications?

---

## References

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [Mozilla Web Security Guidelines](https://infosec.mozilla.org/guidelines/web_security.html)
- [Google Security Blog](https://security.googleblog.com/)

---

## Exercises

1. Find and fix security vulnerabilities in a sample codebase.
2. Implement password hashing and salting.
3. Set up HTTPS on a local server.
4. Perform a basic penetration test with OWASP ZAP.
5. Write secure authentication logic for a login page.

---

## Summary

Security must be a priority for all software engineers. Building secure systems protects users, organizations, and your own reputation.

---
