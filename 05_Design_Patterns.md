# 05. Design Patterns

---

## What Are Design Patterns?

Design patterns are tried-and-tested solutions to common software design problems. They provide templates and best practices for structuring code, improving maintainability, and facilitating communication among engineers. Unlike frameworks or libraries, patterns are conceptual blueprints, not code.

---

## Why Are Design Patterns Important?

- **Reusability:** Leverage proven solutions for recurring challenges.
- **Efficiency:** Avoid reinventing the wheel.
- **Maintainability:** Simplify code changes and bug fixes.
- **Communication:** Provide a shared vocabulary for developers.
- **Scalability:** Facilitate the evolution and extension of systems.

---

## Categories of Design Patterns

### 1. Creational Patterns

Handle object creation mechanisms.

- **Singleton:** Ensures a class has only one instance.
- **Factory Method:** Defines an interface for creating an object, but lets subclasses alter the type.
- **Abstract Factory:** Creates families of related objects.
- **Builder:** Separates object construction from its representation.
- **Prototype:** Clones existing objects.

### 2. Structural Patterns

Deal with object composition.

- **Adapter:** Makes incompatible interfaces compatible.
- **Decorator:** Adds new behavior to objects dynamically.
- **Facade:** Provides a simplified interface to a complex system.
- **Composite:** Treats individual objects and compositions uniformly.
- **Proxy:** Provides a surrogate for another object.

### 3. Behavioral Patterns

Define ways objects interact and distribute responsibility.

- **Observer:** Notifies dependent objects of changes.
- **Strategy:** Allows selecting an algorithm at runtime.
- **Command:** Encapsulates requests as objects.
- **State:** Alters behavior when an object changes state.
- **Iterator:** Provides a way to access elements sequentially.
- **Chain of Responsibility:** Passes requests along a chain of handlers.

---

## Example: Singleton Pattern (Python)

```python
class Singleton:
    _instance = None
    def __new__(cls):
        if not cls._instance:
            cls._instance = super().__new__(cls)
        return cls._instance
```
Use: Logging, configuration classes.

---

## Example: Factory Pattern (Python)

```python
class Animal:
    def speak(self):
        pass

class Dog(Animal):
    def speak(self):
        return "Woof!"

class Cat(Animal):
    def speak(self):
        return "Meow!"

class AnimalFactory:
    @staticmethod
    def get_animal(animal_type):
        if animal_type == 'dog':
            return Dog()
        elif animal_type == 'cat':
            return Cat()
        else:
            return None

a = AnimalFactory.get_animal('dog')
print(a.speak())
```

---

## Example: Observer Pattern

Used in GUIs, event-driven systems, and publish/subscribe models.

---

## How to Choose a Pattern

1. **Understand the Problem:** Identify recurring structural, creational, or behavioral issues.
2. **Match the Pattern:** Use documentation or pattern catalogs.
3. **Apply Judiciously:** Not every problem needs a pattern—avoid overengineering.

---

## Common Mistakes

- Overusing patterns when a simple solution suffices.
- Using patterns without fully understanding them.
- Neglecting to document the intent of the chosen pattern.

---

## Pattern Catalogs

- "Gang of Four" book: Design Patterns: Elements of Reusable Object-Oriented Software.
- [Refactoring Guru: Pattern Catalog](https://refactoring.guru/design-patterns/catalog)
- [SourceMaking](https://sourcemaking.com/design_patterns)

---

## Interview Questions

1. Explain the difference between Factory and Abstract Factory.
2. When would you use the Observer pattern?
3. How does the Strategy pattern support open/closed principle?
4. Give a real-world use case for the Proxy pattern.
5. What are the pros and cons of the Singleton pattern?

---

## References

- [Design Patterns: Elements of Reusable Object-Oriented Software](https://en.wikipedia.org/wiki/Design_Patterns)
- [Refactoring Guru Patterns Catalog](https://refactoring.guru/design-patterns/catalog)
- [SourceMaking Patterns](https://sourcemaking.com/design_patterns)

---

## Exercises

1. Implement a Singleton logger in your favorite programming language.
2. Use the Factory pattern to create different types of notifications (email, SMS).
3. Identify a use case from your experience for the Observer pattern.
4. Refactor a legacy code segment using the Decorator pattern.
5. Write a short essay on when not to use design patterns.

---

## Summary

Design patterns are essential tools for software engineers. Mastering them can dramatically improve your design skills and help you shine in interviews and real-world projects.

---
