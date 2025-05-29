# 04. Software Design Principles

---

## What Are Software Design Principles?

Software design principles are foundational guidelines that inform and shape the architecture, structure, and implementation of software systems. They help engineers build code that is robust, maintainable, adaptable, and easy to understand. Following these principles leads to improved code quality, fewer bugs, and lower costs in the long run.

---

## Why Are Design Principles Important?

- **Maintainability:** Well-designed code is easier to modify, extend, and debug.
- **Reusability:** Promotes code/components that can be reused across multiple projects.
- **Scalability:** Encourages designs that can grow with system requirements.
- **Readability:** Makes code easier for others (and your future self) to understand.
- **Testability:** Simplifies writing and running tests for your code.
- **Collaboration:** Reduces friction when working in teams by establishing shared standards.

---

## Key Principles (Expanded)

### 1. SOLID Principles

These five principles, introduced by Robert C. Martin ("Uncle Bob"), are pillars of object-oriented design but also apply more broadly:

- **S: Single Responsibility Principle (SRP)**
  - A class or module should have one, and only one, reason to change.
  - Example: Separate logic for data access, business rules, and UI.

- **O: Open/Closed Principle**
  - Software entities (classes, modules, functions) should be open for extension but closed for modification.
  - Example: Use interfaces or abstract classes to add new features without changing existing code.

- **L: Liskov Substitution Principle**
  - Objects of a superclass should be replaceable with objects of a subclass without breaking correctness.
  - Example: Subclasses should not throw unexpected exceptions or require special handling.

- **I: Interface Segregation Principle**
  - No client should be forced to depend on methods it does not use.
  - Example: Prefer several small, specific interfaces over a single large, general-purpose one.

- **D: Dependency Inversion Principle**
  - Depend upon abstractions, not concretions. High-level modules should not depend on low-level modules.
  - Example: Use dependency injection to provide dependencies.

---

### 2. DRY: Don’t Repeat Yourself

- Avoid duplication of code and logic.
- Centralize logic, so changes are made in one place only.
- Example: Extract common validation logic into a reusable function.

---

### 3. KISS: Keep It Simple, Stupid

- Strive for the simplest solution that solves the problem.
- Avoid unnecessary complexity.
- Example: Prefer straightforward loops over clever but obscure recursion.

---

### 4. YAGNI: You Aren’t Gonna Need It

- Don’t implement functionality until it’s necessary.
- Avoid speculative generality and over-engineering.
- Example: Don’t add configuration options that aren’t requested by users.

---

### 5. Separation of Concerns

- Each part of a program should address a separate concern or responsibility.
- Example: MVC (Model-View-Controller) frameworks separate data, UI, and logic.

---

### 6. Modularity

- Divide a system into distinct components or modules with well-defined interfaces.
- Makes individual modules easier to develop and test.

---

### 7. Law of Demeter (Principle of Least Knowledge)

- A module should only communicate with its immediate friends.
- Reduces coupling and makes code more robust to changes.

---

### 8. Favor Composition Over Inheritance

- Prefer assembling small, focused objects via composition rather than deep inheritance hierarchies.
- Leads to more flexible and maintainable designs.

---

## Cohesion and Coupling

- **Cohesion:** The degree to which elements within a module belong together. High cohesion is preferred.
- **Coupling:** The degree of interdependence between modules. Low coupling is desired.

| Aspect     | Good Practice       | Bad Practice         |
|------------|--------------------|---------------------|
| Cohesion   | High               | Low                 |
| Coupling   | Low                | High                |

---

## Example: Applying SOLID (Python)

```python
# SRP Violation:
class UserManager:
    def save_user(self, user): ...
    def send_email(self, user, msg): ...  # Email logic mixed in

# SRP Adherence:
class UserManager:
    def save_user(self, user): ...
class EmailSender:
    def send_email(self, user, msg): ...
```

---

## Example: Favor Composition

```python
class Engine:
    def start(self): ...

class Car:
    def __init__(self, engine):
        self.engine = engine
    def drive(self):
        self.engine.start()
```

---

## Design Principle Violations ("Code Smells")

- Large classes ("God objects")
- Long methods/functions
- Duplicate code
- Tight coupling between modules
- Feature envy (one class overly depends on another)
- Primitive obsession (using basic types when richer objects are needed)
- Inappropriate intimacy (modules know too much about each other)

---

## How to Apply Principles in Practice

- Regularly perform code reviews.
- Refactor as you go; don't wait for major rewrites.
- Use design patterns judiciously—don’t force them.
- Write and maintain tests to support safe refactoring.
- Document rationale for architectural decisions.

---

## Interview Questions

1. What is the Single Responsibility Principle? Give an example.
2. How does the Open/Closed Principle help with maintainability?
3. Explain the difference between high cohesion and low coupling.
4. What are the dangers of violating DRY?
5. Why is composition often favored over inheritance?

---

## Further Reading and References

- [SOLID Principles (Wikipedia)](https://en.wikipedia.org/wiki/SOLID)
- [Clean Code by Robert C. Martin](https://www.oreilly.com/library/view/clean-code/9780136083238/)
- [Refactoring Guru: Design Principles](https://refactoring.guru/design-principles)
- [Martin Fowler: Code Smells](https://martinfowler.com/bliki/CodeSmell.html)
- [Design Patterns: Elements of Reusable Object-Oriented Software](https://en.wikipedia.org/wiki/Design_Patterns)
- [Effective Java by Joshua Bloch](https://www.oreilly.com/library/view/effective-java/9780134686097/)

---

## Exercises

1. Refactor a function with duplicated logic using DRY.
2. Identify violations of SOLID in a sample class and correct them.
3. Explore a codebase and find examples of high coupling and low cohesion.
4. Rewrite an inheritance-based model using composition.
5. Write a brief essay on the importance of KISS and YAGNI in agile development.

---

## Summary

Software design principles are essential for building sustainable, high-quality systems. Mastering them will improve your effectiveness as an engineer and set you apart in interviews and real-world projects.

---
